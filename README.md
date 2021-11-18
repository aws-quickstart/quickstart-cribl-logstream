## quickstart-cribl-logstream—Quick Start
This Quick Start guide was created by [Cribl](https://cribl.io) to help automate the deployment of [Cribl LogStream](https://cribl.io/logstream/) in your AWS environment. These  automated reference deployments use AWS CloudFormation templates to deploy EC2 instances, IAM policies and S3 buckets, following AWS best practices. 

You can use the AWS Cloudformation templates included with the Quick Start to deploy a Cribl LogStream instance in your AWS account in about 15 minutes. The Quick Start automates the following:


| VPC | ARM64 | x86_64 |
| --- | ---- | ---- |
| Deploy in an existing VPC | [Cribl LogStream ARM64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-2.s3.us-west-2.amazonaws.com/logstream/cribl-single-template-arm64.yaml) | [Cribl LogStream x86_64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-2.s3.us-west-2.amazonaws.com/logstream/cribl-single-template.yaml) |
| Deploy in a new VPC | [Cribl LogStream ARM64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-1.s3.us-west-1.amazonaws.com/logstream/cribl-single-template-vpc-arm64.yaml) | [Cribl LogStream x86_64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-1.s3.us-west-1.amazonaws.com/logstream/cribl-single-template-vpc.yaml) |
| Deploy in new VPC with Flow Logs to s3 enabled | [Cribl LogStream ARM64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-2.s3.us-west-2.amazonaws.com/logstream/cribl-single-template-vpc-logging-arm64.yaml) | [Cribl LogStream x86_64](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/template?stackName=Cribl-LogStream&templateURL=https://aws-quickstart-cribl-logstream-us-west-2.s3.us-west-2.amazonaws.com/logstream/cribl-single-template-vpc-logging.yaml) | 

![Architecture](/docs/images/architecture_diagram.png)

For architectural details, step-by-step instructions, and customization options, see the [deployment guide](https://aws-quickstart.github.io/quickstart-cribl-cribl-logstream/).


To post feedback, submit feature ideas, or report bugs, use the [**Issues**](https://github.com/amiracle/quick-start-cribl/issues) section of this [GitHub repo](https://github.com/amiracle/quick-start-cribl).

To submit code for this Quick Start, see the [AWS Quick Start Contributor's Kit](https://aws-quickstart.github.io/).