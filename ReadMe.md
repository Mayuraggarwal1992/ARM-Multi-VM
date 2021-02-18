
## For Deployment of MUltiple VM - Spot Instances

az account set -s  xxxsub-namexxx

az group deployment validate --resource-group  XXXX --template-file azuredeploy.json --parameters parameters.json

az group deployment create --resource-group  XXXXX --template-file azuredeploy.json --parameters parameters.json

