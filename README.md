Login-AzureRmAccount

Get-AzureRmSubscription -SubscriptionId "xxx"
Select-AzureRmSubscription -SubscriptionId "xxx"
New-AzureRmResourceGroup -Name "ashishth-llap-cluster" -Location "East US2"-Force 
New-AzureRmResourceGroupDeployment -ResourceGroupName "ashishth-llap-cluster" -TemplateUri "https://raw.githubusercontent.com/ashishthaps/101-hdinsight-interactivehive/master/azuredeploy.json" -TemplateParameterFile "C:\llaparm\101-hdinsight-interactivehive\azuredeploy.parameters.json"
