asav-test-template
==================
Sample of Microsoft Azure - ARM Template to deploy Cisco ASAv with related Azure Resource.

## Requirements
Existing Resource Group, Storage Account in MS Azure Emvironment

## Installation
1. Copy all the json script (asav-test-template.json) to your newly added ARM Template section in Azure Portal
2. Configuration
3. Deploy from Template

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F100-blank-template%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F100-blank-template%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a>

## Configuration
Modify each parameter for your Cisco ASAv deployment in MS Azure.

	"virtualNetworks_name": {
            "defaultValue": "(your VNET name)", 
		"addressSpace": {
                    "addressPrefixes": [
                        "(your VNET IP address prefix : "10.1.0.0/16")"
												
	"virtualMachines_ASAv_name": {
            "defaultValue": "(your ASAv VM name)" ,

	"storageAccounts_name": {
            "defaultValue": "(your Storage account name)",

	"networkInterfaces_ASAv_01_Nic[0-3]_name": {
            "defaultValue": "(your ASAv Nic[0-3] name)",
		"privateIPAddress": "(your ASAv Nic[0-3] IP address : "10.1.0.4")"
		"addressPrefix": "(your ASAv Nic[0-3] IP address prefix : 10.1.0.0/24")",

	"routeTables_(interface name)_ASAv_RouteTable_name": {
            "defaultValue": "(your ASAv Route Table name)",
            
	"publicIPAddresses_name": {
            "defaultValue": "(your Public IP address name)",
            
	"networkSecurityGroups_ASAv_01_SecurityGroup_name": {
            "defaultValue": "(your ASAv SG name)",

	"osProfile": {
		"adminUsername": "(ASAv login username)",
		"adminPassword": "(ASAv login password)",
