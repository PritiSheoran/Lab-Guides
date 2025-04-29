
# Create a Web App using Azure Portal 


## Overview

Azure App Service is a fully managed web application hosting platform. This platform as a service (PaaS) is offered by Azure. Azure App Service is actually a collection of four services, all of which are built to help you host and run web applications. Web Apps are the most commonly used of the four services. 
In this task, we will create a new web app that runs a Docker container.


## Task to be Done

1. Create a Web App
1. Test the Web App


## Task 1 : Create a Web App

1. Go to **Azure Portal** in search bar search for **App Service (1)** and select **App Service (2)**.

   ![AppService](Search.png)

2. Click on **+Create(1)**, choose **Web App(2)**.

   ![Create](Create.png) 

3. In **Basics** tab, add the following information and click on **Next: Disks > (14)**

   | **Settings**                     | **Values**                                               |
   |----------------------------------|----------------------------------------------------------|
   | Subscription                     | **Accept default subscription (1)**                      |
   | Resource group                   | **priti (2)**                                            |


   ![Basics Tab](Basic1.png)

   | **Settings**                    | **Values**                                                |
   |---------------------------------|-----------------------------------------------------------|
   | Virtual machine name            | **MD-VM (3)**                                             |
   | Region                          | **West US 2 (4)**                                         |
   | Availability options            | **No infrastructure redundancy required (5)**             |
   | Security Type                   | **Standard (6)**                                          |
   | Image                           | **Windows Server 2019 Datacenter - x64 Gen2 (7)**         |
