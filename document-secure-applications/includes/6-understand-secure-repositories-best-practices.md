In this learning unit, you will explore essential practices and tools to secure your code repositories and development workflows. These strategies are critical for AI engineers, developers, DevOps engineers, platform engineers, and solution architects to ensure the integrity and security of their software projects.

## Identify risks in code repositories with secret scanning
Secret scanning is a vital tool for detecting exposed secrets, such as API keys or credentials, in your code repositories. GitHub's secret scanning feature automatically identifies tokens or credentials that have been committed to a repository. Alerts are generated for detected secrets, allowing you to take immediate action to mitigate risks.

- Enable secret scanning for your repository by navigating to **Settings** > **Advanced Security** and selecting **Enable Secret Scanning**.
- Use push protection to proactively block commits containing secrets during the push process.
- Define custom patterns to detect organization-specific secrets not covered by default patterns.

For more information, see [GitHub secret scanning documentation](https://docs.github.com/en/code-security/secret-scanning/introduction/about-secret-scanning).

> [!NOTE]
> Secret scanning is available for all public repositories and private repositories with GitHub Advanced Security.

## Implement branch security policies for secure code management
Branch protection rules help safeguard critical branches from unauthorized changes. These rules enforce security measures such as requiring pull request reviews and restricting who can push changes.

- Configure branch protection rules by navigating to **Settings** > **Branches** in your repository.
- Require pull request approvals before merging changes.
- Enable status checks to ensure all tests pass before merging.
- Restrict who can push directly to protected branches.

These policies ensure that only reviewed and approved changes are integrated into critical branches, reducing the risk of introducing vulnerabilities.

## Secure software supply chains with dependency management best practices
Managing dependencies effectively is crucial to securing your software supply chain. Tools like Dependabot and GitHub's dependency graph provide insights into your project's dependencies and their vulnerabilities.

- Enable Dependabot alerts to receive notifications about vulnerable dependencies.
- Use Dependabot security updates to automatically generate pull requests for fixing vulnerabilities.
- Leverage the dependency review feature to visualize changes to dependencies in pull requests before merging.

For more details, see [GitHub dependency management documentation](https://docs.github.com/en/code-security/supply-chain-security/understanding-your-software-supply-chain/about-dependency-review).

## Embed Zero Trust principles into developer workflows
Zero Trust principles, such as least privilege access and assume breach, are essential for securing the development lifecycle. These principles can be applied from precommit to deployment stages.

- Use role-based access controls (RBAC) to limit access to repositories and resources.
- Regularly audit permissions and remove unnecessary access.
- Monitor and log all activities within your repositories to detect potential breaches.

By embedding these principles, you can minimize the attack surface and enhance the overall security posture of your workflows.

## Harden developer environments with trusted tools and extensions
Securing developer environments involves using verified tools and managing IDE extensions to reduce the attack surface.

- Use trusted IDE extensions and regularly review their permissions.
- Limit access to sensitive resources from development environments.
- Employ containerized development environments to isolate dependencies and configurations.

These practices ensure that your development environment remains secure and resilient against potential threats.