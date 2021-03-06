---
title: Configure the SAP Web IDE Destination for SAP Jam Collaboration on SAP Cloud Platform
description: Demonstrates how to configure the SAP Web IDE Destination for SAP Jam Collaboration on SAP Cloud Platform
primary_tag: products>sap-jam-collaboration
tags: [  tutorial>intermediate, products>sap-jam, products>sap-cloud-platform, topic>cloud ]
---

## Prerequisites  
 - **Proficiency:** Intermediate

## Next Steps
- Select a tutorial from the [Tutorial Navigator](http://www.sap.com/developer/tutorial-navigator.html) or the [Tutorial Catalog](http://www.sap.com/developer/tutorials.html)

## Details
### You will learn  
In this tutorial you will learn how to configure the Web IDE SAP Jam Collaboration Destination on SAP Cloud Platform.

To enable your Web IDE to recognize the SAP Jam Collaboration UI5 mobile components you will need to register a second destination on SAP Cloud Platform.

### Time to Complete
**15 Min**

---

[ACCORDION-BEGIN [Step 1: ](Create the destination configuration file on SAP Cloud Platform)]

1.  Create a file named `sapjam\_webide\_repo`
2.  Copy and paste the following into this file:
    ```
    Description=SAP Jam Plugins
    Type=HTTP
    TrustAll=true
    Authentication=NoAuthentication
    WebIDEUsage=plugin_repository
    Name=sapjam_webide_repo
    WebIDEEnabled=true
    CloudConnectorVersion=2
    URL=https:\//raw.githubusercontent.com/SAP/SAPJamSampleCode/master/hcp_samples/
    ProxyType=Internet  
    ```
3.  Save this file.
4.  If you configure the destination manually, all values must be the same including the name of the destination.


[ACCORDION-END]

[ACCORDION-BEGIN [Step 2: ](Import the destination configuration file into SAP Cloud Platform)]

1.  Login to the _Hana Cloud Server Cockpit_
2.  Select your account
3.  Click **Connectivity**
4.  Click **Destinations**
5.  Click **Import Destination**
6.  Select your destination configuration file `sapjam\_developer` and click **Open**.
7.  Click **Save**

![Import your destination configuration file into SAP Cloud Platform page](loio5ca95460e55c49978cf59cb4684996d8_HiRes.png)

Figure 1: Import your destination configuration file into SAP Cloud Platform


[ACCORDION-END]

---

## Next Steps
- Select a tutorial from the [Tutorial Navigator](http://www.sap.com/developer/tutorial-navigator.html) or the [Tutorial Catalog](http://www.sap.com/developer/tutorials.html)
