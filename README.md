# AzureCLI

##Interactive login and set subscription

```
## interactive login
az login
## set subscription
$subscriptionName = 'set name'
subscriptionId="$(az account list --query "[?name=='$subscriptionName'].id" --output tsv)"
az account set --subscription $subscriptionId
```
- 
