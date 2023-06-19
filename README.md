# GitHub actions CI/CD pipeline for MuleSoft 
### Branch Management
  **Main branch** is for Staging and Production which you need to manually click to run the workflow. It will promt you with an input to select which enviroment you need to deploy to 
  1. **prod** (Deploy main branch to Staging and Production ENV)
  2. **stag** (Only deploy to staging)

     keep in mind that this branch will not do the testing and will deploy automaticly after you run the workflow
  
  **Dev branch** is for QA and Developer enviroment this branch will automaticly test-log-build-deploy after PR, Merge, and CRON job 

### Secrets and Varaibles
#### Varaibles for deployment
 1. CLOUDHUB_ENVIRONMENT: "prod-01"
 2. GITHUB_ENVIRONMENT: "prod"
 3. CLOUDHUB_WORKERS: "1"
 4. CLOUDHUB_WORKER_TYPE: "MICRO"
 5. CLOUDHUB_REGION: "ca-central-1"
 6. HTTP_PRIVATE_PORT: "8091"
#### Secrets
 1. ANYPOINT_PLATFORM_PASSWORD
 2. ANYPOINT_PLATFORM_USERNAME
 3. DECRYPTION_KEY

### Workflows
there are 3 workflows
1. **CICD** this is a main workflows to config
2. **CI** reuseable workflow for CI (test build snapshot)
3. **CD** reuseable workflow for CD (deployment)
> **Note**
> 
> This is a simple Mule application for testing only.

## Other resources

