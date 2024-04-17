# AzureCLI

## Interactive login and set subscription


## interactive login
```
az login
```

## set subscription Name
```
$subscriptionName = {subcriptionName}
```
## get Id and set subscription
```
$subscriptionId="$(az account list --query "[?name=='$subscriptionName'].id" --output tsv)"
az account set --subscription $subscriptionId
```

## Verify
```
az account show
```
