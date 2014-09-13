[![Build Status](https://jenkins.ci.cloudbees.com/job/plugins/job/yaml-pipeline-plugin/badge/icon)](https://jenkins.ci.cloudbees.com/job/plugins/job/yaml-pipeline-plugin/)

Jenkins YAML Pipeline / Plugin
=====================
Jenkins Plugin which manages the scripts and the updating of the
Jenkins jobs using a high level abstraction based on YAML in order to create and maintain Jobs and Pipelines as a result.

Background
----------
Job DSL plugin (https://github.com/jenkinsci/job-dsl-plugin/wiki) is a wonderful plugin in order to automate your Jenkins Job creation

```yaml

```


Development
===========

Building
--------
To build the plugin from source:

    ./gradlew build

To run Jenkins and test JPI:

    ./gradlew server

Build job-dsl.hpi to be installed in Jenkins:

    ./gradlew jpi
	
	
How to install
--------------

Run 

	./gradlew hpi:hpi
	
to create the plugin .hpi file.


To install:

1. copy the resulting ./build/yaml-pipeline.hpi file to the $JENKINS_HOME/plugins directory. Don't forget to restart Jenkins afterwards.
	
2. or use the plugin management console (http://example.com:8080/pluginManager/advanced) to upload the hpi file. You have to restart Jenkins in order to find the pluing in the installed plugins list.


Authors
-------
Victor Martinez <VictorMartinezRubio@gmail.com>


License
-------
Licensed under the Apache License, Version 2.0 (the “License”); you may not use this file except in compliance with the
License. You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
“AS IS” BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific
 language governing permissions and limitations under the License.