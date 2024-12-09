# .github

This repository contains organization-wide configurations and templates for JLU Software team. It provides default community health files, templates, and workflows that are shared across all repositories in the organization.

## 📂 Repository Structure

```plaintext
.github/
├── CODE_OF_CONDUCT.md      # Code of Conduct
├── CODEOWNERS              # Default code owners
├── CONTRIBUTING.md         # Organization-wide contributing guidelines (English)
├── CONTRIBUTING_CN.md      # Organization-wide contributing guidelines (Chinese)
├── FUNDING.yml            # Sponsorship configuration
├── workflow-templates/    # Reusable workflow templates
│   ├── python-project.yml
│   └── cpp-project.yml
├── workflows/            # Organization-level workflows
│   ├── python-package.yml
│   └── dependency-review.yml
├── actions/             # Custom actions
│   ├── python-lint/
│   └── build-docs/
└── profile/            # Organization profile
    └── README.md       # Public organization profile
```

## 🔍 What's Inside

### Community Health Files

Default files used across all repositories in the organization:

- Contributing Guidelines (English & Chinese)
- Code of Conduct
- Workflows
- Funding Configuration
- // Code Owners

### Workflow Templates

Ready-to-use GitHub Actions workflows for:

- Python Projects
- C++ Projects
- Documentation Building
- Code Linting & Testing

### Custom Actions

Reusable actions for common tasks:

- Python Code Linting
- Documentation Building

## 🛠️ Usage

### For Repository Maintainers

1. When creating new workflows, check the workflow templates in Actions tab
2. Reference custom actions in your workflows using:

   ```yaml
   - uses: ./.github/actions/python-lint
   ```

3. Follow the contributing guidelines for consistency
4. Help us improve these configurations by opening issues or PRs

### For Contributors

1. Read through CONTRIBUTING.md before making contributions
2. Use provided issue and PR templates
3. Check workflow templates when setting up new projects

## 📝 Notes

- These configurations serve as defaults and can be overridden by individual repositories
- Workflow templates are available in the "Actions" tab when creating new workflows
- Custom actions can be referenced from any repository in the organization

## 🔄 Maintenance

This repository is maintained by the JLU Software team. If you have suggestions for improvements:

1. Open an issue to discuss the proposed changes
2. Submit a PR with updates
3. Ensure documentation is updated accordingly

## 📮 Contact

- [Team Discussion Board](https://github.com/orgs/SoftwareTarsgo/discussions)
- Email: [tarsgosoftware@outlook.com](mailto:tarsgosoftware@outlook.com)
