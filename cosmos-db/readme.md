### creating the resource group
`
az group create -l eastus -n cosmos-acct-rg
`

### deploying the template
`
az deployment group create --name armTestTemplate --resource-group cosmos-acct-rg --template-file "main.json"
`

### deploy the template by using parameters
`
az deployment group create --name armTestTemplate --resource-group cosmos-acct-rg --template-file "main.json" --parameters <param1=val1 param2=val2>
`