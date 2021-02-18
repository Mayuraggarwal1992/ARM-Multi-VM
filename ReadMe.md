
## For Deployment

az account set -s  ITS-APPOPS-TW-NUA01-QA

### Bank
az group deployment validate --resource-group  TheBestBank --template-file azuredeploy.json --parameters bank.parameters.json

az group deployment create --resource-group  TheBestBank --template-file azuredeploy.json --parameters bank.parameters.json

### Retailer
az group deployment validate --resource-group  TheBestRetailer --template-file azuredeploy.json --parameters retailer.parameters.json

az group deployment create --resource-group  TheBestRetailer --template-file azuredeploy.json --parameters retailer.parameters.json