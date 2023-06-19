# GitHub actions CI/CD pipeline for MuleSoft 
### Branch Management
The **Main branch** is used for Staging and Production environments. To run the workflow, you need to manually click on it. You will be prompted to select the environment you want to deploy to: 
  1. **prod**: Deploys the main branch to Staging and Production environments.
  2. **stag**: Deploys only to the Staging environment.

     Please note that this branch does not perform testing and will automatically deploy after running the workflow.
  
The **Dev branch** is intended for QA and Developer environments. This branch automatically executes tests, logs, builds, and deploys after a Pull Request (PR), Merge, or Cron job.

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
There are 3 workflows available:
1. **CICD** this is a main workflows to config.
2. **CI** reuseable workflow for CI (test build snapshot).
3. **CD** reuseable workflow for CD (deployment).
   
> **Note**
> 
> This is a simple Mule application for testing only.

## Other resources

