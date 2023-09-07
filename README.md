## CI/CD Workflow for React SSR

This GitHub Actions workflow automates the continuous integration and deployment of our React SSR application to an AWS S3 bucket. It triggers on pushes to the "master" branch and performs the following steps:

- **Checkout**: This step checks out your repository's code.
- **Configure AWS Credentials**: This step configures AWS credentials to access the S3 bucket.
- **Deploy static site to S3 bucket**: This step synchronizes the contents of the repository with the S3 bucket.

### Prerequisites

- AWS credentials with appropriate permissions.
- An S3 bucket named "techdome" in the "us-south-1" region.
- AWS CLI installed and configured on the runner machine.

### Usage

1. Fork or clone this repository.
2. Set up the required secrets in your GitHub repository settings (`AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`).
3. Make changes to your React SSR project.
4. Push changes to the "master" branch to trigger the workflow.

For more details, see the [GitHub Actions workflow file](https://github.com/pathakanuj24/react-ssr/blob/master/.github/workflows/ci-cd.yml).

