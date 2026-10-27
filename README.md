# ci-cd-final-project

## Project Description

The **ci-cd-final-project** demonstrates a Continuous Integration and Continuous Deployment (CI/CD) workflow using GitHub Actions, Tekton Pipelines, and Red Hat OpenShift. The project automates code linting, unit testing, container image building, and application deployment.

## Objectives

- Automate code quality checks using Flake8.
- Execute unit tests using Nose.
- Configure automated workflows using GitHub Actions.
- Define pipeline tasks using Tekton.
- Build container images using Buildah.
- Deploy the application on OpenShift.
- Verify application startup and availability on port 8000.

## Technologies Used

- GitHub and GitHub Actions
- Python
- Flake8
- Nose
- Tekton Pipelines
- Buildah
- Red Hat OpenShift
- YAML
- Docker and container technology

## Project Structure

```text
ci-cd-final-project/
├── README.md
├── oc-pipeline-application-logs.txt
├── cicd-github-validate
├── .github/
│   └── workflows/
│       └── workflow.yml
└── .tekton/
    └── tasks.yml
```

## CI/CD Pipeline Steps

1. **Cleanup:** Prepares the workspace for pipeline execution.
2. **Git Clone:** Retrieves the project source code from the GitHub repository.
3. **Linting:** Checks Python source code quality using Flake8.
4. **Unit Testing:** Executes automated tests using Nose.
5. **Buildah:** Builds the application container image.
6. **Deploy:** Deploys the application to the OpenShift environment.

## GitHub Actions Workflow

The GitHub Actions workflow is defined in `.github/workflows/workflow.yml`.

The workflow is intended to:
- Check out the source code.
- Set up the required runtime environment.
- Install project
