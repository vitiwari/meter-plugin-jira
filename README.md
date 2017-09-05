TrueSight Pulse Jira Integration Plugin
=========================================

Collects tickets(Jira Core, Jira Software and Jiar Service desk) from jira servers and collected tickets are sent to Truesight Intelligence as Events. 
The plugin allows multiple Jira instances data to be collected with independent polling interval.

### Prerequisites

#### Supported OS

|     OS    | Linux | Windows | OS X |
|:----------|:-----:|:-------:|:----:|
| Supported |   v   |    v    |  v   |

#### Runtime Environment

|  Runtime | node.js | Python | Java |
|:---------|:-------:|:------:|:----:|
| Required |         |        |    v*  |
\* java 1.8+ 

* [How to install java?](https://www3.ntu.edu.sg/home/ehchua/programming/howto/JDK_Howto.html)

#### TrueSight Pulse Meter versions v4.7.0-852 or later

- To install new meter go to Settings->Installation or [see instructions](https://help.boundary.com/hc/en-us/sections/200634331-Installation).
- To upgrade the meter to the latest version - [see instructions](https://help.boundary.com/hc/en-us/articles/201573102-Upgrading-the-Boundary-Meter).

#### Ingesting historical Jira data
If you want to import historical Jira data into TrueSight Intelligence, it is recommended that you ingest the historical data before configuring the plugin for data collection. For more information, see [Jira bulk ingestion on GitHub](https://github.com/boundary/jira-tsi-bulkingestion-script).

#### Plugin Configuration Fields

|Field Name        |Description                                                                    |
|:-----------------|:------------------------------------------------------------------------------|
|Application Name  |The TrueSight Intelligence App using which the events will be tagged. If the App does not exist, a new App is created                                            		   	   									 |
|Jira Server Name  |The host of Jira server                                            		   	   |
|Port              |The port of Jira server                                            		       |
|Username          |The user of Jira server                                            		       |
|Password          |The password of Jira server                                        		       |
|Poll Interval     |How often (in minutes) to poll for collecting the tickets                      |
|Field Mapping     |Type of fields will be collected(more info please check in template section)   |
|protocolType      |Type of protocals(https or http) 											   |
|Source	           |The jira instance name														   | 



### Templates
 1. [Jira Default Template](https://github.com/boundary/meter-plugin-jira/blob/master/template/jiraDefaultTemplate.json)


### References
[Jira Plugin Documentation](https://docs.bmc.com/docs/display/bti10/jira+Plugin)

