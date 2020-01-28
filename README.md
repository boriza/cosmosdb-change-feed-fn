# Cosmos DB change feed trigger processing with Azure Functions v2

1) install azure function cli, az cli on your machine, VS.Code and Azure Functions Extension

2) in local.settings.json
```
{
  "IsEncrypted": false,
  "Values": {
    "AzureWebJobsStorage": "STORAGE CONTAINER CONNECTION",
    "FUNCTIONS_WORKER_RUNTIME": "dotnet",
    "DOCUMENTDB": "DOCUMENTDB CONNECTOIN STRING"
  }
}
```
3) Finally run locally func start --build

4) Deploy with 
```
func azure functionapp publish <FunctionAppName> --publish-local-settings -i	

```