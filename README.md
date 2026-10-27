# OpenShift CI/CD Pipeline Project

## Project Description
This project demonstrates a Continuous Integration and Continuous Deployment (CI/CD) pipeline using GitHub Actions, Tekton, and OpenShift. It automates code linting, unit testing, image building, and application deployment.

## Objectives
- Automate code quality checks using Flake8.
- Execute unit tests using Nose.
- Define pipeline tasks using Tekton.
- Build container images using Buildah.
- Deploy the application on OpenShift.
- Verify application availability on port 8000.

## Technologies Used
- GitHub
- GitHub Actions
- Python
- Flake8
- Nose
- Tekton Pipelines
- Buildah
- Red Hat OpenShift
- YAML

## Project Structure
```text
openshift-cicd-project/
├── README.md
├── oc-pipeline-application-logs.txt
├── .github/
│   └── workflows/
│       └── workflow.yml
└── .tekton/
    └── tasks.yml
```

## Pipeline Steps
1. **Cleanup:** Prepares the pipeline workspace.
2. **Git Clone:** Retrieves the source code from the repository.
3. **Lint:** Checks Python code quality using Flake8.
4. **Unit Tests:** Runs automated tests using Nose.
5. **Buildah:** Builds the application container image.
6. **Deploy:** Deploys the application to OpenShift.

## Application Details
The application is configured to listen on port `8000`. Application logs can be used to verify startup and service availability.

Expected log message:
`SERVICERUNNING`

## Execution
1. Push the project files to a public GitHub repository.
2. Run the GitHub Actions workflow.
3. Configure Tekton tasks and the pipeline in OpenShift.
4. Execute the pipeline and inspect each task's status.
5. Verify the deployed application and its logs.

## Expected Outcome
The pipeline should complete linting, unit testing, image building, and deployment successfully. The deployed application should become accessible on its configured port.

## Author
Student Project

## Conclusion
This project demonstrates how CI/CD automation can improve code quality, testing consistency, container image creation, and application deployment using GitHub and OpenShift.
