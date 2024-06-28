# paas-coding-interview

## Study case

> This study case could be long and not achieved at the end of the interview. What we expect is to have enough material to evaluate the candidate skills even if the case is not completed

* Fork this project
* Write a simple CLI in Go / Python
  * It should implement a workflow in sync command with the following steps:
    * Get a parameter with application_name
    * Activate Datadog downtime
    * Trigger ArgoCD app sync (The application is ready to be deployed, just need to trigger the sync)
    * Remove Datadog downtime
* Create a pull request to share your work with us 

You must:
* Mock all real calls to Datadog/ArgoCD and write functions/methods which only retrieve hard coded struct base on service documentation
* Handle idempotency (what happen if the CLI fail in the middle of the run)

## Resources
 
* https://docs.datadoghq.com/api/latest/downtimes/ 
* https://cd.apps.argoproj.io/swagger-ui 
