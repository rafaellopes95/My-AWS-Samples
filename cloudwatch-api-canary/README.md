# CloudWatch Synthetics - Canary for API
This project contains a template that creates the following top level resources:
* Canary -> Resource that will send synthetic traffic to check availability of the API.
* API -> Resource that has a mock endpoint.

## Deploying the template
Before deploying the template, validate the template with SAM as below:

sam validate

Note: Run that command inside template.yaml folder, or specify its path with -t option.

In case SAM says "Is a valid SAM template", then proceed and deploy the stack using the following command:

sam deploy --guided --capabilities CAPABILITY_NAMED_IAM

Note: On next steps run only sam deploy command if you prompted "Y" to save the preferences into samconfig.toml file.
