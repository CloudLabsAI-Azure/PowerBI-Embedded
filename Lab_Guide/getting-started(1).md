# Power BI Embedded Hands On Lab

### Overall Estimated Duration: 4 hours

## Overview

Power BI Embedded enables you to seamlessly integrate interactive Power BI reports and dashboards into your applications, providing rich data visualization experiences for your users. With capabilities to create, embed, and customize Power BI content, this service helps organizations enhance decision-making processes and deliver actionable insights. By leveraging Power BI Embedded, you can enable scalable, secure, and cost-effective analytics solutions tailored to your business needs, fostering innovation and improving operational efficiency.

## Objective

This lab is designed to equip participants with hands-on experience in leveraging Power BI Embedded to integrate and customize data visualizations within applications, providing scalable and interactive reporting solutions.

- **Power BI Embedded Workshop Guide:** Implement Power BI Embedded to embed reports and dashboards into custom applications. Configure access and manage authentication for seamless integration.

## Prerequisites

Participants should have the following prerequisites:

- **Basic Understanding of Power BI**: Familiarity with Power BI concepts, including creating reports and dashboards.
- **Experience with Azure Portal**: Ability to navigate and manage Azure resources via the Azure Portal.
- **Knowledge of Power BI Service**: Understanding of how to publish and manage Power BI reports in the Power BI Service.
- **Basic Programming Knowledge**: Familiarity with programming or scripting languages (such as JavaScript or C#) to interact with Power BI Embedded APIs for embedding reports into applications.
- **Familiarity with APIs**: Understanding of how to use REST APIs for embedding Power BI content into applications.

## Architechture

The architecture for integrating **Power BI Embedded** into applications involves using the **Power BI Embedded** service, which allows embedding **Power BI** reports and dashboards within your application. The reports are created and stored in the **Power BI service**, and authentication is managed via **Azure Active Directory (Azure AD)** to ensure secure access. A client application communicates with **Power BI** using the **Power BI REST API** to embed reports and handle user interactions. The application displays these reports seamlessly, enabling users to explore and interact with the embedded data. This architecture leverages **Azure's cloud capabilities** to deliver scalable, interactive data visualizations within custom applications.

## Architechture Diagram

![](./media/arch01.JPG)

## Explanation of Components

The architecture for this lab involves several key components:

- **Power BI Embedded Service**: Allows the integration of Power BI reports and dashboards into custom applications, enabling users to view interactive reports directly within the app.
- **Power BI Reports and Dashboards**: The visualizations and data insights created in Power BI that can be embedded into external applications.
- **Azure Active Directory (AAD)**: Provides identity and access management, ensuring secure authentication and authorization for Power BI Embedded users.
- **Power BI REST API**: A set of web services that allows developers to interact with Power BI resources, enabling the embedding of reports, management of user access, and more.
- **Power BI Workspace**: A container within Power BI for organizing and managing reports and datasets, which can be shared or embedded into other applications.


## Getting Started with Lab

Welcome to your Power BI Embedded Hands-On Lab! This lab is designed to give you practical experience with embedding Power BI reports and dashboards into your applications. Let's get started and explore how you can integrate Power BI into your solutions.

## Accessing Your Lab Environment
 
Once you're ready to dive in, your virtual machine and lab guide will be right at your fingertips within your web browser.

   ![](./media/emb1.png)
 
## Virtual Machine & Lab Guide

Your virtual machine is your workhorse throughout the workshop. The lab guide is your roadmap to success.

## Exploring Your Lab Resources
 
To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab. Here, you will find the Azure credentials. Click on the **Environment** option to verify the credentials.
 
   ![](./media/emb2.png)
 
## Utilizing the Split Window Feature
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Top right corner.
 
   ![](./media/emb3.png)

## Managing Your Virtual Machine
 
Feel free to **start, stop**, or **restart** your virtual machine as needed from the **Resources** tab. Your experience is in your hands!

   ![](./media/new-get-start-25-4.png)

## Lab Guide Zoom In/Zoom Out
 
To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment.

   ![](./media/new-get-start-25-6.png) 

## Let's Get Started with Power BI Portal
 
1. On the Lab VM, open **Microsoft Edge** from the desktop. In a new tab, navigate to **Microsoft Fabric** by copying and pasting the following URL into the address bar:

   ```
   https://app.powerbi.com/
   ```

2. On the **Enter your email, we'll check if you need to create a new account** tab, you will see the login screen, in that enter the following email/username, and click on **Submit**.
 
   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>
 
      ![](media/pbi39u.png)

3. Now enter the following password and click on **Sign in**.
 
   - **Password:** <inject key="AzureAdUserPassword"></inject>
 
      ![](media/pbi33u.png)
     
1. If you see the pop-up **Stay Signed in?**, select **No**.

   ![02](../Images/12062025(3).png)

1. You should be able to view the Power BI Portal.

   ![image](https://github.com/user-attachments/assets/c70e25c2-4172-4818-b393-c479bf24595a)

1. From the side blade, click on **Workspaces (1)** and select **hacker<inject key="DeploymentID" enableCopy="false" />** **(2)** which is pre-created for the lab.

   ![](media/pbi40.jpg)

1. You'll be able to visualize the **Wingtip Sales Analysis** report uploaded in the workspace.

   ![](media/updated-reportsu.png)

1. From Power BI home page, Click on the **Settings (1)** icon at the top and select **Admin portal (2)** button.

   ![](media/Mod1S6.png)

1. Scroll down to Developer settings, if not enabled then **Enable (1)** the **Service principals can use Fabric APIs**. Under Apply to option, select the **Specific security groups (2)** button, search and select **PowerbiSDP (3)** group. Finally, click on **Apply (4)**. 

      ![](media/Mod1S7.png)

      >**Note** : Please proceed if the **PowerbiSDP** security group is already applied.
 
      >**Note** : You can also use the **Filter by keyword** search box at the top right of the page to search for Service principals can use Fabric APIs.

1. Scroll down to Admin API settings, if not enabled then **Enable (1)** the **Service principals can access read-only Admin APIs**. Under Apply to option, select the **Specific security groups (2)** button, search and select **PowerbiSDP (3)** group. Finally, click on **Apply (4)**.    

      ![](media/Mod1S8.png)   

      >**Note** : Please proceed if the **PowerbiSDP** security group is already applied.

      >**Note** : You can also use the **Filter by keyword** search box at the top right of the page to search for Service principals can access read-only Admin APIs.

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

Now, click on **Next >>** from the lower right corner to move on to the next page.
   
   ![](./media/GS4.png)

## Happy Learning!!