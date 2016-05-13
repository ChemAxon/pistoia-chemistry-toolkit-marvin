# pistoia-chemistry-toolkit-marvin project details

## Overview
This project is part of Pistoia <a href="https://github.com/PistoiaHELM/HELM2NotationToolkit">HELM2NotationToolkit</a> 
for handling biological molecules with supporting <a href="http://www.pistoiaalliance.org/projects/hierarchical-editing-language-for-macromolecules-helm/">HELM</a> 
and HELM2 formats.<br/>
This chemistry plugin provides chemical logic by ChemAxon's Marvin beans behind to monomers of biomolecules.

## Requirements for the build
Java 1.7, <br/>
Maven 3 or higher <br/>
This plug-in is depending on ChemistryToolkit, so you need to access an artifact of this project from a public (or local) maven repository.

## The deployed version
The most simple way for using this plug-in is to download the deployed version from ChemAxon's <a href="https://repository.chemaxon.com/artifactory/webapp/login.html?0">artifact repository</a>.
You can reference the ChemAxon Public Repository in your Maven project's pom.xml:
<pre>
&lt;repositories&gt;
    &lt;repository&gt;
        &lt;id&gt;ChemAxon Public Repository&lt;/id&gt;
        &lt;url&gt;https://repository.chemaxon.com/artifactory/libs-release&lt;/url&gt;
    &lt;/repository&gt;
&lt;/repositories&gt;
 
&lt;dependencies&gt;
    &lt;dependency&gt;
        &lt;groupId&gt;com.chemaxon&lt;/groupId&gt;
        &lt;artifactId&gt;ChemistryTookitMarvin&lt;/artifactId&gt;
        &lt;version&gt;15.5.4.0&lt;/version&gt;
    &lt;/dependency&gt;
&lt;/dependencies&gt;
</pre><br/>
This is not an open repository, username and password is required.<br/>
You can add your account info in settings.xml:<br/>
<pre>
&lt;servers&gt;
  &lt;server&gt;
    &lt;id&gt;ChemAxon Public Repository&lt;/id&gt;
    &lt;username&gt;Your username&lt;/username&gt;
    &lt;password&gt;Your password&lt;/password&gt;
  &lt;/server&gt;
&lt;/servers&gt;
&lt;/pre&gt;
&lt;br/&gt;
</pre>
Note that in order to obtain access rights, you will need to send a request to maven-repo-request@chemaxon.com (it is free).

## Using the plug-in
You need a valid <a href="https://docs.chemaxon.com/display/docs/About+ChemAxon+Licensing+LIC">Marvin license</a>, which ChemAxon grants at no charge for usage within the context of the Pistoia Alliance HELM project, and the plugin's jar file has to be in the classpath.
