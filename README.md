# debian-aws-ssm-agent

Base Debian Buster image with [AWS CLI](https://aws.amazon.com/cli/) and [AWS SSM Agent](https://docs.aws.amazon.com/systems-manager/latest/userguide/ssm-agent.html) installed. 

Running this container on the ec2 instance with proper IAM permissions will allow running any `aws` command, including `aws ssm` inside the container.

## Example use
```
docker run krzyzakp/debian-aws-ssm-agent:latest aws ssm start-session --region eu-central --target i-XXXXXXXXXXXXXXX
```
