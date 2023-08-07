# GitHub Workflows for Javascript Projects

This repository offers workflow templates tailored for JavaScript projects built with Node.js, leveraging Yarn v3 and Buf, and designed to integrate with various deployment targets via Planton Cloud services.

## Workflow Descriptions

### Buld & Push Docker Image to GCP Artifact Registry

A workflow providing an end-to-end solution for Node.js projects with Yarn v3 and Buf integrations targeting containerized deployments:

1. Checking out code.
2. Installing and setting up the Planton CLI.
3. Exporting the Buf Token.
4. Setting up the Node.js environment with caching and Yarn v3 support.
5. Building the application using Make.
6. Authenticating and logging in to the GCP Artifact Registry.
7. Building and pushing Docker images to the specified registry.

### Deploy Microservice to GKE

This workflow supports the deployment of Node.js applications with Yarn v3 and Buf integrations as microservices on Planton Cloud:

1. Checking out code.
2. Installing and setting up the Planton CLI.
3. Exporting the Buf Token.
4. Setting up the Node.js environment with caching and Yarn v3 support.
5. Building the application using Make.
6. Authenticating and logging in to the GCP Artifact Registry.
7. Building and pushing Docker images.
8. Deploying the microservice to the specified Planton Cloud environment.

## Inputs

Each workflow has its specific inputs for execution. For details on necessary inputs for each workflow, refer to the respective YAML file. For instance, the `build-and-push-docker-image.node.yarnv3.buf.yaml` workflow requires:

- (List of inputs as provided before for this workflow...)

And similarly for `deploy-microservice.node.yarnv3.buf.yaml`:

- (List of inputs as provided before for this workflow...)

## Secrets

Ensure you've set up the necessary secrets in your GitHub repository settings. The required secrets include:

- `PLANTON_CLOUD_CLIENT_EMAIL`
- `PLANTON_CLOUD_CLIENT_SECRET`

## Usage

1. Choose the appropriate workflow from this repository based on your deployment requirements.
2. Add the selected workflow to your project's `.github/workflows` directory.
3. Configure the necessary secrets and inputs in your repository settings.
4. Trigger the workflow as per your CI/CD needs.

## Support

If you encounter any issues or require further assistance, please file an issue in this GitHub repository.

## Contributing

If you have suggestions for how this GitHub Action could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

## License

This project is licensed under the [MIT License](LICENSE).
