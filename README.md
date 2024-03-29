# SAS Viya 4 Resource Guide

## Overview

This guide describes a set of linked open-source projects that support the pre-installation, deployment, and subsequent monitoring and management of SAS Viya platform software.  

## Resources

### Planning for a SAS Viya Platform Deployment

The [SAS Viya Orders CLI](https://github.com/sassoftware/viya4-orders-cli) can be used to obtain required files that enable a deployment of the SAS Viya platform.

### Standing Up Compute Resources

The SAS Viya Infrastruture as Code repositories can be used to create the necessary compute resources for a SAS Viya platform deployment. The following cloud provider is supported at this time:
- [SAS Viya Infrastructure as Code - Azure](https://github.com/sassoftware/viya4-iac-azure)
- [SAS Viya Infrastructure as Code - AWS](https://github.com/sassoftware/viya4-iac-aws)
- [SAS Viya Infrastructure as Code - GCP](https://github.com/sassoftware/viya4-iac-gcp)
- [SAS Viya Infrastructure as Code - Open Source Kubernetes](https://github.com/sassoftware/viya4-iac-k8s)

Once compute infrastructure has been created, run the Pre-Installation Report application in the [SAS Viya Administration Resource Kit](https://github.com/sassoftware/viya4-ark). This application verifies whether sufficient compute resources and permissions are present to support a smooth deployment.

### Deploying the SAS Viya Platform

The documentation that you can access from [my.sas.com](https://my.sas.com) walks you through
the process for deploying your SAS Viya platform software.

When you are ready to deploy the SAS Viya platform, the [SAS Viya Deployment](https://github.com/sassoftware/viya4-deployment) project provides Ansible playbooks to automate the deployment.

When the deployment is complete, run the Deployment Report application from the [SAS Viya Administration Resource Kit](https://github.com/sassoftware/viya4-ark) to generate information about the deployment that can be easily shared.

### Monitoring the SAS Viya Platform

After deploying the SAS Viya platform, a key part of managing the system is monitoring. The SAS Viya platform provides an optional set of standard open-source tools to collect and display the collected metric data, to manage alerts that are triggered by metric values, and to collect and view log messages. You can use these tools or support monitoring and logging using your own tools. The [SAS Viya Monitoring for Kubernetes](https://github.com/sassoftware/viya4-monitoring-kubernetes) project provides the open source tools to support logging and monitoring.

### Update the SAS Viya Platform Software

A SAS software update replaces some or all of your deployed software with the latest versions of that software. The documentation that you can access from [my.sas.com](https://my.sas.com) walks you through the process of updating your SAS Viya platform software.

The [SAS Viya Orders CLI](https://github.com/sassoftware/viya4-orders-cli) tool enables you to 
automate a workflow that manages the life-cycle of the deploying and updating of SAS Viya platform software.

## Contributing

We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to submit contributions to these projects.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).

## Additional Resources

* [SAS Viya Platform Operations Guide](https://documentation.sas.com/?softwareId=mysas&softwareVersion=prod&docsetId=itopswlcm&docsetTarget=home.htm)
* [SAS Viya Administration Checklist](https://github.com/sassoftware/viya4-admin-checklist)
