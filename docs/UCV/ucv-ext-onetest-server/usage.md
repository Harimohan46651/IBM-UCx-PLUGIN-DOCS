
# HCL DevOps Test Server - Usage

To use the HCL DevOps Test Server plug-in you must define the integration, create a value stream, and upload the integration.

The value stream map contains the properties, you will use to define the plug-in integration. Basically, the plug-in integration is defined with a value stream within the DevOps Velocity user interface. Defining the integration includes defining configuration properties that connect the DevOps Velocity server to the DevOps Test server.

The basic flow to use the plug-in includes:

1. Download the value stream map. The value stream map is a JSON file used to define integrations.
2. Edit the JSON file to include the plug-in configuration properties.
3. Save and upload the JSON file. This replaces the current JSON file with the new content.
4. View the new integration on the Integration user interface page.

You can map a build to a metric using tags defined on the DevOps Test server by evaluating the tag against a regular express. Use the Build Label Pattern field to define the regular expression. For example, a build expression of “([A-Z]+-[0-9]+)” and a test has a tag of “BUILD-123”, the build is mapped with ID BUILD-123 in the DevOps Velocity server to the newly created metric. For assistance in forming a regular expression, see the [Regular expression tester](https://regexr.com) website. You can use the website to help form and test a regular expression based on your build ID.

## Integration type

The HCL DevOps Test Server plug-in supports endpoint integration which are listed in the following table.


| Name | Path | Method |
| --- | --- | --- |
| OneTestEndpoint | onetest/callback | Post |

## Integration

From the user interface Value Steam page, click **Upload** to upload the value stream map which is a JSON file.

The JSON file contains the information for creating a value stream and integrating with the DevOps Test server. The following table describes the information for the creating a DevOps Velocity value stream map.


| Name | Description | Required |
| --- | --- | --- |
| image | The version of the plug-in that you want to use. To view available versions, see the [UrbanCode DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-onetest-server/tags). If a value is not specified, the latest version is used. | No |
| name | An assigned name to the value stream. | Yes |
| loggingLevel | The level of Log4j messages to log. Valid values are: all, debug, info, warn, error, fatal, off, and trace. The default is info. | No |
| properties | List of [configuration properties](#properties) used to connect and communicate with the DevOps Test server.Enclose the properties within braces. | Yes |
| tenant\_id | The name of the tenant. | Yes |
| type | Unique identifier assigned to the plug-in. The value for the HCL DevOps Test Server plug-in is `ucv-ext-onetest-server`. | Yes |

## Configuration Properties

The configuration properties which are included in the `properties` field are unique to the
HCL DevOps Test Server plug-in and define the connection and communication to the DevOps Test server.


| Name | Property Name | Type | Description | Required |
| --- | --- | --- | --- | --- |
| Build Label Pattern | buildRegExp | String | A regular expression pattern that will match a build ID on a test execution label. For example: ([A-Z]+-[0-9]+). | No |
| HCL DevOps Test Offline User Token | oneTestRefreshToken | String | The offline user token created in the HCL DevOps Test user interface by clicking the Create Token button. | Yes |
| HCL DevOps Test Server URL | oneTestUrl | String | The base URL of the HCL DevOps Test Server. For example: https://tp-cicd2.nonprod.hclpnp.com. | Yes |
| Workflow Id | WorkflowId | String | The value stream that this metric is associated. | No |
| DevOps Velocity User Access Key | ucvAccessKey | String | The user access key to authenticate with the DevOps Velocity server. | No |

## Example

The following example can be used as as template to include the AppScan plug-in integration into the JSON file. Copy and paste the template into the JSON file and make the appropriate changes.


```

"integrations": [
{

"type": "ucv-ext-onetest-server",
"tenant_id": "",
"name": "",
"logginglevel": "INFO",

"properties":{
"ucvAccessKey": "",
"oneTestUrl" : "",
"oneTestRefreshToken":"",

"buildRegExp": "([A-Z]+-[0-9]+)"
}``
}``
]

```



|Back to ...||Latest Version|HCL DevOps Test Server |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[1.0.17](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-onetest-server/ucv-ext-onetest-server-1.0.17.tar.7z.001)|[Readme](README.md)|[Overview](overview.md)|[Downloads](downloads.md)|
