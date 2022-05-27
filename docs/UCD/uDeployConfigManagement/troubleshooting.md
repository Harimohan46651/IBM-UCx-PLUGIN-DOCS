
IBM UrbanCode Deploy Configuration Management - Troubleshooting
===============================================================

# Troubleshooting



### Troubleshooting




 


When using the Batch Import Properties step, you must include the component name in the 
properties file, as shown in the following example code:



```
ComponentName=Component A
name=myName
state=myState

```


If you do not include the component name in the properties file, the following error message is displayed:



```

Error Updating Properties!
java.io.IOException: 404 Not Found
No component for null

```



|Back to ...||Latest Version|IBM UrbanCode Deploy Configuration Management ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[17.1132359]()|[Readme](README.md)|[Overview](overview.md)|[Steps](steps.md)|[Downloads](downloads.md)|