---
author_name: René Jeglinsky
author_profile: https://github.com/renejeglinsky
description: This tutorial shows you how to deploy your SAP Cloud Application Programming Model (CAP) application to SAP Business Technology Platform (BTP), Cloud Foundry environment using SAP HANA Cloud service.
auto_validation: true
primary_tag: software-product-function>sap-cloud-application-programming-model
tags: [ tutorial>beginner, programming-tool>node-js, software-product>sap-business-technology-platform, software-product>sap-fiori, software-product>sap-hana-cloud, software-product-function>sap-cloud-application-programming-model ]
time: 30
parser: v2
---

# Deploy a CAP Business Service to SAP Business Technology Platform

## You will learn
  - How to deploy your CAP business service on SAP BTP and binding appropriate service instances. See the [Developer Guide for Cloud Foundry](https://docs.cloudfoundry.org/devguide/) for more details

## Prerequisites
- You've downloaded and installed the [cf command line client](https://github.com/cloudfoundry/cli#downloads) for Cloud Foundry as described in the tutorial [Install the Cloud Foundry Command Line Interface (CLI)](cp-cf-download-cli).
- You've finished the tutorial [Create a CAP Business Service with Node.js using Visual Studio Code](cp-apm-nodejs-create-service).
- If you don't have a Cloud Foundry Trial subaccount and dev space on [SAP BTP](https://cockpit.hanatrial.ondemand.com/cockpit/) yet, create your [Cloud Foundry Trial Account](hcp-create-trial-account) with **US East (VA) as region** and, if necessary [Manage Entitlements](cp-trial-entitlements).
- You've downloaded and installed the [cf command line client](https://github.com/cloudfoundry/cli#downloads) for Cloud Foundry as described in the tutorial [Install the Cloud Foundry Command Line Interface (CLI)](cp-cf-download-cli).
- You've downloaded and installed the [MBT Built Tool](https://sap.github.io/cloud-mta-build-tool/download/)
- You've downloaded and installed the [MultiApps CF CLI plugin](https://github.com/cloudfoundry/multiapps-cli-plugin/blob/master/README.md).
- You've to [Use an existing SAP HANA Cloud service instance](https://developers.sap.com/tutorials/btp-app-hana-cloud-setup.html#42a0e8d7-8593-48f1-9a0e-67ef7ee4df18) or [set up a new SAP HANA Cloud service instance](https://developers.sap.com/tutorials/btp-app-hana-cloud-setup.html#3b20e31c-e9eb-44f7-98ed-ceabfd9e586e) to deploy your CAP application


---

## Intro

It's now time to switch to SAP HANA as a database and prepare your project for an MTA deployment to SAP BTP Cloud Foundry. To continue with this tutorial you need to [Use an existing SAP HANA Cloud service instance](https://developers.sap.com/tutorials/btp-app-hana-cloud-setup.html#42a0e8d7-8593-48f1-9a0e-67ef7ee4df18) or [set up a new SAP HANA Cloud service instance](https://developers.sap.com/tutorials/btp-app-hana-cloud-setup.html#3b20e31c-e9eb-44f7-98ed-ceabfd9e586e) to deploy your CAP application.

> Your SAP HANA Cloud service instance will be automatically stopped overnight, according to the server region time zone. That means you need to restart your instance every day, before you start working with your trial.
