Jenkins is an open-source popular CI/CD tool used to automate the pipeline.

It Automate various parts of software development.
.Building
.Testing
.Deploying

* What is CI/CD?
CI (Continuous Integration): A process where developers integrate code changes into a shared repository frequently. This is followed by automated builds and tests to detect issues early.
CD (Continuous Delivery/Deployment): A process where code changes are automatically tested and deployed to production or staging environments, ensuring the application is always in a deployable state.

* Why CI/CD is Important?
- Automates testing, security checks, and deployment, reducing manual effort and errors.
- Ensures faster, more reliable delivery of applications to customers.
- Helps in identifying bugs and vulnerabilities early in the development cycle.

🏗️ CI/CD Workflow
Code Commit → Jenkins Trigger → Build → Test → Docker Build → Deploy

🔁 Flow Explanation
.Developer pushes code to GitHub

.Jenkins pipeline is triggered automatically

.Application is built and tested

.Docker image is created

.Application is deployed on server

🔄 Pipeline Stages
1) Checkout - Pulls code from GitHub repository
2) Build - Builds the application
3) Test - Runs automated tests
4) Docker Build - Builds Docker image
5) Deploy -Runs the application container

🔐 Best Practices
.Store credentials in Jenkins Credentials Manager

.Do not hardcode secrets in pipeline

.Use environment variables

.Enable logging and monitoring

🐞 Troubleshooting

| Issue                  | Fix                          |
| ---------------------- | ---------------------------- |
| Build fails            | Check Jenkins console logs   |
| Docker error           | Verify Docker is running     |
| App not accessible     | Check port (8000) & firewall |
| Pipeline not triggered | Verify GitHub webhook        |


