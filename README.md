# pistoia-chemistry-toolkit-marvin project details

## Overview
This project is part of Pistoia <a href="https://github.com/PistoiaHELM/HELM2NotationToolkit">HELM2NotationToolkit</a> 
for handling biological molecules with supporting <a href="http://www.pistoiaalliance.org/projects/hierarchical-editing-language-for-macromolecules-helm/">HELM</a> 
and HELM2 formats. For more details see the documentation: https://github.com/PistoiaHELM/HELM2NotationToolkit/blob/master/HELM2_overview.docx
This chemistry plugin provides chemical logic by ChemAxon's Marvin beans behind to monomers of biomolecules.

## Reqiurements for the build
Java 1.7, <br/>
Maven 3 or higher <br/>
This plug-in is depending on ChemistryToolkit, so you need to accessing an artifact of this project in a public (or local) maven repository.

## The deployed version
The most simple way for using this plug-in to download the deployed version from ChemAxon's <a href="https://repository.chemaxon.com/artifactory/webapp/login.html?0">artifact repository</a>.
you can reference the ChemAxon Public Repository in your Maven project's pom.xml:
<pre>
&lt;repositories&gt;
    &lt;repository&gt;
        &lt;id&gt;ChemAxon Public Repository&lt;/id&gt;
        <url>https://repository.chemaxon.com/artifactory/libs-release</url>
    </repository>
</repositories>
 
<dependencies>
    <dependency>
        <groupId>com.chemaxon</groupId>
        <artifactId>ChemistryTookitMarvin</artifactId>
        <version>1.0.0</version>
    </dependency>
</dependencies>
</pre><br/>
This is not an open repository, username and password is required.<br/>
You can add your account info in settings.xml:<br/>
<pre>
<servers>
  <server>
    <id>ChemAxon Public Repository</id>
    <username>Your username</username>
    <password>Your password</password>
  </server>
</servers>
</pre>
<br/>
For access rights, please send a request to maven-repo-request@chemaxon.com (it is free).

## Using of the plug-in
You need a valid <a href="https://docs.chemaxon.com/display/docs/About+ChemAxon+Licensing+LIC">Marvin license</a> and the plugin's jar file has to be in the classpath.
