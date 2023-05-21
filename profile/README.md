# UET App Distributor Platform

_This plaform is used to launch and distribute web applications, developed by UET university's students, to the Internet._

## Features
App Distributor Platform provides several features:
  - For development team: 
    - Automatically deploy applications with databases
    - Automatically add a domain name for deployed applications (hard, so this is optional)
    - Provide logs, dashboards and monitors for deployed applications
    - Connect with source control systems to automatically rollout new application versions
  - For operations team:
    - Cloud-native solution with lowest cost
    - Provision the whole Platform with one click
    - Provide logs, dashboards, and monitor for Platform infrastructures

Administrators only need to update the `requirement.yaml` file, then the platform will provision and manage the rest.

## Technology stack
- Kubernetes: manage containerized applications
- Elastic Search - Logstash - Kibana (ELK) stack: monitor application logs
- Gitlab - Gitlab CI: source code repository and CICD platform
- Terraform: provisions infrastructure
- Ansible: install, update, remove open-source applications

## User workflow
- Prepare application code on a source control system
- Access UET App Distributor Platform Portal to manually trigger application deployment
-  

## Approach