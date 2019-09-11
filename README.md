[<img src="https://sling.apache.org/res/logos/sling.png"/>](https://sling.apache.org)

 [![Build Status](https://builds.apache.org/buildStatus/icon?job=Sling/sling-org-apache-sling-bnd-plugin-headers-parameters-remove/master)](https://builds.apache.org/job/Sling/job/sling-org-apache-sling-bnd-plugin-headers-parameters-remove/job/master) [![Test Status](https://img.shields.io/jenkins/t/https/builds.apache.org/job/Sling/job/sling-org-apache-sling-bnd-plugin-headers-parameters-remove/job/master.svg)](https://builds.apache.org/job/Sling/job/sling-org-apache-sling-bnd-plugin-headers-parameters-remove/job/master/test_results_analyzer/) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

# Apache Sling bnd Remove Parameters from OSGi Headers Plugin

This module is part of the [Apache Sling](https://sling.apache.org) project.

This module provides a plugin for [bnd](https://bnd.bndtools.org) to remove parameters from OSGi headers.

Example instruction (for bnd file):

````
-plugin:\
  org.apache.sling.bnd.plugin.headers.parameters.remove.Plugin;\
    'Require-Capability'='osgi.service;filter:="(objectClass=org.osgi.service.event.EventHandler)";effective:=active;cardinality:=multiple'
````
