
# Urbancode Deploy - Overview

The UrbanCode Deploy plugin for UrbanCode Velocity synchronizes applications, processes, components, versions, snapshots, teams, environments, and more from UrbanCode Deploy. A Deploy application can be configured as an application in an UrbanCode Velocity pipeline and the UrbanCode Deploy processes can be configured in the UrbanCode Velocity pipeline. The UrbanCode Velocity Pipeline can then display the latest version of the application deployed to different environments.

## Compatibility

The UrbanCode Deploy plug-in requires UrbanCode Velocity version 2.3 or later.

## Versions

UrbanCode Velocity plug-in images are located in DockerHub. To view available versions, see the [UrbanCode DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-ucd/tags).

## History


### Version 3.3.56

* **Removed UrbanCode Deploy Status Task**: Assign status task is removed and made part of main UrbanCode Deploy Task as post deployment success or failure step for assigning Snapshot or Component Version status.


### Version 2.3.52

* **Internal Server Error Fix**: The urbancode deploy plugin was giving internal server error while syncing the application processes from the UCD server.

### Version 2.3.51

* Major Enhancements

### Version 1.0.16

* **Corrected incorrectly spelled plugin name**: In urbancode deploy plugin, display name was incorrectly spelled as Ubrancode deploy. Now corrected to Urbancode deploy.

### Version 1.0.12

* Importing failed application deployment history.

### Version 1.0.11

* User AccessKey Related Changes.

### Version 1.0.10

* Initial release.


|Back to ...||Latest Version|Urbancode Deploy |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[3.3.56 - File 1](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-ucd/ucv-ext-ucd:3.3.56.tar.7z.001) [3.3.56 - File 2](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-ucd/ucv-ext-ucd:3.3.56.tar.7z.002)|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
