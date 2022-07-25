## Running the Edgescan task

This toolkit brings in data from Edgescan

To run this task you need the following information from Edgescan:

1. Edgescan Token
1. Kenna connector ID

## Command Line

See the main Toolkit for instructions on running tasks. For this task, if you leave off the Kenna API Key and Kenna Connector ID, the task will create a json file in the default or specified output directory. You can review the file before attempting to upload to the Kenna directly.

Recommended Steps:

1. Run with Edgescan Keys only to ensure you are able to get data properly from the scanner
1. Review output for expected data
1. Create Kenna Data Importer connector in Kenna (example name: Edgescan KDI)
1. Manually run the connector with the json from step 1
1. Click on the name of the connector to get the connector id
1. Run the task with Edgescan Keys and Kenna Key/connector id

Complete list of Options:

| Option | Required | Description | default |
| --- | --- | --- | --- |
| edgescan_token | true | Edgescan Token | n/a |
| edgescan_page_size | false | Edgescan page size | 100 |
| edgescan_api_host | false | Edgescan API Hostname | live.edgescan.com |
| kenna_api_key | false | Kenna API Key | n/a |
| kenna_api_host | false | Kenna API Hostname | api.us.kennasecurity.com |
| kenna_connector_id | true | Kenna connector ID | n/a |
| output_directory | false | The task will write JSON files here (path is relative to /Users/mykola_ukhanskyi/Files/toolkit) | output/edgescan |
| create_findings | false | The task will create findings, instead of vulnerabilities | n/a |
| include_network_vulnerabilities | false | The task will include network layer vulnerabilities | true |
| include_application_vulnerabilities | false | The task will include application layer vulnerabilities | true |

## Support

All issues and inquiries relating to this toolkit implementation must contact Edgescan support.

[comment]: <> (Please add preferred methods to contact Edgescan support.)
