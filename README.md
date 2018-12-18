asav-test-template
==================
Sample of Microsoft Azure - ARM Template to deploy Cisco ASAv with related Azure Resource.

## Requirements
Existing Resource Group in MS Azure Emvironment

## Installation
Copy all the json script to your newly added ARM Template section in Microsoft Azure

## Configuration
Modify each parameter for your Cisco ASAv deployment in MS Azure.

	"virtualNetworks_vnet01_name": {
            "defaultValue": "(your VNET name)", 
		"addressSpace": {
                    "addressPrefixes": [
                        "(your VNET IP address prefix : "10.1.0.0/16")"
												
	"virtualMachines_ASAv_01_name": {
            "defaultValue": "(your ASAv VM name)" ,

	"storageAccounts_shkimura_name": {
            "defaultValue": "(your Storage account name)",

	"networkInterfaces_ASAv_01_Nic[0-3]_name": {
            "defaultValue": "(your ASAv Nic[0-3] name)",
		"privateIPAddress": "(your ASAv Nic[0-3] IP address : "10.1.0.4")"
		"addressPrefix": "(your ASAv Nic[0-3] IP address prefix : 10.1.0.0/24")",

	"routeTables_(interface name)_ASAv_RouteTable_name": {
            "defaultValue": "(your ASAv Route Table name)",
            
	"publicIPAddresses_PIP_001_name": {
            "defaultValue": "(your Public IP address name)",
            
	"networkSecurityGroups_ASAv_01_SecurityGroup_name": {
            "defaultValue": "(your ASAv SG name)",

	"osProfile": {
		        "adminUsername": "(ASAv login username)",
            "adminPassword": "(ASAv login password)",
