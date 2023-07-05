# UET App Distributor Platform

_This plaform is used to launch and distribute web applications, developed by UET university's students, to the Internet._

## Overview
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
- Google Cloud Platform: hosting cloud provider 
- Kubernetes: container orchestration
- Elastic Search - Logstash - Kibana stack: platform log management
- Prometheus - Grafana: platform infrastructure monitoring
- Github with Github Actions: source code repository and CI/CD platform
- Terraform: provisions infrastructure
- Ansible: install, update, remove open-source applications

## Detail features
- Platform:
  - Provision infrastructure (Github Actions + Terraform):
    - [x] Network: VPC, firewall
    - [x] Compute: VM
    - [x] IAM: service account
  - Setup and manage Kubernetes (Github Actions + Ansible roles):
    - [ ] Set up MicroK8s
    - [ ] Manage cluster
  - Deploy platform applications (Github Actions):
    - [ ] Deploy supported databases: Postgres, MongoDB
    - [ ] Deploy Distributor