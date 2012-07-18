A jenkins plugin for leiningen builds.

## Installation

For now this has to be installed manually, the following steps should
be taken:

* compile the hpi plugin with: `mvn package`
* in jenkins, go to "configure jenkins" then advanced and upload the resulting .hpi file to jenkins
* restart jenkins
* in jenkins main configuration, set the full path to the leiningen standalone JAR (as found here: https://github.com/downloads/technomancy/leiningen/leiningen-2.0.0-preview7-standalone.jar)
* jobs can now be created with leiningen build steps 

## Tips

If you want to archive artifacts, you will have to specify the path to the artifacts you want archived in a post build step `target/*.jar` or `target/*.war` for lein2 works perfectly
