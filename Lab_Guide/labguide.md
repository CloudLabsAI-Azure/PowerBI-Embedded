# Power BI Embedded Workshop Guide

## Outcome

At the end of this workshop, you will learn how to –
1. Module 1: Embed a Power BI report using App Owns Data embedding
1. Module 2: Embed Q&A (Question & Answer) for a Power BI dataset
1. Module 3: Understand exporting a visual’s data 
1. Module 4: Enable data security based on user context

## Getting started
1. Open the App Owns Data sample code from your desktop

1. Open the sample in VS Code and run the sample as is

Files to be updated while completing the modules

1. /appsettings.json
1. /wwwroot/js/index.js
1. /Services/PBIEmbedService.cs

## Hands-on

### Module 1: Embedding Your First Power BI report

1. Login to your virtual machine with the username and password provided (hacker1/password).

1. Open up a browser and login to powerbi.com with the user and password provided (i.e. 
hacker1@ /password)

1. Find the workspace related to your hacker# (i.e. hacker1, hacker2, … hackerXX, etc.) and locate
the “Wingtip Sales Analysis” report.

   ![](media/pbi1.png)

    Capture the Workspace ID, Report ID, and Dataset ID for this report and put it into notepad.

1. Launch Visual Studio Code – which can be found on your virtual machine.

   ![](media/pbi2.png)

1. In Visual Studio Code – click on **Open Folder** and point to the folder where the solution can be 
found – this folder should be on your desktop:

   ![](media/pbi3.png)

1. Navigate to the `/appsettings.json` file and **add/update** the Azure AD and Power BI configurations 
i.e., client ID, tenant ID, client secret, workspace ID, report ID, and dataset ID.

    **Important**:

    1. Azure AD configurations (client ID, tenant ID, client secret) will be shared with you 
during the session.
    
    1. For Power BI configuration, you can refer to the earlier steps where you captured
workspace ID, report ID, dataset ID.

   ![](media/pbi4.png)

1. Click on the Terminal and type in `dotnet run` and Enter to run the sample code to embed the 
power bi report `Wingtip Sales Analysis` in READ mode.

   ![](media/pbi4.png)

1. Once the code is executed, you can click on the link `https://localhost:5001` as shown below to 
launch the browser/app:   

   ![](media/pbi5.png)

1. Once the browser is launched, you should see a web app that has now embedded your “Wingtip 
Sales Analysis” report you viewed from Power BI in the earlier steps.




   