# ElectricFlow Action Plugin

ElectricFlow is an enterprise-grade DevOps Release Automation platform that simplifies provisioning, build and release of multi-tiered applications. This plugin enables bi-directional integration between ElectricFlow and Dynatrace. It allows ElectricFlow users the ability to uncover performance issues much earlier in the delivery pipeline. ElectricFlow Action plugin enables closed feedback loop, where automated actions such as rollbacks can be triggered based on Dynatrace incidents.

Key feature of integration includes:

* Control Release Pipeline progress using performance and architectural metrics from Dynatrace

* Create production deployment incidents in Dynatrace to aid troubleshooting of performance issues

* Trigger automated actions such as rollbacks in ElectricFlow based on Dynatrace incidents and policies

* End-to-end visibility in Release Pipelines of success/degradation from baselines, and in Dynatrace of deployment details including application, environment and pipeline information


# Installation

In order to install ElectricFlow Action plugin, import the plugin jar file into the Dynatrace Server. Refer to Dynatrace documentation for more details.

To install Dynatrace plugin on ElectricFlow system, please go to [Dynatrace - Electric Cloud](https://electric-cloud.com/plugins/directory/p/dynatrace) for further information.


# Configuration

In order to configure ElectricFlow action plugin, please follow the steps:

1. Select the Dynatrace incident that you want to setup and open Edit dialog.
2. Under Actions tab, add ElectricFlow action. Choose 'on incident begin' for Execution.
3. Set up the following ElectricFlow specific configurations
* ElectricFlow API End-Point: ElectricFlow Server API URL or end-point (for example https://<electric-flow-server>)
* ElectricFlow Username: ElectricFlow User Name
* ElectricFlow Password: ElectricFlow User Password
* Method: HTTP Request Method (for example POST). Only POST and PUT methods are currently supported.
* Parameters: HTTP Request Parameters for ElectricFlow API call, in key=value pairs. For example, pipelineName=Rollback
* Body: HTTP Request Body

