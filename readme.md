https://github.com/marketplace/actions/azure-functions-action

Create the Function App
Create  .github/workflow/actions.yml
Create a Service Principal

/subscriptions/4fd85f80-d7c8-46d0-9b86-ba3b7402377a/resourceGroups/hacker6_helloworld/providers/Microsoft.Web/serverFarms/ASP-hacker6helloworld-bd6a

  az ad sp create-for-rbac --name "helloworld" --role contributor \
                            --scopes /subscriptions/4fd85f80-d7c8-46d0-9b86-ba3b7402377a/resourceGroups/hacker6_helloworld/providers/Microsoft.Web/sites/hacker6helloworld \
                            --sdk-auth
{
  "clientId": "496a6f8f-3de9-49d8-a96f-920ec6922102",
  "subscriptionId": "4fd85f80-d7c8-46d0-9b86-ba3b7402377a",
  "tenantId": "6065c98a-b00b-42a9-a805-f81775ebdf92",
  "activeDirectoryEndpointUrl": "https://login.microsoftonline.com",
  "resourceManagerEndpointUrl": "https://management.azure.com/",
  "activeDirectoryGraphResourceId": "https://graph.windows.net/",
  "sqlManagementEndpointUrl": "https://management.core.windows.net:8443/",
  "galleryEndpointUrl": "https://gallery.azure.com/",
  "managementEndpointUrl": "https://management.core.windows.net/"
}

