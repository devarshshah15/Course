In creating your pipeline, you must be able to create a build server that is capable of building a target project.  Please have a target platform in mind (java, .net, node.js, web, etc.).  Otherwise, the default project will be [deeplearning4j](https://github.com/SkymindIO/deeplearning4j/).

The build server must support the following properties.

* The ability to trigger a build in response to a git commit via a [git hook](http://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks).
* The ability to setup dependencies for the project and restore to a clean state.
* The ability to execute a build script (e.g., shell, maven)
* The ability to run a build on multiple nodes (e.g. [jenkins slaves](https://wiki.jenkins-ci.org/display/JENKINS/Distributed+builds), [go agents](https://github.com/kmugrage/go-agent-docker), or a spawned droplet/AWS.).
* The ability to retrieve the status of the build via http.

In creating your build server, you have the option of configuring an existing tool, such as Jenkins or GoCD, or of using a minimal build setup via scripts/code (e.g., automating the docker technique in the workshop).


### Evaluation

* Triggered Builds - 20%
* Dependency Management - 20%
* Build Script Execution - 20%
* Multiple Nodes - 20%
* Status - 20%