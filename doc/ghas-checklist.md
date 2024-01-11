# Secrets scanning checklist

* [ ] Enable Secrets Scanning - See [Configure secrets scan](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/configuring-secret-scanning-for-your-repositories)
* [ ] Enabled Secrets Push Protection - See [Push protection for repositories](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/push-protection-for-repositories-and-organizations)
* [ ] Understand the scanning patterns and limitations of secrets scanning and push protection -  See [Push protection limitations](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/troubleshooting-secret-scanning#push-protection-limitations) and [Secret scanning patterns](https://docs.github.com/en/code-security/secret-scanning/secret-scanning-patterns)
* [ ] Find & manage secret alerts - See [Manage secret alerts](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/managing-alerts-from-secret-scanning)
* [ ] Try to push a secret with push protection enabled - See [Using secret as a push protection on the command line](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/push-protection-for-repositories-and-organizations#using-secret-scanning-as-a-push-protection-from-the-command-line)
* [ ] Create a custom secret scanning pattern - [See Define Custom Patterns](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/defining-custom-patterns-for-secret-scanning). This requires an enterprise license.
* [ ] Create an exclude pattern for files and folders - See [Excluding directories from secrets scanning alerts for users](https://docs.github.com/en/enterprise-cloud@latest/code-security/secret-scanning/configuring-secret-scanning-for-your-repositories#excluding-directories-from-secret-scanning-alerts-for-users)


# Dependabot alerts checklist

* [ ] Enable Dependabot alerts - See [Configuring Dependabot Alerts](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-alerts/configuring-dependabot-alerts)
* [ ] Configure Dependabot custom rules
* [ ] Enable Dependabot Security Updates - See [Configuring Dependabot Security Updates](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-security-updates/configuring-dependabot-security-updates)
* [ ] Enable Dependabot Grouped Security Updates (Beta)
* [ ] Configure Dependabot version updates - See [Configuring Dependabot version updates](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-version-updates/configuring-dependabot-version-updates)
* [ ] Configure Dependabot Notifications - See [Configure notifications for Dependabot alerts](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-alerts/configuring-notifications-for-dependabot-alerts)
* [ ] Review the Dependency Graph and export an SBOM - See [Viewing the Dependency Graph](https://docs.github.com/en/enterprise-cloud@latest/code-security/supply-chain-security/understanding-your-software-supply-chain/exploring-the-dependencies-of-a-repository#viewing-the-dependency-graph) and [Export dependencies as SBOM](https://docs.github.com/en/enterprise-cloud@latest/code-security/supply-chain-security/understanding-your-software-supply-chain/exporting-a-software-bill-of-materials-for-your-repository)
* [ ] Review Dependabot alerts and review search facets and filters
* [ ] Review a single alert - See [View Dependabot Alert](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-alerts/viewing-and-updating-dependabot-alerts)
    - [ ] Find related CVE and CWEs
    - [ ] See "All affected repositories"
    - [ ] See related alerts
    - [ ]  Navigate to the related pull request (if present)
    - [ ] Note the dismissal options for a Dependabot alert - See [Dismissing Dependabot Alerts](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/dependabot-alerts/viewing-and-updating-dependabot-alerts#dismissing-dependabot-alerts)
* [ ] Merge a pull request from Dependabot - See [Managing pull requests for dependency updates](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/working-with-dependabot/managing-pull-requests-for-dependency-updates)
    - [ ]  Review the `@dependabot` chat ops options - See [Managing Dependabot pull requests with comment commands](https://docs.github.com/en/enterprise-cloud@latest/code-security/dependabot/working-with-dependabot/managing-pull-requests-for-dependency-updates#managing-dependabot-pull-requests-with-comment-commands)


# Code scanning with CodeQL

* [ ] Enable Code scanning - See [Configuring code scanning](https://docs.github.com/en/enterprise-cloud@latest/code-security/code-scanning/enabling-code-scanning/configuring-default-setup-for-code-scanning)
* [ ] Review the CodeQL workflow
* [ ] Review 3rd party code scanning workflows
* [ ] Review Code scanning alerts
    - [ ] Review search facets and filters
* - Review a single alert
    - [ ] Review severity
    - [ ] Review related CVE/CWEs
    - [ ] Review the source of the CodeQL query
    - [ ] Review sources and sink (Show Paths) - Note, not all alerts will have Show Paths.
    - [ ] Follow the sink to the code line(s) and see the Copilot X icon. Can you get advice on how to fix it?
    - [ ] Note the dismissal options for a Code scanning alert - See [Dismissing code scanning alerts]()
    - [ ] Review summary, descriptions, fixes and references
    - [ ] Review commit history

# Security advisories

* [ ] Create a security advisory - See [About Security Advisory](https://docs.github.com/en/enterprise-cloud@latest/code-security/security-advisories/working-with-repository-security-advisories/about-repository-security-advisories)

# Security policy

* [ ] Review the security policy - See [Adding a security policy to your repository](https://docs.github.com/en/enterprise-cloud@latest/code-security/getting-started/adding-a-security-policy-to-your-repository)

# General

* - [ ] Review branch protection rules - See [Managing a branch protection rule](https://docs.github.com/en/enterprise-cloud@latest/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule)
* - [ ] Review repository permissions - [Managing your repositories teams and people](https://docs.github.com/en/enterprise-cloud@latest/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository)
* - [ ] Review Security Overview (Requires Owner or Admin permission on the Org) - See [About the security overview](https://docs.github.com/en/enterprise-cloud@latest/code-security/security-overview/about-security-overview)
* - [ ] Review API for pull GHAS repo info - See [Code Scanning API](https://docs.github.com/en/enterprise-cloud@latest/rest/reference/code-scanning). See also https://github.com/austimkelly/ghas-utils for org-level insights across multiple repos.