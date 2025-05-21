# Welcome to the handson example

## Situation

You can find here the sourcecode of a java springboot service. It is a simple demo service, not containing any complex functionality.
Your task is now to create an openshift pipeline as code (using the Openshift pipeline as code feature) that checks out the code from the git repository, builds the java part and does a code scan with Sonarqube.
The developer uses maven as a build tool and centralized the sonarqube configuration in a separate properties file.

## Expected output:
* You have checked out the code from this repository
* You have developed the code for the pipeline in your IDE
* You have code templates for all additional resources.
* We will copy your code into a training environment and run the code/pipeline
* Please walk us through the necessary steps for that.

## Helpfull information:

As target namespace please use 'asolutions-pipelines' on an Openshift-cluster
Following secrets and PVCs are already stored in the namespace:

### Secrets:
- bitbucket-server-webhook-config (containing the webhook secret and the personal accesstoken for bitbucket)
    - provider.token (bitbucket PSA)
    - webhook.secret (webhook secret)

- sonar (containing the token for sonarqube/sonarcloud).
    - token (sonarqube/sonarcloud PSA)

### PVC:
- pipeline-shared-workspace

## GOOD LUCK!
