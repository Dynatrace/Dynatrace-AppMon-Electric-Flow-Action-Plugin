# ElectricFlow Action Plugin
Dynatrace Action Plugin for Electric Flow. Allows to make requests to Electric Flow API.

# Installation

Import the Plugin into the Dynatrace Server. Refer to Dynatrace documentation for more details.


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

