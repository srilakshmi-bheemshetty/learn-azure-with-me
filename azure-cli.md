# Create VM using Azure CLI

### Starting with resource group

    az group create --name MyResourceGroup --location eastus

### Creating VM with Vnet
az vm create `

    --resource-group $resourceGroup `
    --name $vmName `
    --image Ubuntu2204 `
    --vnet-name $vnetName `
    --subnet $subnetName `
    --generate-ssh-keys `
    --output json `
    --verbose

### Delete the Resource Group to delete all the resources


	az group delete --name leaning-azure-cli
