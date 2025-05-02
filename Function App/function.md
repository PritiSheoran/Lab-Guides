# Create a Function App using Azure Portal


## Overview

Azure Functions is a serverless solution that allows you to write less code, maintain less infrastructure, and save on costs. Instead of worrying about deploying and maintaining servers, the cloud infrastructure provides all the up-to-date resources needed to keep your applications running.

## Task to be Done

1. Create a Function App
1. Create a Blob triggered function 


## Task 1 : Create a Function App

1. On **Azure Portal page** in search bar search for **Function App(1)** and select **Function App(2)**.

   ![Function App](Search.png)

2. On App Service page, click on **+Create(1)**, choose **Function App(2)** from the dropdown menu.

   ![+Create](Create.png)

3. Choose Hosting plan as **Consumption(1)** then click on **Select(2)**.

   ![Hosting Plan](Hosting.png)

4. In **Basics** tab, add the following information and click on **Review + Create(8)**

   | **Settings**                    | **Values**                                               |
   |---------------------------------|----------------------------------------------------------|
   | Subscription                    | Select **Innova8 Training (1)**                          |
   | Resource group                  | Select **priti.sheoran18 (2)** from dropdown menu        |
   | Function App Name               | Provide a unique name e.g **practice122 (3)**            |
   | Operating System                | Select **Linux(4)**                                      |
   | Runtime stack                   | Select **Python (5)**  from the dropdown                 |
   | Version                         | Select  **3.11 (6)** from the dropdown menu              |
   | Region                          | Select a nearby region e,g. **Central US**               |

   ![Basic](Basic.png)

6. Once the validation pass, click on **Create(1)**.

   ![Review+Create](Create1.png) 

7. Wait a few minutes while Azure sets up your Function App. Click on the **Go to resource(1)** option.

   ![AppS](Resource.png)
   
9. Navigate to **Storage Account** page, form the **Data Storage(1)** select **Container**.  
    
   ![AppS](Container.png)

10. On the container page, select ** + Container(1)** to create a new container.

    ![AppS](CC.png)

11. Create a **New Container** and click **Create(2)**.
    
    | **Settings**                    | **Values**                                               |
    |---------------------------------|----------------------------------------------------------|
    | Name                            |  **Provide a unique name (1)**                           |

    ![AppS](New.png)    
   
## Task 2: Create a Blob triggered function 

1. On the **Overview(1)**, click **Create function(2)**.

   ![AppS](Function.png)
   
3. On the Select a template tab of the **Create function**, click on the **Blob trigger(1)** option and then click on **Next(2)**.

   ![Function](Function1.png)
   
5. On the Template details tab and click on **Create(4)**.

   | **Settings**                    | **Values**                                                            |
   |---------------------------------|-----------------------------------------------------------------------|
   | Provide a function name         | Select **Default name or provide a unique name(1)**                   |
   | Path                            | Provide your container name **images(2)**                             |
   | Name                            | Select storage account name from New **pritisheoran18ab32 (3)**       |

   ![Function](Function3.png)
    
7. Navigate to Storage account, Upload an image inside you Container.

  ![Function](Upload.png)
  
9. On the BlobTrigger1 > Code + Test, review the auto-generated code and note that the code is designed to run an Blob request and log information.

 ![Function](Log.png)   

   



   

   
