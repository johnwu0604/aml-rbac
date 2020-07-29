# Azure Machine Learning - Advanced Role-Based Access Control (RBAC)

The following repository shows an example of how to create custom roles on Azure Machine Learning. Using some of the provided templates, you can create role definitions that prevent datastore registration, model deployment, or compute creation.

## Prequisite

Make sure you have the [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest) installed and you are logged into your subscription. 

## How to create a new role

1. Use one of the sample templates or creation a new template using the same format. All available operations are listed in the `superuser-role.json` file. You can also find the full list and their definitions [here](https://docs.microsoft.com/en-us/azure/role-based-access-control/resource-provider-operations#microsoftmachinelearningservices)

2. Replace the `SUBSCRIPTION_ID` with your subscription ID or modify the scope which you want to assign the role

3. Run `az role definition create --role-definition data-scientist-role.json`
