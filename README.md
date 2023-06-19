# GitHub actions CI/CD pipeline for MuleSoft 
### Branch Management
  **Main branch** is for Staging and Production which you need to manually click to run the workflow. It will promt you with an input to select which enviroment you need to deploy to such as prod (Deploy main branch to Staging and Production ENV) and stag (Only deploy to staging), keep in mind that this branch will not do the testing 
  
  **Dev branch** is for QA and Developer enviroment this branch will automaticly test-log-build-deploy after PR, Merge, and CRON job 


> **Note**
> 
> This is a simple Mule application to test. Please update the `app.name` and `env` properties from the `pom.xml` to your own.

## Other resources

The initial versions of the pipeline are based on the following repository created by Archana Patel: [arch-jn/github-actions-mule-cicd-demo](https://github.com/arch-jn/github-actions-mule-cicd-demo).
