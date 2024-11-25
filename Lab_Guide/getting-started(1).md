# POWER BI EMBEDDED HANDS ON LAB

### Overall Estimated Duration: 3 hours

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

![](../media/archdiagram.JPG)

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
 
Once you're ready to dive in, your virtual machine and **Lab Guide** will be right at your fingertips within your web browser.

   ![Create storage by clicking confirm.](../media/GettingStarted/gspage01.png)  

### Virtual Machine & Lab Guide
 
Your virtual machine is your workhorse throughout the workshop. The lab guide is your roadmap to success.
 
## Exploring Your Lab Resources
 
To get a better understanding of your lab resources and credentials, navigate to the **Environment Details** tab.

   ![Create storage by clicking confirm.](../media/GettingStarted/ai-900-gettingstarted-04.png)
 
## Utilizing the Split Window Feature
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Top right corner.
 
   ![](../media/GS8.png)
 
## Managing Your Virtual Machine
 
Feel free to start, stop, or restart your virtual machine as needed from the **Resources** tab. Your experience is in your hands!
 
  ![](../media/GS5.png)

## Lab Validation

1. After completing the task, hit the **Validate** button under Validation tab integrated within your lab guide. If you receive a success message, you can proceed to the next task, if not, carefully read the error message and retry the step, following the instructions in the lab guide.

   ![Inline Validation](../media/inline-validation.png)

1. You can also validate the task by navigating to the **Lab Validation** tab, from the upper right corner in the lab guide section.

   ![Lab Validation](../media/lab-validation.png)

1. If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com.

 
## Let's Get Started with Azure Portal
 
1. On your virtual machine, click on the Azure Portal icon as shown below:
 
    ![](../media/GS1.png)
 
1. You'll see the **Sign into Microsoft Azure** tab. Here, enter your credentials:
 
   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>
 
      ![](../media/GS2.png "Enter Email")
 
3. Next, provide your password:
 
   - **Password:** <inject key="AzureAdUserPassword"></inject>
 
      ![](../media/GS3.png "Enter Password")

1. If you see the pop-up Action Required, click **Ask Later**.

   ![](../media/asklater.png)

   >**NOTE:** Do not enable MFA, select **Ask Later**.
 
1. If you see the pop-up **Stay Signed in?**, click **No**.

   ![](../media/GS9.png)

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the lab.

1. If a **Welcome to Microsoft Azure** popup window appears, click **Maybe Later** to skip the tour.

## Support Contact
 
The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:
- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

Now, click on **Next** from the lower right corner to move on to the next page.

![](../media/GS4.png)

### Happy Learning!!
