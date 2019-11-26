# debian-aws-tools

Base Debian Buster image with [AWS CLI](https://aws.amazon.com/cli/), [AWS SSM Agent](https://docs.aws.amazon.com/systems-manager/latest/userguide/ssm-agent.html) and [jq](https://stedolan.github.io/jq/) installed. 

Running this container on the ec2 instance with proper IAM permissions will allow running any `aws` command, including `aws ssm` inside the container.

## Example use
```
docker run krzyzakp/debian-aws-tools:latest aws ssm start-session --region eu-central --target i-XXXXXXXXXXXXXXX
```
