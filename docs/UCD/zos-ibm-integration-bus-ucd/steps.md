
IBM Integration Bus (IIB) plugin Deploy step for zOS - Steps
============================================================

# Steps



### Steps




 



Process steps in the  plug-in
-----------------------------


* zOS Deploy


Deploy a Broker 
Archive. This step will set the output property ‘completionCode’, representing the last completion code returned from 
the broker during deployment.




Input properties for zOS Deploy
-------------------------------




| Name | Type | 
Description | Required |
| --- | --- | --- | --- |
| Bar File Names | String | Comma or new line separated list of 
Broker Archive files to deploy. | Yes |
| Execution Groups | String | Comma or new line separated list of Execution 
Groups to Deploy to. | Yes |
| Deployment Type | **Enumeration:** Full Incremental ```${p?:iib.deployType}``` | Specify 
either an incremental or full deployment. You may specify the ‘```${p?:iib.deployType}``'` option and set the 
`'iib.deployType'` property to either ‘incremental’ or ‘full’ at any level in the property hierarchy. | No |
| 
Start/Stop Message Flows | Boolean | Check to stop all Message Flows in the Execution Group before deployment and start 
all Message Flows after deployment. | No |
| IP | String | The ip address of the target server for a remote connection. 
You must specify either an ‘IP’ and ‘Port’ to connect to a remote broker or an ‘Integration Node Name’ to connect to a 
local broker. | No |
| Port | String | The port of the target server for a remote connection. You must specify either an
 ‘IP’ and ‘Port’ to connect to a remote broker or an ‘Integration Node Name’ to connect to a local broker. | No |
| Port
 | String | The port of the target server for a remote connection. You must specify either an ‘IP’ and ‘Port’ to connect
 to a remote broker or an ‘Integration Node Name’ to connect to a local broker. | No |
| Use SSL | Boolean | 
Administration security authentication/authorization. This option is only available in IIB version 10. | No |
| 
Integration Node Name | String | Name of Integration Node. You must specify either an ‘IP’ and ‘Port’ to connect to a 
remote broker or an ‘Integration Node Name’ to connect to a local broker. | No |
| Username | String | Username for 
secure authentication. Explicit user authentication only available with IIB 10. | No |
| Password | String | Password 
for secure authentication. Explicit user authentication only available with IIB 10. | No |
| Trace File | String | The 
file to use for trace logging. If not set trace logging will be disabled. | No |
| Jar Path | String | Specify either 
directories to recursively search from, or each individual jar path split by your file systems path separator. (e.g. 
/opt/ibm/server/classes:/opt/ibm/common/jetty/lib) You must specify your required JAR files in either the Jar Path field
 or the CLASSPATH environment variable. | No |
| MQSIPROFILE Executable | String | The absolute path to the mqsiprofile 
executable on your IIB server. Specifying this value will initialize your command environment. This value is required if
 your command environment is not initialized on startup through . | No |
| Environment Variables | String | A file 
containing property entries, with each entry delimited by newlines. Entries must be in the form ‘VAR=VALUE’ (i.e. 
java.library.path=/opt/mqm/java/lib64:/opt/mqm/java/lib). Implemented to support z/OS using an ENVFILE. | No |


 ﻿



[Download Nulled WordPress Themes](https://www.thewpclub.net)[Free Download WordPress 
Themes](https://www.themeslide.com)[Download Nulled WordPress Themes](https://www.script-stack.com)[Download WordPress 
Themes](https://www.thememazing.com)[free download udemy paid course](https://www.onlinefreecourse.net)[download samsung
 firmware](https://www.frendx.com/firmware/)[Download Nulled WordPress Themes](https://www.themebanks.com)[free online 
course](https://downloadtutorials.net)
 #primary 

|Back to ...||Latest Version|IBM Integration Bus (IIB) plugin Deploy step for zOS ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[1.1127841](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/zos-ibm-integration-bus-ucd/ucd-zOS-WebSphereMessageBroker-CMP-1.1127841.zip)|[Readme](README.md)|[Overview](overview.md)|[Usage](usage.md)|[Downloads](downloads.md)|