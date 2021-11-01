# Introduction to Wegger

The purpose of this organization is for educational purposes solely. The goal of the BDSA 2021 project is to implement a vertical slice of the SE Training project. 

To read more about the project, see the [official description](https://docs.google.com/document/d/1tGa5GxtLnlMOByaU7yLQRKUboxcACghlc5asTOULlHQ/edit).

The project is licensed under GPL FLOSS. 


## For stakeholders 

In order to establish transparency in the process, stakeholders can keep track of the quality of the code with static code analysis reports at [SonarCloud](https://sonarcloud.io/organizations/wegger-bdsa2021/projects). 
#### webAPI
+ [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi)
+ [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=coverage)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi)
+ [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=bugs)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi)
+ [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi)
+ [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi) 
+ [![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=wegger-BDSA2021_webapi&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=wegger-BDSA2021_webapi)

Additionally, stakeholders can go to the [projects overview](https://github.com/orgs/wegger-BDSA2021/projects) to get an overview of work in progress. 


## Workflow strategy for repositories 

![Git Flow strategy](https://miro.medium.com/max/2000/1*tnvRls6Dg7vFt0zGdtfu_w.png)

All repositories in the project use the Git Flow strategy for the version control workflow. Please follow the instructions below before contributing any code to any of the repositories within the Wegger organisation. 
- `Main` only reflects the most current production ready state of the source code. The CD pipeline will deploy main to production upon merging with main. Only hotfix branches and the development branch may be merged into main - this can only be done via pull requests. 
- `Development` reflects the latest development for the next release. 
- `Feature` branches is to checked out from development (or another feature branch based on the preferences of the developer) and may only be merged into develop using pull requests. Before submitting a pull request, it is recommended to pull the latest version of remote development to your local environment and then merge it with your local feature branch. The name of the feature branch should be featurename_feature.
- `Hotfix` branches are for fixing bugs quickly that are already in production. Pull the latest version of main to your local machine, checkout a new branch, fix the bug, commit it locally, set the hotfix branch to track upstream, push it, and submit a pull request via github. Remember to merge the hotfix branch into develop as well. The name of the hotfix branch should be bug name_hotfix. 
- (`Release` branches will not be utilised for such a small project)




