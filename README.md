# Cisco Adaptive Security Virtual Appliance (ASAv)

## Security for virtual and hybrid cloud environments
The ASAv is a virtualized network security solution that provides policy enforcement 
and threat inspection across heterogeneous, multisite environments.

ASA firewall and VPN capabilities help safeguard traffic and multitenant architectures. Available in most hypervisor environments, 
the Cisco ASAv can be deployed exactly where it is needed to protect users and workloads on-premises or in the cloud.

## Supported Platforms

Most of the features that are supported on a physical ASA by Cisco software are supported on the virtual appliance as well, except for clustering and multiple contexts. The virtual appliance supports 
site-to-site VPN, remote-access VPN, and clientless VPN functionalities as supported by physical ASA devices.

The ASAv is supported on the following platforms:

* VMware ESXi  
* KVM  
* Hyper-V  
* AWS  
* Azure

## Support & Downloads  
All support information for Cisco Adaptive Security Virtual Appliance (ASAv)  

**Data Sheet**  
[Cisco Adaptive Security Virtual Appliance (ASAv) Data Sheet](https://www.cisco.com/c/en/us/products/collateral/security/adaptive-security-virtual-appliance-asav/datasheet-c78-733399.html?cachemode=refresh)

**Documentation**  
* Release Notes: [Go here](https://www.cisco.com/c/en/us/support/security/virtual-adaptive-security-appliance-firewall/products-release-notes-list.html).  
* Technical Documentation: [ASAv Getting Started Guide](https://www.cisco.com/c/en/us/support/security/virtual-adaptive-security-appliance-firewall/products-installation-guides-list.html)  
* White Papers: [Go here](https://www.cisco.com/c/en/us/products/security/virtual-adaptive-security-appliance-firewall/white-paper-listing.html)  

**Software**  
[Downloads Home](https://software.cisco.com/download/home/286119613/type)  

## Public Cloud Deployment  
### Azure  
The ASAv on Microsoft Azure supports the Standard D3 and Standard D3_v2 instances, which supports four vCPUs, 14 GB, and four interfaces.  

You can deploy the ASAv on Microsoft Azure in one of three ways:
* As a stand-alone firewall using the Azure Resource Manager
* As an integrated partner solution using the Azure Security Center
* As a high availability (HA) pair using the Azure Resource Manager

**Azure Resource Templates**  
You can deploy the ASAv using Azure Resource Manager templates. An Azure Resource Template is a JSON file. 
To simplify the deployment of all the required resources, you can use two JSON files:  
* **Template File** — This is the main resources file that deploys all the components within the resource group. 
* **Parameter File** — This file includes the parameters required to successfully deploy the ASAv. It includes details such 
as the subnet information, virtual machine tier and size, username and password for the ASAv, the name of the storage container, etc. 
You can customize this file for your Azure deployment environment.  

*Example: Azure Resource Manager JSON Template File*  
```
{
    "$schema": "http://schema.management.azure.com/schemas/2018-01-01/deploymentTemplate.json#",
    "contentVersion": "",
    "parameters": {  },
    "variables": {  },
    "resources": [  ],
    "outputs": {  }
}
```
**Documentation**  
* Templates and Examples: Included in this repository.
* Technical Documentation: [Deploy the ASAv On the Microsoft Azure Cloud](https://www.cisco.com/c/en/us/td/docs/security/asa/asa910/asav/quick-start-book/asav-910-qsg/asav_azure.html)

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com)  
___

### AWS  
The ASAv runs as a guest in the AWS environment of the Xen Hypervisor. ASAv on AWS supports the following instance types:  
* **c3.large, c4.large, m4.large** — 2 vCPUs, 3.75 GB, 3 interfaces (1 management interface, 2 data interfaces)
**Note:** Both the ASAv10 and ASAv30 are supported on the c3.large instance. However, we do not recommend deploying the 
ASAv30 on any large instances due to resource under-provisioning.  
* **c3.xlarge, c4.xlarge, m4.xlarge** — 4 vCPUs, 7.5 GB, 4 interfaces (1 management interface, 3 data interfaces)
**Note:** Only the ASAv30 is supported on xlarge instances.  

You create an account on AWS, set up the ASAv using the AWS Wizard, and chose an Amazon Machine Image (AMI). 
The AMI is a template that contains the software configuration needed to launch your instance.  
**Note:** The AMI images are not available for download outside of the AWS environment.  

**Documentation**  
* Technical Documentation: [Deploy the ASAv On the AWS Cloud](https://www.cisco.com/c/en/us/td/docs/security/asa/asa910/asav/quick-start-book/asav-910-qsg/asav_aws.html)

[<img src="https://a0.awsstatic.com/libra-css/images/logos/aws_logo_smile_179x109.png"/>](https://aws.amazon.com/)  
___ 
# ASAv templates and artifacts  

#### TBD

