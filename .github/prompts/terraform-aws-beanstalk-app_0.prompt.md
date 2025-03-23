# Terraform AWS Elastic Beanstalk Application Module

Create a Terraform module for deploying the Django Terraform UI application on AWS Elastic Beanstalk.

## Requirements

1. Create a configurable Terraform module that sets up an AWS Elastic Beanstalk environment for the Django Terraform UI application.
2. Support Docker platform for Elastic Beanstalk.
3. Include all necessary AWS resources:
   - Elastic Beanstalk application
   - Elastic Beanstalk environment
   - Application Load Balancer
   - Auto Scaling Group configuration
   - Security Groups
   - IAM roles and instance profiles
   - CloudWatch Logs configuration
   - Optional RDS database for Django backend
4. Design a configuration system that allows:
   - Customizing instance types and sizes
   - Setting environment variables for the Django application
   - Configuring auto-scaling parameters
   - SSL certificate attachment
   - VPC and subnet configuration

## Module Structure

1. Follow Terraform module best practices for structure and organization.
2. Create separate resource files for logical groupings (eb.tf, iam.tf, etc.).
3. Provide comprehensive variable definitions with proper descriptions and defaults.
4. Include useful outputs for integration with other resources.
5. Create examples directory with common usage patterns.

## Features

1. Support for custom Docker images from ECR or public registries.
2. Configuration for environment variables to be passed to the Django application.
3. Integration with AWS secrets manager for sensitive variables.
4. CloudWatch alarms for monitoring the environment.
5. Elastic Beanstalk platform updates handling.
6. Configurable health check paths and thresholds.
7. Support for blue/green deployments.

## Security Considerations

1. Implement security group best practices.
2. Use principle of least privilege for IAM roles.
3. Support encryption for data at rest and in transit.
4. Configure proper logging and monitoring.
5. Implement secure handling of environment variables.

## Documentation

1. Create comprehensive README with usage examples.
2. Document all variables and outputs clearly.
3. Include architecture diagrams.
4. Provide guidance on security best practices.
