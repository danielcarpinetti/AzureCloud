AZURE CLI COMMANDS

	- List all the subscriptions on the ID account and which one is in use:

az account list --query "[].{Nome:name, Selecionada:isDefault}"
	OR
az account list --output table


To set a subscription:

az account set  --subscription <Subscription>


	- List the Vnets

az network vnet list


	- List all the VMs with Zones In the subscription:

az vm list --query "[].{Name:name, Type:type, Zone:zones}"



	- To check the effective route Table

Get-AzEffectiveRouteTable `

-NetworkInterfaceName myVMNic1 `

-ResourceGroupName myResourceGroup `



