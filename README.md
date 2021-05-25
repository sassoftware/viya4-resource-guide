# SAS Viya 4 Resource Guide

## Overview

This guide describes a set of linked open-source projects that support the pre-installation, deployment, and subsequent monitoring and management of SAS Viya software.  

## Resources

### Planning for a SAS Viya Deployment

The [SAS Viya Orders CLI](https://github.com/sassoftware/viya4-orders-cli) can be used to obtain required files that enable a deployment of SAS Viya.

### Standing Up Compute Resources

The SAS Viya Infrastruture as Code repositories can be used to create the necessary compute resources for a SAS Viya deployment. The following cloud provider is supported at this time:
- [SAS Viya Infrastructure as Code - Azure](https://github.com/sassoftware/viya4-iac-azure)
- [SAS Viya Infrastructure as Code - AWS](https://github.com/sassoftware/viya4-iac-aws)
- [SAS Viya Infrastructure as Code - Google Cloud Platform (GCP)](https://github.com/sassoftware/viya4-iac-gcp)

Once compute infrastructure has been created, run the Pre-Installation Report application in the [SAS Viya Administration Resource Kit](https://github.com/sassoftware/viya4-ark). This application verifies whether sufficient compute resources and permissions are present to support a smooth deployment.

### Deploying SAS Viya

The documentation that you can access from [my.sas.com](https://my.sas.com) walks you through
the process for deploying your SAS Viya software.

When you are ready to deploy SAS Viya, the [SAS Viya Deployment](https://github.com/sassoftware/viya4-deployment) project provides Ansible playbooks to automate the deployment.

Once the deployment is complete, run the Deployment Report application from the [SAS Viya Administration Resource Kit](https://github.com/sassoftware/viya4-ark) to generate information about the deployment that can be easily shared.

### Monitoring SAS Viya

After deploying SAS Viya, a key part of managing the system is monitoring. SAS Viya provides an optional set of standard open-source tools to collect and display the collected metric data, to manage alerts that are triggered by metric values, and to collect and view log messages. You can use these tools or support monitoring and logging using your own tools. The [SAS Viya Monitoring for Kubernetes](https://github.com/sassoftware/viya4-monitoring-kubernetes) project provides the open source tools to support logging and monitoring.

### Update SAS Viya software

A SAS software update replaces some or all of your deployed software with the latest versions of that software. The documentation that you can access from [my.sas.com](https://my.sas.com) walks you through the process of updating your SAS Viya software.

The [SAS Viya Orders CLI](https://github.com/sassoftware/viya4-orders-cli) tool enables you to 
automate a workflow that manages the life-cycle of the deploying and updating of SAS Viya software.

## Contributing

We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to submit contributions to these projects.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).

## Additional Resources

* [SAS Viya Operations Guide](https://documentation.sas.com/?softwareId=mysas&softwareVersion=prod&docsetId=itopswlcm&docsetTarget=home.htm)
