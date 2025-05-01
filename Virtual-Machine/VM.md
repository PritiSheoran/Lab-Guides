
# Create a Virtual Machine using Azure Portal


## Overview

An Azure virtual machine (VM) is a computing resource provided by Microsoft Azure. It allows users to create and use virtualized computing instances in the cloud. Azure Virtual Machines enable users to run applications, host websites, and perform various computing tasks without needing to purchase and maintain physical hardware.


## Task to be Done

1. Create a Virtual Machine
1. Connect to Virtual Machine


## Task 1 : Create a Virtual Machine

- Go to **Azure Portal** in search bar search for **Virtual Machine(1)** and select **Virtual Machine(2)**.

  ![VMSearch](Search.png)

- Click on **+Create (1)**, choose **Azure Virtual Machine (2)**.
 
  ![VMSearch](Create.png)

- In **Basics** tab, add the following information and click on **Next: Disks > (14)**


  | **Settings**                     | **Values**                                               |
  |----------------------------------|----------------------------------------------------------|
  | Subscription                    | **Accept default subscription (1)**                       |
  | Resource group                  | **priti (2)**                                             |


  ![Basics Tab](Basic1.png)

  | **Settings**                    | **Values**                                                |
  |---------------------------------|-----------------------------------------------------------|
  | Virtual machine name            | **MD-VM (3)**                                             |
  | Region                          | **West US 2 (4)**                                         |
  | Availability options            | **No infrastructure redundancy required (5)**             |
  | Security Type                   | **Standard (6)**                                          |
  | Image                           | **Windows Server 2019 Datacenter - x64 Gen2 (7)**         |

  ![Basics Tab](Basic2.png)

  | **Settings**                    | **Values**                                                |
  |---------------------------------|-----------------------------------------------------------|
  | Size                            | **Standard B2s (8)**                                      |
  | Username                        | **priti (9)**                                             |
  | Password                        | **March@123456 (10)**                                     |
  | Co nfirm Password                | **March@123456 (11)**                                    |
 
  ![Basics Tab](Basic3.png)

  | **Settings**                    | **Values**                                                |
  |---------------------------------|-----------------------------------------------------------|
  | Public inbound ports            | **Allow selected ports (12)**                             |
  | Select inbound ports            | **RDP(3389) (13)**                                        |

  ![Basics Tab](Basic4.png)
  

- In **Disk** Tab, choose the following values and click **next: Networking (4)**

  | **Settings**                     | **Values**                                                |
  |----------------------------------|-----------------------------------------------------------|
  | OS disk size                     | **Image default (127 GiB) (1)**                           |
  | OS disk type                     | **Standard SSD (locally-redundant storage) (2)**          |
  | Key management                   | **Platform managed key  (3)**                             |


  ![Disk](OSDisk.png)


- In **Networking** tab, check the following values, leave everything as default and click **Next: Management (4)**

  | **Settings**                                     | **Values**                                         |
  |--------------------------------------------------|----------------------------------------------------|
  | Public inbound ports                             | **Allow selected ports (1)**                       |
  | Select inbound ports                             | **RDP(3389) (2)**                                  |
  | Delete public IP and NIC when VM is deleted      | **Enable (3)**                                     |

  ![Networking](Networking.png)

- Click on the **Review + create** at the buttom of the page. 
- Click **Create (1)** to start the deployment.

  ![Review + Create](Review+Create.png)


- Wait a few minutes while Azure sets up your Virtual Machine. Click on the **Go to resource (1)** option.

  ![Deployment Progress](Deploymnet.png)


## Task 2: Connect to Virtual Machine

Once deployed:

- Now, you will be redirected to the newly created virtual machine's page. Click **Connect (1)** and choose **Connect (2)**

  ![Connect](Connect.png)

- Click **Connect > RDP** and **download the RDP file (1)** and open it.

  ![RDP](RDP.png)

- **Open the downloaded RDP file** and click **Connect (1)** when prompted.

  ![RDP](Prompt.png) 

- Select **More choices (1)** option, choose **Use a different account (2)** enter your credentials Username: **.\priti (3)** and password: **March@123456 (4)**. 
- Click **ok(6)** you should be able to connect to VM successfully.

  ![RDP](Credentials.png)
