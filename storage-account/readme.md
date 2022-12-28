### creating the resource group
`
az group create -l eastus -n storage-acct-rg
`

### deploying the template
`
az deployment group create --name armTestTemplate --resource-group storage-acct-rg --template-file "storage.json"
`

### deploy the template by using parameters
`
az deployment group create --name armTestTemplate --resource-group storage-acct-rg --template-file "storage.json" --parameters storageName='dbstorageaccount001' storageSKU='Standard_LRS'
`