# Secure Azure DevOps CI/CD Pipeline (DevSecOps Demo)

This repository demonstrates a reusable Azure DevOps YAML pipeline that follows modern CI/CD and DevSecOps practices. It is designed as a portfolio-ready example for teams looking to standardize builds, testing, and security checks.

## Goals
- Provide a clean, production-style Azure DevOps pipeline structure
- Demonstrate staged CI/CD: Build → Test → Security/Quality → Package
- Show how to enforce basic quality gates and where security tooling can be integrated

## What the Pipeline Does
### Stage 1: Build & Test
- Installs .NET SDK
- Restores dependencies
- Builds in Release mode
- Runs unit tests and publishes test results

### Stage 2: Security & Quality Checks (Demo)
- Includes placeholders for:
  - Dependency scanning (e.g., OWASP Dependency-Check, Snyk, Trivy)
  - SAST scanning (e.g., SonarQube, CodeQL)
- Demonstrates a simple quality gate that fails the pipeline if `TODO` markers exist

### Stage 3: Package
- Publishes a build artifact (example packaging step)

## How to Use
1. Import this repository into Azure DevOps Repos (or connect from GitHub)
2. Create a new pipeline and select `azure-pipelines.yml`
3. Run the pipeline on the `main` branch

## Customization Ideas
- Replace placeholder steps with real security scanners (SAST/DAST)
- Add deployment stages for Dev/Test/Prod environments
- Add approval gates and environment checks
- Publish coverage reports and code quality metrics

## Skills Demonstrated
- Azure DevOps YAML pipelines
- CI/CD best practices
- Quality gates
- Secure pipeline patterns (DevSecOps-ready structure)

## Notes
This is a demo project intended for portfolio and learning purposes. It contains no proprietary code, secrets, or environment-specific details.
