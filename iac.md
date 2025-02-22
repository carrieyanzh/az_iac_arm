az storage account create -n myacctname0220 -g myrg0220
 
az group export -g myrg0220 > simpletemplate0220.json

az group deployment create --template-file simpletemplate0220.json --parameters storageAccounts_0220_name=mystorageacct0220 -g myrg0220

az storage account list -g myrg0220 --query "[].name"

az group deployment create --template-file simpletemplate0220.json --parameters storageAccounts_0220_name=mystorageacct0220 -g myrg0220 --mode complete

az storage account list -g myrg0220 --query "[].name"

git clone https://github.com/cadullms/simplegreet 

New-AzResourceGroupDeployment -name "episode03_01" -resourcegroupname "my_rg0218" -templatefile .\template.json -TemplateParameterObject $ParametersObj

$ParametersObj = @{
storageAccountName= "my0221"
storageAccountType = "mytype0221"
}

New-AzResourceGroupDeployment -name "episode03_01" -resourcegroupname "my_rg0218" -templatefile .\template.json -TemplateParameterfile .\template.param.json

Functions:
Numberic - add, div, min, max, copyIndex
string : conct, contains, split, replace, trim
Date: uctNow, dateTimeAdd
Resource : list keys , ResourceGroup
Comparision: equals , greater, less
Logical : and , or , not , if
Array : concat, length , range, take, union

New-AzResourceGroupDeployment -name "episode03_01" -resourcegroupname "my_rg0218" -templatefile .\functiontemplate.json 


 1 try { . "c:\Users\carrieyanzh\AppData\Local\Programs\Microsoft VS Code\resources\app\out\vs\workbench\contrib\...
   2 bicep
   3 bicep --help
   4 bicep --version
   5 az --version
   6 Get-InstalledModule
   7 $PSVersionTable.PSVersion
   8 cls
   9 clear
  10 lcs
  11 cls
  12 history
  13 Get-InstalledModule AZ
  14 Get-InstalledModule Az

