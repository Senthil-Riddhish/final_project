## Kovid
###### Industry     : Health 
###### Project Link : [https://agreeable-moss-0efea7910.1.azurestaticapps.net](https://senthil-riddhish.github.io/final_project/)
## Project Description :
A website that provides various services. All services in one place. In order to solve the problem, the patients can automatically register the portal and can able to book an appointment with a doctor with the proper guidance. Worked in an healthcare filed and tried to bring all kinds of services in a single place. The purpose of the website is to help those who didn't get proper consultation from the doctor and suffering from the disease. Where it be opportunity and continent for them where they can able to register and get proper guidance from them.
###### Primary Azure Technology : Static Web Apps, Storage
## Flow chart :
<img src="https://docs.microsoft.com/en-us/azure/static-web-apps/media/local-development/cli-conceptual.png" height="50%" width="50%">

<img src="https://techcommunity.microsoft.com/t5/image/serverpage/image-id/183512i380FC55BF9A766DB/image-size/large?v=v2&px=999" height="50%" width="50%">

## Steps Followed
* Create a repository
- Clone the repository
* Create a static web app
<br />

1.Sign in to the Azure CLI by using the following command.
```
Azure CLI
az login
```
2.Create a resource group.
3.Create a variable to hold your GitHub user name.
```
GITHUB_USER_NAME=<YOUR_GITHUB_USER_NAME>
```
4.Create a new static web app from your repository.
```
az staticwebapp create \
    --name my-first-static-web-app \
    --resource-group my-swa-group \
    --source https://github.com/$GITHUB_USER_NAME/my-first-static-web-app \
    --location "eastus2" \
    --branch main \
    --app-location "src" \
    --login-with-github
```
5.Enter the user code as displayed your console's message.<br />
6.Select the Continue button.<br />
7.Select the Authorize AzureAppServiceCLI button.<br />
* View the website
```
az staticwebapp show \
  --name  my-first-static-web-app \
  --query "repositoryUrl"
```
```
az staticwebapp show \
  --name my-first-static-web-app \
  --query "defaultHostname"
```
## Github commands : 
```
git init
git add -A
git commit -m 'Added my project'
git remote add origin git@github.com:sammy/my-new-project.git
```
## Problem Statement/Opportunity :
A service-based website where it provides various kinds of services. Many people can't get the opportunity to consult a doctor and facing difficulties to get prescription from them. Even the old age people can't get the doctor's appointment. But website that has been created provides various services like testing the patient's doctor appointment and doctor consultancy. All these services in a single place where the patients can be benefited. The future and enhancement would be disease identification along with the proper systematic consultant. The medicine and consultant in a systematics mode. The opportunity would be development and upgradation of doctor and patient co-ordination. Provides help for those who didn't get an opportunity to consult a doctor.

      
