# DXC Framework Configuration (Example)
Example DXC Framework Configuration used in the CLI as well as in CloudFormation Templates.

This example shows the structure, but should be cloned and modified for each use.

### Related Repositories
The DXC Framework consists of a set of related repositories, each containing a subset of the
overall functionality
- **DXCF Framework CLI ([dxcf-cli](https://github.com/dxctechnology/dxcf-cli))** - Contains the CLI
  program written in Node.js 10, that manages the build process, and which will provide various
  utility methods over time to simplify steps of the buid process.
- **DXCF Framework Templates ([dxcf-templates](https://github.com/dxctechnology/dxcf-templates))** -
  Contains the CloudFormation Templates which are built by the CLI. These templates are written in
  YAML, and use the AWS cfn-init method in combination with scripts, in a manner similar to AWS
  Quick Starts, to automate functionality on Instances which can not be accomplished by
  CloudFormation direct. Additionally, Lambda-backed CustomResources are used in many areas to
  extend CloudFormation functionality.
- **DXCF Framework Functions ([dxcf-functions](https://github.com/dxctechnology/dxcf-functions))** -
  Contains the Lambda Functions which are used to extend CloudFormation via CustomResources, or
  implement additional management functionality, such as logic triggered by CloudWatch Events.
- **DXCF Framework Scripts ([dxcf-scripts](https://github.com/dxctechnology/dxcf-scripts))** -
  Contains scripts written in bash or PowerShell to implement various aspects of complex cfn-init
  automation logic, in a manner similar to AWS QuickStarts.
- **DXCF Framework Configuration Example ([dxcf-config](https://github.com/dxctechnology/dxcf-config))** -
  *Because of the sensitive nature of the Configuration data, this is not yet Open Source, but we will
  have an example in place to show structure shortly.*
