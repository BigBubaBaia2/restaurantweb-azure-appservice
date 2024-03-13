# Deploying Restaurant Web Using Azure App Services

This guide outlines the steps to deploy the Restaurant Web application using Azure App Services, with specific customizations to the standard process.

## Getting Started

First you can follow the tutorial on deploying a Python and PostgreSQL app in Azure App Services provided by Microsoft:

[Tutorial: Build a Python and PostgreSQL app in Azure App Services](https://learn.microsoft.com/en-us/azure/app-service/tutorial-python-postgresql-app?tabs=django%2Cwindows&pivots=azure-portal)

**Note:** Instead of using the GitHub project suggested in the tutorial, we will utilize our own project located at: [https://github.com/ISYS53333/restaurantweb-azure-appservice](https://github.com/ISYS53333/restaurantweb-azure-appservice), you should FORK this repository and then use your own repository.  This will allow you to see how automated changes are pushed to the app services code when changes are made to the code base.

Please begin directly from **Step 1** of the tutorial, applying the following changes and additions as you proceed. Also feel free to use your own naming in Step 2:

### Changes and Additions

- **Step 4 (Configure Authentication):** Choose **Basic Authentication** instead of User-Assigned Identity under Authentication Types.

- **After completing Step 4:** Execute an additional command to populate the database with initial data:

  ```bash
  python manage.py loaddata menu_data.json
  ```
