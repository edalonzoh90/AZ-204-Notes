# AZ-204-Notes

### Using PowerShell
**Installing AZ module**  
`Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force`  

**Connecting to Azure Account**  
`Connect-AzAccount`  
  
**Connecting SSH**  
`ssh -i <path to .pem> azureuser@ip`
  
**Installing Apache**  
```
sudo apt update -y
sudo apt install -y apache2
sudo systemctl start apache2
sudo systemctl status apache2
```

**Create new Resource Group**  
`New-AzResourceGroup -Name GR-AZ-400 -Location 'EastUS'`

**Create new VM**  
`New-AzVM -ResourceGroupName 'GR-AZ-400' -Location 'EastUS' -ViertualNetworkName 'MyVMNet' -SubnetName 'default' -SecurityGroupName 'MyNSG'  -Name 'pwrsdemo' -PublicIpAddressName 'MyPublicIP' -OpenPort 80, 443`





**To verify if port 80 is open**  
https://ping.eu/port-chk/
