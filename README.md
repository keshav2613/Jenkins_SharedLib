# Jenkins Shared Library 🚀

A reusable Jenkins Shared Library for standardizing CI/CD pipeline stages and reducing duplicated pipeline code across projects.

Includes reusable Groovy functions for Docker workflows, code-quality analysis, and DevSecOps security scanning.

## 🛠️ Technologies

`Jenkins` `Groovy` `Docker` `SonarQube` `Trivy` `OWASP Dependency-Check` `CI/CD` `DevSecOps`

## 📦 Shared Pipeline Functions

| Function                        | Purpose                           |
| ------------------------------- | --------------------------------- |
| `code_checkout.groovy`          | Source-code checkout              |
| `docker_build.groovy`           | Build Docker images               |
| `docker_push.groovy`            | Push Docker images to a registry  |
| `docker_compose.groovy`         | Docker Compose operations         |
| `docker_cleanup.groovy`         | Docker resource cleanup           |
| `sonarqube_analysis.groovy`     | SonarQube code analysis           |
| `sonarqube_code_quality.groovy` | SonarQube quality checks          |
| `owasp_dependency.groovy`       | Dependency vulnerability scanning |
| `trivy_scan.groovy`             | Container vulnerability scanning  |

## 🔄 CI/CD Workflow

`Code Checkout → Code Analysis → Security Scan → Docker Build → Docker Push → Deployment`

## 🔌 Usage

Configure this repository as a Jenkins Global Pipeline Library and load it in your Jenkinsfile:

```groovy
@Library('Shared') _
```

The reusable functions inside `vars/` can then be called from Jenkins pipeline stages.

## 🎯 Purpose

This project demonstrates reusable CI/CD automation using Jenkins Shared Libraries, with integrated code-quality and security scanning.
