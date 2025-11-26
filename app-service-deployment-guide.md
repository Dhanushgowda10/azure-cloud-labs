# Azure App Service Deployment Guide

## Objective of the Lab

- Deploy a Web App using Azure App Service
- Learn how to configure App Service settings including runtime, region, and deployment options
- Integrate GitHub for continuous deployment
- Gain hands-on experience managing web applications in a cloud environment

---

## Task 1: Deploying a Web App in Azure App Service

In this task, you will deploy a Java-based Web App on Azure using App Service and configure it for continuous deployment from GitHub.

### Step 1: Navigate to App Service

1. In the Azure portal, type **App Service** into the search bar
2. Select **App Service** from the search results

### Step 2: Start Creating a Web App

1. On the App Service page, click **Create**
2. From the dropdown, select **Web App**

### Step 3: Fill in the Basics Tab

In the Basics tab, enter the following details:

| Setting | Value |
|---------|-------|
| Subscription | Choose your subscription |
| Resource Group | Select your existing resource group |
| Name | Provide a unique name for your web app |
| Publish | Select **Code** |
| Runtime Stack | Select **Java 17** |
| Java Web Server Stack | Choose **Java SE Embedded Web Server** |
| Operating System | Select **Windows** |
| Region | Choose **West US** |
| Windows Plan | Click Create new, enter a name for your App Service plan, and click OK |

Click **Next: Database** to continue.

### Step 4: Skip the Database Tab

- No database is needed for this web app
- Simply click **Next: Deployment**

### Step 5: Configure Deployment Settings

In the Deployment tab:

1. **Continuous Deployment**: Enable it
2. **GitHub Account**: Click **Change account**
3. A popup will appear - authorize AzureAppServices, enter your GitHub password, and click **Confirm**

Fill the remaining fields:

| Setting | Value |
|---------|-------|
| Organization | Enter your GitHub username |
| Repository | Select the repository where your code is stored |
| Branch | Select **main** |

Click **Review + create**

### Step 6: Create the App Service

- On the Review + create page, verify all configurations
- Click **Create** to begin deployment

### Step 7: Access the Deployed Web App

1. Once deployment is complete, click **Go to resource** on the deployment page
2. In the Overview tab of your App Service, click **Browse** to open your live web application

---

## Summary

You have successfully:
- Created an Azure App Service Web App
- Configured Java runtime environment
- Set up continuous deployment from GitHub
- Deployed and accessed your live web application
