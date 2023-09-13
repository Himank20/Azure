# Create a Virtual Machine using Azure Portal
#
#
This document describes the steps involved in provisioning a virtual machine using the Azure portal.


After we open the the Virtual Machines blade in Azure Portal, follow the mentioned steps: -
#
**Step 1** -> The first tab we get is the Basics tab which contains the general information about our VM. We start with selecting a Resource Group for our Virtual Machine or creating a new one.
**A Resource Group act as a container which holds all the related resources for a solution**
![](https://i.imgur.com/Vye9ZCr.png)
#
**Step 2** -> Next we will give a name for our virtual machine. Usually while naming an Azure resource we follow a naming covention which consists of **resourceType_environment_resource_instanceNumber**
![](https://i.imgur.com/csq2M5r.png)
#
**Step 3** -> Now we will select a region for our resource. This should be ideally close to where our users or customers are. Location can also be selected based on other factors like Data residency requirements, Compliance requirements or cost.
![](https://i.imgur.com/Yba7scW.png)
#
**Step 4** -> Next we will select availability options for our virtual machine. According to our needs we can select a suitable option. 
![](https://i.imgur.com/wMLkl1r.png)
#
**Step 5** -> Now we will select the base operating system or application for our virtual machine
![](https://i.imgur.com/l7XRHx8.png)
#
**Step 6** -> Next we select a VM size to support the workload that we want to run on our virtual machine. 
![](https://i.imgur.com/1rb4oVG.png)
#
**Step 7** -> Now we will select an authentication type for our VM. It can either be a password or SSH key. Here I have selected the password authentication and given a username and password for the machine
![](https://i.imgur.com/zynwQNQ.png)
#
**Step 8** -> After selecting the authenication type, we will configure public input ports to restrict the incomming traffic. For connecting remotely, we will keep the SSH (22) port open.
![](https://i.imgur.com/zynwQNQ.png)
#
**Step 9** -> In the Disk tab, we will select the Azure managed OS disk type according to our workload needs.
![](https://i.imgur.com/wcI5oZp.png)
#
**Step 10** -> In the same tab, we also have the option to attach a seperate Data Disk which is temporary disk to store files or create a new disk.
![](https://i.imgur.com/rtrbDgE.png)
#
**Step 11** -> Next in the Networking tab, we can define the network related aspects of out virtual machine like Virtual Network, Subnet, Public IP and other settings.
![](https://i.imgur.com/tcZmwYs.png)
While configuring the vnet and subnet settings, we can move forward with the pre populated settings or create a new virtual network by clicking on **Create New**. This will open a new tab as shown below
![](https://i.imgur.com/9RrFhOF.png)
#
**Step 12** -> Next in networking tab, we can define our load balancing options or these settings can also be defined later
![](https://i.imgur.com/fAPoDSD.png)
#
**Step 13** -> In the Management tab, we configure the management options for our virtual machine. Some of the notable settings to configure here are Login with Azure AD, Backup and Patch Orchestration settings
![](https://i.imgur.com/AZ89HgW.png)
#
**Step 14** -> In the Monitoring tab, we can configure the monitoring and diagnostic settings for the virtual machine
![](https://i.imgur.com/autMwwa.png)
#
**Step 15** -> In the Advanced tab, we can configure settings like Extensions, VM Applications, Custom data, Dedicated Host, etc.
![](https://i.imgur.com/Wd11qdq.png)
#
**Step 16** -> In the Tags tab, we can define tags for our resources. Tags are useful for categorizing our resources for billing purpose.
![](https://i.imgur.com/lwOjezQ.png)
#
**Step 17** -> Once all the settings are configured click on Review + Create. Azure will validate all the settings before provisioning our virtual machine. Once done, we can see a successful validation message as mentioned below and proceed to create the VM.
![](https://i.imgur.com/uia9iiN.png)


