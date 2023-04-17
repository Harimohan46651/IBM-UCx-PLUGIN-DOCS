
# HCL AppScan on Cloud (ASoC) - Overview


The HCL AppScan on Cloud (ASoC) plugin allows for integration with the HCL Appscan on Cloud server. This plugin uses the Appscan on Cloud REST interface to interact with the HCL Appscan on Cloud application. Data is gathered from the ASoC server and displayed as a graphical view in the UrbanCode Velocity portfolio.

## Compatibility

Must be running UrbanCode Velocity version 1.2.1 and later to use this plug-in.

## Versions

UrbanCode Velocity plug-in images are located in DockerHub. To view available versions, see the [UrbanCode DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-asoc/tags).

## History

### Version 3.0.19

* The older versions of ASoC plugin was not reporting critical issues. The issue is fixed.

### Version 3.0.12

* Removed Manual User Access Key: From current version onwards this plugin will only support Auto Generated User Access Key feature of UrbanCode Velocity.
* Initial Sync Date Field Added: Under the hidden properties section of add integration page for the ASoC plugin an Initial Sync Date field is added. This field is optional and can be used only for the first sync.
* Added WorkflowId: Under the hidden properties section of add integration page for ASoC plugin a Workflow ID field is added. This field is optional and can be used to provide UbranCode Velocity WorkflowId - the ID of a Value Stream (VSM )to which ASoC vulnerability data is associated.
* Preventing Installation on Older Versions: This version of ASoC Plugin can only be installed on UrbanCode Velocity version 2.5.0 and later
* Making scheduled event optional: The scheduled event - Sync ASoC Data has been made optional from this version onwards. To enable the scheduled event please check the box in integration properties with label Run as a Scheduled Event.

### Version 3.0.11

* Fix for Changed API.

### Version 3.0.5

* User access key related changes.

### Version 2.0.1

* Syncs historic data from ASoC. Also webhook support enabled. Note: This is a **breaking change** as the end point changes from ‘POST’ to ‘GET’

### Version 1.0.24

* Proxy support added.

### Version 1.0.18

* Bug fix.

### Version 1.0.17

* Added Build URL to link ASoC scan results in VSM.

### Version 1.0.16

* Bug fixes.

### Version 1.0.14

* Name field in Insights mapped to the scan name in ASoC.

### Version 1.0.13

* Bug fixes.

### Version 1.0.9

* Update plugin version from 0.x.x to 1.x.x format.

### Version 0.0.4

* Initial release


|Back to ...||Latest Version|HCL AppScan on Cloud (ASoC) |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[3.0.19](https://github.com/UrbanCode/IBM-UCV-PLUGINS/raw/main/files/ucv-ext-asoc/ucv-ext-asoc:3.0.19.tar.7z.001)|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
