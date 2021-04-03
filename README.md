# Software Factory Examples

Samples and templates for setting up a secure software factory based on recommendations from the CNCF Supply Chain Security Whitepaper

## What This Repository Includes:
- A model for a base "Build Worker" container (`Dockerfile.sample`)
- An example of how to use a Kubernetes job object as the foundation for your build steps (`base-job.yaml`).
- Examples of how to you might construct a pipeline in each of:
    - Argo
    - Tekton
    - Jenkins
- An example of a terraform script for configuring a secure S3 bucket that can act as the storage repository for either your injested dependencies or your completed artefacts (`secureBucket`)
- Example configurations for major package managers to direct them to use attached, "local" repositories instead of trying to pull from the internet during builds (`packageManagerConfigs`)
- An example of how to do offline signing using Notary (`offlineSigning`)


## See Also

The examples here are meant to be illustrative of the recommendations included in the CNCF SIG-Security Supply Chain Security Whitepaper. They are examples only and must be modified to meet the needs of your organization. We recommend consulting the whitepapper for more details and explanations around each of these examples.

Additionally, check out the [secureGitHub](https://github.com/SorenTech/secure-GitHub) project, which provides a utility for implementing many of the recommendations from the paper for securing your first party source code repositories via the GitHub API.
