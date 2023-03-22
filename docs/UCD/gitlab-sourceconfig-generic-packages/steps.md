# GitLab Generic Packages - Process Steps

* [GitLab Generic Packages Component Properties](#comp-prop)


### GitLab Generic Packages Component Properties

Create versions and import packaged files from GitLab.


| Name | Type | Description                                                                                                          | Required |
| ---- | ---- | -------------------------------------------------------------------------------------------------------------------- | -------- |
| Server URL | String | The Base URL and port for the GitLab server. | Yes |
| Access Token | String | The access token to use to authenticate with the GitLab server. | No |
| Project Id | String | The project ID in GitLab. | Yes |
| Package Name | Boolean | The exact name of package that must match to import a specific package. | Yes |
| Status | String | The package status. It can be default (default) or hidden. | No |
| File Includes | String | A list of file patterns to include in the component. Separate each pattern with a new line or comma. To include all files, leave blank or type **/*. | No |
| File Excludes | String | A list of file patterns to exclude from the component. Separate each pattern with a new line or comma. | No |
| Extensions of files to Convert | String | If text-type files must be converted into another character set, type the list of file extensions to be converted. Matching file types are converted into the default or system character set of the system where the agent is located. Separate list items with commas. | No |
| Log4j Logging Level | Boolean | Configure the level of Log4j messages to output to the console. Specify the logging level as ALL, TRACE, DEBUG, INFO, WARN, ERROR, FATAL, or OFF. | No |



|          Back to ...          ||         Latest Version         |GitLab Generic Packages|||||
|:-----------------------------:|:------------------------------:| :---: | :---: | :---: | :---: | :---: | :---: |
| [All Plugins](../../index.md) | [Deploy Plugins](../README.md) |[1.1147446](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/gitlab-sourceconfig-generic-packages/ucd-plugins-sourceconfig-gitlab-generic-packages-1.1147446.zip)|[Overview](overview.md)|[Usage](usage.md)|[Downloads](downloads.md)|
