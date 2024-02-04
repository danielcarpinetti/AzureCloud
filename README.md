# AzureCloud

ARM Templates and Powershell Scripts

Instructions:

- To run a ARM Template
	- Open the PS
	- uptload the .json script
	- run the command below to create the Resource Group (Replace the fields accordantly):

$RGName = “galáxia-infra1-rg”
New-AzResourceGroup –Name $RGName -Location “brazilsouth”

	- Run the command below to execute the script:

New-AzResourceGroupDeployment -ResourceGroupName $RGName -TemplateFile arm-template-test.json

