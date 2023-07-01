
# HCL AppScan Enterprise (ASE) - Overview

The AppScan Enterprise plug-in provides integration with an HCL AppScan Enterprise server. This
plug-in retrieves the security vulnerability report of the application and displays it as metrics in insights.


## Compatibility

Must be running UrbanCode Velocity version 1.2.1 and later to use the plug-in.

## Versions

There is no install process for this plug-in. The AppScan Enterprise plug-in is identified to UrbanCode
Velocity as a value stream integration. UrbanCode Velocity plug-in images are located in DockerHub and the UrbanCode
Velolcity code accesses the version that you select. To view available versions, see the [UrbanCode
DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-appscan/tags).

## History

### Version 2.0.47

* **Preventing Syncing of plugin on older Versions of ASE**: This version of HCL Appscan Enterprise plugin sync's appscan data only when appscan enterprise version is 10.0.0 or greater than 10.0.0. Plugin throws error if appscan enterprise version is older and no syncing of appscan data happens.
* **Disabled certificate verification**: Disabled strict certificate verification for REST API calls made by plugin.

### Version 2.0.41

* **Removed Manual User Access Key**: From current version onwards this plugin will only support Auto Generated User Access Key feature of Urbancode Velocity.
* **Initial Sync Date Field Added**: Under the hidden properties section of add integration page for the HCL Appscan Enterprise plugin an Initial Sync Date field is added. This field is optional and can be used only for the first sync.
* **Added WorkflowId**: Under the hidden properties section of add integration page for HCL Appscan Enterprise plugin a Workflow ID field is added. This field is optional and can be used to provide Urbancode Velocity WorkflowId - the ID of a Value Stream (VSM )to which HCL Appscan Enterprise vulnerability data is associated.
* **Preventing Installation on Older Versions**: This version of HCL Appscan Enterprise Plugin can only be installed on Urbancode Velocity version 3.0.0 and later

### Version 2.0.35

* Scheduled Event Functionality Added
* UAK Changes
* Issue Level Data Chart Added

### Version 1.0.31

* Removed IBM related keywords

### Version 1.0.30

* Updated data retrieval logic

### Version 1.0.23

* Bug fix.

### Version 1.0.21

* Added Build URL to link Appscan Enterprise scan results in VSM.

### Version 1.0.20

* Bug fix.

### Version 1.0.16

* Update plugin version from 0.x.x to 1.x.x format.

### Version 0.0.13

* Initial release

|Back to ...||Latest Version|HCL AppScan Enterprise (ASE) |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[2.0.47](https://github.com/UrbanCode/IBM-UCV-PLUGINS/raw/main/files/ucv-ext-appscan/ucv-ext-appscan:2.0.47.tar.7z.001)|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
