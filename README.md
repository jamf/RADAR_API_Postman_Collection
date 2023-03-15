# RADAR - Postman API Collection

## Overview
This collection is provided to assist Jamf Security Cloud (RADAR) users of the Risk API. It provides a quick method to interact with all non-deprecated endpoints.

This article describes the recommended Postman configuration and setup process to import the collection, configure variables to connect it to your Jamf Security Cloud environment and begin testing API calls and interacting with the Risk API.

The following expectations were used when designing this collection:
* All POST operations include a pre-populated request body.
  - This request body may not include all fields supported by the body of the given object, however it will include those required to successfully create the object.
  - Pull requests or issue submissions are encouraged to enhance or update this data.
* All GET operations include at least one example response.
  - Endpoints that have conditional inputs in the form of parameters or request bodies should include multiple examples (e.g. `override`).
* All query parameters that have a defined list of acceptable values denote the allowed values in the description of the parameter.

## Import the Collection
Use the following options to import the collection into Postman:
* Click the [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/19047489-1a8f6a3f-89d6-43d0-9120-23efaa140db3?action=collection%2Fimport) button to automatically import the collection into your Postman app.
* In Postman, click File >> Import.
  - Download the JSON included in this repo and select the .json file.

## Define Environment Variables
This collection utilizes the following variables which should be defined within the environment variables. Using variables at the collection level is not currently supported by the script that performs that authorization token requests. Follow Postman's documentation to [Manage Environments](https://learning.getpostman.com/docs/postman/environments_and_globals/manage_environments).

| Variable           | Description                                                | Example                   |
|--------------      |-------------------------------------------------           |---------------------------|
| application_ID     | Application Id to authenticate to Jamf Security Cloud with       | 23a55907-11240-9cec-bce9-6e666943b59e             |
| application_Secret | Application Secret of the Application ID to Jamf Security Cloud  | gBKbS)?y_VDw7CxSS_dj                 |


## Getting Started
After the collection has been imported and valid values have been defined for the variables, all calls should be supported with minimal input required. Additional data will be required either in the form of a parameter value and/or a request body.