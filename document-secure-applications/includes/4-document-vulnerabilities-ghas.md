GitHub Advanced Security (GHAS) provides tools and features to enhance the security of your code repositories. This learning unit explores how to document vulnerabilities, analyze attack paths, implement secure practices, embed Zero Trust principles, and secure developer environments.

## Document vulnerabilities using GitHub Advanced Security (GHAS)
GitHub Advanced Security offers features like secret scanning and dependency review to identify and document vulnerabilities in your code repositories. Secret scanning detects sensitive information such as API keys or tokens that might have been accidentally committed. Dependency review helps you understand the impact of changes to dependencies, including identifying vulnerable versions before merging pull requests.

- Use secret scanning to detect leaked secrets and receive alerts.
- Leverage dependency review to assess the security implications of dependency updates.

> [!NOTE]
> Secret scanning is enabled by default for public repositories but requires a GHAS license for private repositories.

## Analyze attack paths for exposed secrets in Azure DevOps
Attack path analysis helps identify exploitable paths from exposed secrets to high-impact assets. By integrating GitHub Advanced Security with Azure DevOps, you can run assessments to understand your organization's exposure to secret leaks and take preventive measures.

- Use the "Risk" view in the Security tab to explore repositories affected by secret leaks.
- Filter results to focus on critical vulnerabilities and export data for further analysis.

:::image type="content" source="../media/theme-light.svg" alt-text="Screenshot of the Security risk view for an organization.":::

> [!TIP]
> For detailed steps on configuring GHAS for Azure DevOps, see [Configure GitHub Advanced Security for Azure DevOps](https://learn.microsoft.com/azure/devops/repos/security/configure-github-advanced-security-features).

## Implement secure software supply chain practices
Securing the software supply chain involves managing dependencies, scanning for vulnerabilities, and monitoring open-source components. GitHub's dependency graph and Dependabot alerts provide insights into your project's dependencies and notify you of vulnerabilities.

- Enable Dependabot alerts to receive notifications about vulnerable dependencies.
- Use dependency review to enforce security checks during pull requests.

### Best practices
- Regularly update dependencies to minimize exposure to known vulnerabilities.
- Combine automated tools like Dependabot with manual reviews for comprehensive security.

## Embed Zero Trust principles into your development workflow
Zero Trust principles emphasize verifying every access request and minimizing trust zones. Integrating these principles into your development lifecycle enhances security and collaboration.

- Implement precommit checks to validate code changes.
- Use branch protection rules to enforce review policies and prevent unauthorized changes.

> [!NOTE]
> Zero Trust principles align with GitHub's security features, such as push protection and delegated bypass for sensitive actions.

## Secure developer environments with branch policies and trusted tools
Securing developer environments involves enforcing branch protection rules, limiting access privileges, and using trusted extensions in integrated development environments (IDEs).

- Configure branch protection rules to require pull request reviews before merging.
- Use least privilege access to restrict permissions to only what is necessary.
- Install trusted extensions in IDEs to ensure secure coding practices.

> [!TIP]
> Explore GitHub's [security overview](https://docs.github.com/en/code-security/security-overview/about-security-overview) to monitor and manage security across your repositories.