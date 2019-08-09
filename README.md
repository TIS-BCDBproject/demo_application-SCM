Pilot System for TIS Blockchain Development basis
==========================
[![image](https://github.com/TIS-BCDBproject/images/blob/master/example.jpg)](https://marketplace.r3.com/solutions/pilot-system-for-tis-blockchain-development-basis)

## Description
"Pilot System for TIS Blockchain Development basis" is an application development basis.

It has the following features.

1. It takes advantage of existing system assets and develops step by step. 
1. It develops gradually while measuring the introduction effect.

Historically, systems have been coordinated between systems by means of data linkage with EDI or through manual human processes. With this, the systems are consolidated on a blockchain. There is also a demonstration system that focus on SCM (supply chain management system) of trading companies and so on. Demonstration includes order, stock and shipment management system.

This system operates only on Windows OS.

## Prerequisite
- Owning the Corda Enterprise 3.2 jar files\[^1]
    You will need:
    - corda-3.2.jar
    - corda-webserver-3.2.jar
    - corda-tools-network-bootstrapper-3.2.jar
- Installation of JDK8

\[^1]:When you do not own those files, please make inquiries with R3.

## Installation
1. Download the "tsc.zip" and unzip it to any directory.
1. Copy "corda-tools-network-bootstrapper-3.2.jar" to "nodes" directory.
1. Rename "corda-3.2.jar" to "corda.jar", and copy it to "nodes" directory.
1. Execute "01_execute_bootstrapper.bat".
1. Rename "corda-webserver-3.2.jar" to "corda-webserver.jar" and copy it to "nodes" directory.
1. Execute "02_copy_corda_webserver.bat".
1. Copy the following files to "C:/home/"
    - properties\comment.properties
    - properties\customerWarehouse.properties
    - properties\message.properties
    - properties\productSupplier.properties
    - properties\supplierWarehouse.properties

## Usage
1. Start each corda nodes and webservers. 
    ``` {.sourceCode .dosbatch}
    > .\start.bat
    ```
   Please wait for a few minutes until all the nodes and web servers have complete to start.
1. Open a html file(in "web" directory) using web browsers.

## Licence
Proprietary

## Author
TIS Inc. (http://www.tis.com/)