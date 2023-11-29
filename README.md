# terraform-github-actions-project

1. create service principal and assign contributing access on subscription
 az ad sp create-for-rbac --name "github-action-spn" --role contributor --scopes /subscriptions/subscription-id --sdk-auth

2. Save the ClientID, ClientSecret, SubscriptionId, TenantID from above commands result in the Github respository secret.