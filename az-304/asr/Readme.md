# Azure Disaster Recovery Demo 

I have a prepared a demo for my azure learners. This ARM Template would help them setup a sample 'source' environment with A Network, Storage and VM.

## ARM Template for Primary Site 

```powershell
New-AzResourceGroup -name src-group -Location eastus   

New-AzResourceGroupDeployment -Name de1 -TemplateFile .\azuredeploy.json -TemplateParameterFile .\azuredeploy.parameters.json -ResourceGroupName src-group
```
