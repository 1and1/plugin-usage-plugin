Plugin Usage
============

This Jenkins plugin gives you the possibility to analyze the usage of your installed Jenkins plugins.

[![Build Status](https://jenkins.ci.cloudbees.com/job/plugins/job/plugin-usage-plugin/badge/icon)](https://jenkins.ci.cloudbees.com/job/plugins/job/plugin-usage-plugin/)

* see [Jenkins wiki](https://wiki.jenkins-ci.org/display/JENKINS/Plugin+Usage+Plugin+(Community)) for detailed feature descriptions
* use [JIRA](https://issues.jenkins-ci.org) to report issues / feature requests

Development
===========

Start the local Jenkins instance:

    mvn hpi:run


How to install
--------------

Run

	mvn clean package

to create the plugin .hpi file.


To install:

1. copy the resulting ./target/plugin-usage-plugin.hpi file to the $JENKINS_HOME/plugins directory. Don't forget to restart Jenkins afterwards.

2. or use the plugin management console (http://example.com:8080/pluginManager/advanced) to upload the hpi file. You have to restart Jenkins in order to find the plugin in the installed plugins list.

Plugin releases
---------------

	mvn release:prepare release:perform

Contributing to the Plugin
==========================

Plugin source code is hosted on [GitHub](https://github.com/jenkinsci/plugin-usage-plugin).
New feature proposals and bug fix proposals should be submitted as
[GitHub pull requests](https://help.github.com/articles/creating-a-pull-request).
Fork the repository on GitHub, prepare your change on your forked
copy, and submit a pull request.  Your pull request will be evaluated
by the [Cloudbees Jenkins job](https://jenkins.ci.cloudbees.com/job/plugins/job/plugin-usage-plugin/)
and you should receive e-mail with the results of the evaluation.

Before submitting your change, please assure that you've added a test
which verifies your change.  Tests help us assure that we're delivering a reliable
plugin, and that we've communicated our intent to other developers in
a way that they can detect when they run tests.

Code coverage reporting is available as a maven target and is actively
monitored.  Please try your best to improve code coverage with tests
when you submit.

Before submitting your change, please review the findbugs output to
assure that you haven't introduced new findbugs warnings.
