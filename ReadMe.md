
## For Deployment

az account set -s  ITS-APPOPS-TW-NUA01-QA

az group deployment validate --resource-group  XXXX --template-file azuredeploy.json --parameters bank.parameters.json

az group deployment create --resource-group  XXXXX --template-file azuredeploy.json --parameters bank.parameters.json

