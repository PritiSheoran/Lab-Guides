
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

3. In **Basics** tab, add the following information and click on **Next: Database > (9)**

   | **Settings**                    | **Values**                                               |
   |---------------------------------|----------------------------------------------------------|
   | Subscription                    | **Accept default subscription (1)**                      |
   | Resource group                  | **webapp (2)**                                           |
   | Name                            | **DockerApp (3)**                                        |
   | Publish                         | **Enable Container (4)**                                 |
   | Operating System                | **Linux (5)**                                            |
   | Region                          | **West US 2 (6)**                                        |


   ![Basics Tab](Basic.png)

   | **Settings**                    | **Values**                                                |
   |---------------------------------|-----------------------------------------------------------|
   | Linux Plan(West US 2)           | **(New) ASP-webapp-8312 (7)**                             |
   | Pricing Plan                    | **Basic B1(100 total ACU, 1.75 GB memory, 1 vCPU) (8)**   |

   ![Basics2 Tab](Basic2.png)

4. On the **Database** tab, leave everything as default, and click on **Next: Container>**.

5. On the **Next: Container>** tab, add the following information and click on **Review + Create (5)**

   | **Settings**                    | **Values**                                               |
   |---------------------------------|----------------------------------------------------------|
   | Image Source                    | **Other container registries (1)**                       |
   | Access Type                     | **Public (2)**                                           |
   | Registry server URL             | **Keep it as default (3)**                               |
   | Image and tag                   | **23mcc20042/fastbite (4)**                              |

   ![Container Tab](Database.png)

6. Once the validation pass, click on **Create (1)**.
   
   ![Review+Create](Review+Create.png) 
   
7. Wait a few minutes while Azure sets up your Web App. Click on the **Go to resource (1)** option.

   ![GoToResource](GoToResource.png)

## Task 2: Test the Web App

 1.  Now, you will be redirected to the newly created web app's page, Copy the **default domain** URL 

     ![Domain](Domain.png)  

 2.  Copy the URL and paste it into a new browser tab to observe the Web page.

     ![output](output.png) 
   
   
   
