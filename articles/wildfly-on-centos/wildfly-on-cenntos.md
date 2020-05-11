---
title: Quickstart - WildFly on CentOS
description: Deploy a standalone node of WildFly on CentOS VM
author: SpektraSystems
ms.author: karler
ms.topic: quickstart
ms.date: 05/11/2020
---

# Quickstart: WildFly on CentOS

This quickstart shows you how to deploy a standalone node of WildFly 18.0.1.Final on top of CentOS 8.0 VM. It also deploys Java Sample Application named JBoss-EAP on Azure on Wildfly. This is ideal for development and testing of enterprise Java applications on Azure. 

## Prerequisites

* Azure Subscription with specified payment method (CentOS-Based 8.0 is an [Azure Marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/openlogic.centos?tab=Overview) product and requires a payment method to be specified in the Azure Subscription). Azure CentOS 8 image is a Pay-as-you-go (PAYG) VM image and does not require the user to license. The VM will be licensed automatically after the instance is launched for the first time and user will be charged hourly in addition to Microsoft's Linux VM rates.  Click [here](https://azure.microsoft.com/en-us/pricing/details/virtual-machines/linux/#linux) for pricing details. WildFly is free to download and use and does not require a Red Hat Subscription or any License, for more details click [here](https://www.wildfly.org/).
* To create the CentOS VM, you will need:

    - **Admin Username** and password/ssh key data which is an SSH RSA public key for your VM.

    - **WildFly Username** and password to enable the WildFly Admin Console and Deployment method.

## Use case


## Configuration choice


## Support and subscription notes

Azure CentOS 8 image is a Pay-as-you-go (PAYG) VM image and does not require the user to license. The VM will be licensed automatically after the instance is launched for the first time and user will be charged hourly in addition to Microsoft's Linux VM rates.  Click [here](https://azure.microsoft.com/en-us/pricing/details/virtual-machines/linux/#linux) for pricing details. WildFly is free to download and use and does not require a Red Hat Subscription or any License, for more details click [here](https://www.wildfly.org/).

## How to consume


## ARM template

<a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/wildfly-standalone-centos8" target="_blank"> [WildFly 18 on CentOS 8 (stand-alone VM)]</a> - This Azure quickstart template deploys a web application named JBoss-EAP on Azure on WildFly 18.0.1.Final running on CentOS 8 VM.

## Resource Links:

This template creates all the Azure compute resources to run WildFly 18.0.1.Final on top of CentOS 8.0 VM. The following resources are created by this template:

- CentOS 8 VM 
- Public IP 
- Virtual Network 
- Network Security Group 
- WildFly 18.0.1.Final
- Sample Java application named JBoss-EAP on Azure deployed on WildFly

## Next steps

- Once you deploy the template successfully, go to the outputs section of the deployment to obtain the VM DNS name, App URL and the Admin Console URL.

- Paste the App URL that you copied from the output page in a browser to view the JBoss-EAP on Azure web page.

- Paste the Admin Console URL that you copied from the output page in a browser to access the WildFly Admin Console and enter the Wildfly Username and password to login.

If you're interested in Red Hat JBoss EAP Azure Quickstart templates, you can find it here:

*  <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-standalone-rhel7" target="_blank"> [JBoss EAP 7.2 on RHEL 7.7 (stand-alone VM)]</a> - Standalone JBoss EAP 7.2 with a sample web app on a RHEL 7.7 Azure VM.

*  <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-standalone-rhel8" target="_blank"> [JBoss EAP 7.2 on RHEL 8.0 (stand-alone VM)]</a> - Standalone JBoss EAP 7.2 with a sample web app on a RHEL 8.0 Azure VM.

*  <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss7.3-eap-standalone-rhel8" target="_blank"> [JBoss EAP 7.3 on RHEL 8.0 (stand-alone VM)]</a> - Standalone JBoss EAP 7.3 with a sample web app on a RHEL 8.0 Azure VM.
