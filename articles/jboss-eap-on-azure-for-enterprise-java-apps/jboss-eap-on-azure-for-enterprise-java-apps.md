---
title: Quickstart - JBoss EAP on Azure for enterprise Java apps
description: Deploy JBoss EAP on Azure on Red Hat Enterprise Linux for enterprise Java apps
author: SpektraSystems
ms.author: karler
ms.topic: quickstart
ms.date: 05/11/2020
---

# Quickstart: JBoss EAP on Azure for enterprise Java apps

This quickstart shows you how to deploy JBoss EAP on top of Red Hat Enterprise Linux. It also deploys Java Sample Application on EAP.

JBoss EAP (Enterprise Application Platform) is an open source platform for highly transactional, web-scale Java applications. EAP combines the familiar and popular Jakarta EE specifications with the latest technologies, like Microprofile, to modernize your applications from traditional Java EE into the new world of DevOps, cloud, containers, and microservices. EAP includes everything needed to build, run, deploy, and manage enterprise Java applications in a variety of environments, including on-premise, virtual environments, and in private, public, and hybrid clouds. To learn more about the JBoss Enterprise Application Platform, visit:
https://access.redhat.com/documentation/en-us/red_hat_jboss_enterprise_application_platform/

Red Hat Subscription Management (RHSM) is a customer-driven, end-to-end solution that provides tools for subscription status and management and integrates with Red Hat's system management tools. To obtain an rhsm account for JBoss EAP, go to: www.redhat.com.

## Prerequisites

* Azure Subscription with the specified payment method (RHEL 7.7/8.0 is an [Azure Marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps?filters=partners%3Blinux&page=1&search=Red%20Hat%20Enterprise%20Linux) product and requires a payment method to be specified in the Azure Subscription). If you have a RHEL OS license of your own and wish to use that, then you can also deploy a RHEL VM of BYOS license type.
* To create the CentOS VM, you will need:

    - **Admin Username** and password/ssh key data which is an SSH RSA public key for your RHEL VM.

    - **EAP Username** and password to enable the EAP Admin Console and Deployment method.
    
## Use case


## Configuration choice

For deployment of RHEL VM you can either choose the VM from the Azure Marketplace or if you have a RHEL OS license of your own and wish to use that, then you can also deploy a RHEL VM of BYOS license type and use your license to register for RHEL OS.

## Support and subscription notes

If you do not have RHEL OS license of you own, you will have to use RHEL PAYG (Pay-As-You-Go) marketplace image for deployment. RHEL Pay-As-You-Go image carries a separate hourly charge that is in addition to Microsoft's Linux VM rates. In this case the VM will be licensed automatically after the instance is launched for the first time and total price of the VM consists of the base Linux VM price plus RHEL VM image surcharge. See [Red Hat Enterprise Linux pricing](https://azure.microsoft.com/en-us/pricing/details/virtual-machines/red-hat/) for details. You also need to have a Red Hat account to register to Red Hat Subscription Manager (RHSM) and install JBoss EAP.

If you have a RHEL OS license and wish to deploy the VM using BYOS (Bring-Your-Own-Subscription) plan. Here your Red Hat Subscription Management (RHSM) account must have both Red Hat Enterprise Linux entitlement (for subscribing the RHEL OS for the VM) and EAP entitlement. To provision the RHEL-BYOS VM in your subscription, you will have to enable it in the Cloud Access from Red Hat portal and activate Red Hat Gold Images for your subscription. You can enable subscription for cloud access by following the instructions mentioned [here](https://access.redhat.com/documentation/en-us/red_hat_subscription_management/1/html/red_hat_cloud_access_reference_guide/con-enable-subs) and activate the Red Hat Gold Images by following the instructions mentioned [here](https://access.redhat.com/documentation/en-us/red_hat_subscription_management/1/html/red_hat_cloud_access_reference_guide/using_red_hat_gold_images#con-azure-access). Once your Azure subscription is enabled, please follow this [link](https://docs.microsoft.com/en-us/azure/virtual-machines/workloads/redhat/byos) to accept the Marketplace terms for RHEL-BYOS image from your Azure subscription.

Note that in both the cases your RHSM account needs EAP entitlement to use the Enterprise Application Platform. You can get an evaluation account for EAP from [here](https://access.redhat.com/products/red-hat-jboss-enterprise-application-platform/evaluation).

Click [here](https://access.redhat.com/products/red-hat-subscription-management) to know more about RHSM.

## How to consume


## ARM template

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-standalone-rhel7" target="_blank"> [JBoss EAP 7.2 on RHEL 7.7 (stand-alone VM)]</a> - This Azure template deploys a web application named JBoss-EAP on Azure on JBoss EAP 7.2 running on RHEL 7.7 VM.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-standalone-rhel8" target="_blank"> [JBoss EAP 7.2 on RHEL 8.0 (stand-alone VM)]</a> - This Azure template deploys a web application named JBoss-EAP on Azure on JBoss EAP 7.2 running on RHEL 8.0 VM.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss7.3-eap-standalone-rhel8" target="_blank"> [JBoss EAP 7.3 on RHEL 8.0 (stand-alone VM)]</a> - This Azure template deploys a web application named JBoss-EAP on Azure on JBoss EAP 7.3 running on RHEL 8.0 VM.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-multinode-singlevm-rhel7" target="_blank"> [JBoss EAP 7.2 on RHEL 7.7 (multi-node, single VM)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 running on multinode of RHEL 7.7 VM.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-multinode-singlevm-rhel8" target="_blank">[JBoss EAP 7.2 on RHEL 8.0 (multi-node, single VM)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 running on multinode of RHEL 8.0 VM.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-clustered-multivm-rhel7" target="_blank">[JBoss EAP 7.2 on RHEL 7.7 (clustered, multi-VM)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 cluster running on 'n' number RHEL 7.7 VMs where n is decided by the user and all the VMs are added to the backend pool of a Load Balancer.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-clustered-multivm-rhel8" target="_blank">[JBoss EAP 7.2 on RHEL 8.0 (clustered, multi-VM)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 cluster running on 'n' number of RHEL 8.0 VMs where n is decided by the user and all the VMs are added to the backend pool of a Load Balancer.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap7.3-clustered-multivm-rhel8" target="_blank"> [JBoss EAP 7.3 on RHEL 8.0 (clustered, multi-VM)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.3 cluster running on 'n' number of RHEL 8.0 VMs where n is decided by the user and all the VMs are added to the backend pool of a Load Balancer.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-clustered-vmss-rhel7" target="_blank"> [JBoss EAP 7.2 on RHEL 7.7 (clustered, VMSS)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 cluster running on RHEL 7.7 VMSS instances.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap-clustered-vmss-rhel8" target="_blank">[JBoss EAP 7.2 on RHEL 8.0 (clustered, VMSS)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.2 cluster running on RHEL 8.0 VMSS instances.

* <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/jboss-eap7.3-clustered-vmss-rhel8" target="_blank">[JBoss EAP 7.3 on RHEL 8.0 (clustered, VMSS)]</a> - This Azure template deploys a web application called eap-session-replication on JBoss EAP 7.3 cluster running on RHEL 8.0 VMSS instances.

## Resource Links:


## Next steps

If you don't have a Red Hat subscription to install a JBoss EAP, you can go through WildFly instead of JBoss EAP:

*  <a href="https://github.com/SpektraSystems/redhat-mw-cloud-quickstart/tree/master/wildfly-standalone-centos8" target="_blank"> [WildFly 18 on CentOS 8 (stand-alone VM)]</a> - Standalone WildFly 18 with a sample web app on a CentOs 8 Azure VM.
