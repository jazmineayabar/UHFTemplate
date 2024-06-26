# M2UHF Template app

This app shows how to use the ACD M2UHF API.  
it is intended to help with the development of a new app, please do not use this as a base for a new app.   

- In the MainActivity, the module is initialized and can be powered on or off.  
  After it is powered on, the reader can be initialized. If this was successful, 
  the following 2 Activities can be started:  

- ScanActivity: Start a tag inventory, the reader will scan all tags in range until the inventory is stopped  

- WriteActivity: The reader scans all tags in range and selects one tag.  
  On this tag, a write operation on the EPC memory bank can be started.   
  If the write operation was successful, all tags in range will be scanned again.  

## Notes
- **This app is just a simple demo without any warranties**    
- **Only for developers, do not use this app for customers**
- No extensive tests were made, so this app might crash in some cases...  
- **Please refer to the ACD M2UHF API documentation for more information and details**
- To set the Java/JDK version in Android Studio, go to Settings->Build,Execution,...->Build Tools->Gradle:  
  Download and Select in `Gradle JDK` the `openjdk-16` package

## Project specifications

|   |   |
|---|---|
|IDE                              |Android Studio Chipmunk 2021.2.1 Patch 2|
|Host OS                          |Ubuntu 20.04.4 LTS|
|Java/JDK version                 |15|
|Gradle version                   |7.2.2|
|Target API version               |32|
|Minimum API version              |28|
|Project version control          |Git/GitLab|
|Additional information           |This app uses the ACD M2UHF API|
