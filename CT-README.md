## Cribl Stream Partner Solution

This Partner Solution deploys Cribl Stream on the AWS Cloud. If you are unfamiliar with AWS Partner Solutions, refer to the [AWS Partner Solutions General Information Guide](https://aws-ia.github.io/content/qs_info.html).

### Cost and licenses

This Partner Solution requires a subscription to [Cribl Stream Single Instance (Free) x86_64](https://aws.amazon.com/marketplace/pp/prodview-3wsytwvqb65gg?sr=0-1&ref_=beagle&applicationId=AWSMPContessa) on the AWS Marketplace.

There are no additional licenses required to use this Partner Solution.

There is no cost to use this Partner Solution, however you will be billed for the resources deployed. For more information see the [AWS Partner Solutions General Information Guide](https://aws-ia.github.io/content/qs_info.html).

### Architecture
![alt text][#architecture1]

[#architecture1]: https://aws-quickstart.github.io/quickstart-cribl-logstream/docs/deployment_guide/images/architecture_diagram.png "Partner Solution architecture for Cribl Stream Partner Solution on AWS"

### How to use
This solution is designed to be deployed in your Home Region only.

When you deploy the solution you will need to provide the following parameters:

Network configuration:
----------------------

| Parameter label (name) | Default | Description |
| --- | --- | --- |
| Availability Zones  <br>(AvailabilityZones) | Requires input | List of Availability Zones to use for the subnets in the VPC. |
| VPC CIDR  <br>(VPCCIDR) | 10.0.0.0/16 | CIDR Block for the VPC. |
| Public subnet 1 CIDR  <br>(PublicSubnet1CIDR) | 10.0.128.0/20 | CIDR block for the public DMZ subnet 1, located in Availability Zone 1. |
| Public subnet 2 CIDR  <br>(PublicSubnet2CIDR) | 10.0.144.0/20 | CIDR block for the public DMZ subnet 2, located in Availability Zone 2. |
| Private subnet 1 CIDR  <br>(PrivateSubnet1CIDR) | 10.0.0.0/19 | CIDR block for private subnet 1, located in Availability Zone 1. |
| Private subnet 2 CIDR  <br>(PrivateSubnet2CIDR) | 10.0.32.0/19 | CIDR block for private subnet 2, located in Availability Zone 2. |
| VPC tenancy  <br>(VPCTenancy) | default | The allowed tenancy of instances launched into the VPC. |

  

Amazon EC2 configuration:
-------------------------

| Parameter label (name) | Default | Description |
| --- | --- | --- |
| EC2 instance type  <br>(instanceType) | c6g.xlarge | EC2 instance type to provision the LogStream instance. If none specified, c6g.2xlarge is used. |
| (webAccessCidr) | 0.0.0.0/0 | REQUIRED: The CIDR IP range permitted to access the LogStream web console. We recommend you set this value to a trusted IP range. |

  

AWS Quick Start configuration:
------------------------------

| Parameter label (name) | Default | Description |
| --- | --- | --- |
| Quick Start S3 bucket name  <br>(QSS3BucketName) | aws-quickstart | Name of the S3 bucket for your copy of the Quick Start assets. Keep the default name unless you are customizing the template. Changing the name updates code references to point to a new Quick Start location. This name can include numbers, lowercase letters, uppercase letters, and hyphens, but do not start or end with a hyphen (-). See https://aws-quickstart.github.io/option1.html. |
| Quick Start S3 key prefix  <br>(QSS3KeyPrefix) | quickstart-cribl-logstream/ | S3 key prefix that is used to simulate a directory for your copy of the Quick Start assets. Keep the default prefix unless you are customizing the template. Changing this prefix updates code references to point to a new Quick Start location. This prefix can include numbers, lowercase letters, uppercase letters, hyphens (-), and forward slashes (/). End with a forward slash. See https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingMetadata.html and https://aws-quickstart.github.io/option1.html. |
| (QSS3BucketRegion) | us-east-1 | AWS Region where the Quick Start S3 bucket (QSS3BucketName) is hosted. Keep the default Region unless you are customizing the template. Changing this Region updates code references to point to a new Quick Start location. When using your own bucket, specify the Region. See https://aws-quickstart.github.io/option1.html. |