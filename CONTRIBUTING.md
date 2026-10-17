# 🤝 Contributing to CampusOne

Thank you for your interest in contributing to **CampusOne — One Campus. One Platform. Infinite Possibilities.**

CampusOne aims to make campus management more accessible, organized, and efficient through modern technology. We welcome contributions that improve functionality, usability, security, accessibility, and documentation.

## 📌 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [Ways to Contribute](#-ways-to-contribute)
- [Getting Started](#-getting-started)
- [Development Workflow](#-development-workflow)
- [Coding Guidelines](#-coding-guidelines)
- [Commit Messages](#-commit-messages)
- [Pull Request Guidelines](#-pull-request-guidelines)
- [Reporting Bugs](#-reporting-bugs)
- [Security Issues](#-security-issues)
- [License](#-license)

## 🌟 Code of Conduct

All contributors are expected to be respectful, professional, inclusive, and constructive.

We do not tolerate harassment, discrimination, personal attacks, or abusive behavior in project discussions.

## 💡 Ways to Contribute

You can help CampusOne by:

- Reporting bugs and unexpected behavior.
- Suggesting new features.
- Improving the user interface and accessibility.
- Developing student, faculty, or administrator modules.
- Improving authentication and authorization.
- Writing tests and improving code quality.
- Updating documentation and setup instructions.
- Reviewing pull requests.

For substantial changes, open an issue first to discuss the proposed solution.

## 🚀 Getting Started

### Prerequisites

Before contributing, make sure you have:

- Node.js compatible with the project dependencies.
- npm.
- Git.
- A GitHub account.
- Access to a development Supabase project, if required.

### 1. Fork the Repository

Fork the official CampusOne repository using GitHub.

### 2. Clone Your Fork

Replace the placeholders with your GitHub username and the actual repository name.

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

### 3. Add the Upstream Repository

```bash
git remote add upstream https://github.com/ORIGINAL-OWNER/ORIGINAL-REPOSITORY.git
```

Replace the URL with the official CampusOne repository URL.

### 4. Install Dependencies

```bash
npm install
```

### 5. Configure Environment Variables

Create a local `.env` file using the project's documented environment variables or `.env.example`.

Never commit real credentials, private keys, database passwords, or production secrets.

### 6. Start Development

```bash
npm run dev
```

Follow the repository README for any additional setup requirements.

## 🔧 Development Workflow

### 1. Sync Your Fork

```bash
git checkout main
git fetch upstream
git merge upstream/main
```

If the repository uses another default branch, replace `main` accordingly.

### 2. Create a Feature Branch

Use a descriptive branch name.

```bash
git checkout -b feature/student-dashboard
```

Other examples:

- `fix/login-validation`
- `docs/setup-guide`
- `feature/attendance-management`
- `test/authentication`

### 3. Make Your Changes

Keep changes focused, readable, and consistent with the existing project architecture.

Avoid unrelated formatting changes or unnecessary dependency additions.

### 4. Run Available Checks

Run the scripts configured in `package.json`. Common examples include:

```bash
npm run build
npm test
```

Only run scripts that exist in the repository. Report any failures clearly.

### 5. Commit Your Changes

```bash
git add .
git commit -m "feat: add student dashboard"
```

### 6. Push Your Branch

```bash
git push origin feature/student-dashboard
```

### 7. Open a Pull Request

Open a pull request against the official repository's default branch. Explain the change, link any related issue, and include screenshots for user-interface changes.

## 🧑‍💻 Coding Guidelines

### TypeScript and React

- Use TypeScript types and interfaces where appropriate.
- Prefer reusable, focused React components.
- Follow existing naming conventions.
- Keep components readable and maintainable.
- Avoid unnecessary dependencies and duplicated logic.
- Handle loading, error, empty, and success states.
- Use semantic HTML and accessible controls.

### UI and Accessibility

- Maintain a consistent visual design.
- Ensure layouts work across desktop and mobile screens.
- Provide appropriate labels for form fields.
- Support keyboard navigation where applicable.
- Use clear feedback messages for user actions.

### Security and Data Access

- Enforce authorization in the backend or database.
- Do not rely solely on hidden buttons or frontend role checks.
- Apply appropriate Supabase Row Level Security policies.
- Validate input and handle errors safely.
- Never expose service-role keys or other privileged secrets in browser code.
- Never include real student records or personal information in commits, screenshots, or test fixtures.

### Database Changes

- Document schema changes.
- Include migration files when the project uses database migrations.
- Consider existing records and backward compatibility.
- Review access policies whenever a table or database function changes.

## 📝 Commit Message Convention

Use clear, descriptive commit messages. The following prefixes are recommended:

| Prefix | Purpose |
|---|---|
| `feat:` | New feature |
| `fix:` | Bug fix |
| `docs:` | Documentation |
| `style:` | Formatting or styling without behavior changes |
| `refactor:` | Code restructuring |
| `test:` | Tests |
| `chore:` | Maintenance tasks |
| `security:` | Security improvements |

Examples:

```text
feat: add faculty dashboard
fix: correct login validation
docs: update installation instructions
test: add authentication tests
security: enforce role permissions
```

## 🔍 Pull Request Guidelines

Before submitting a pull request, confirm that:

- [ ] The change has a clear purpose.
- [ ] The branch is based on the latest relevant code.
- [ ] Existing conventions have been followed.
- [ ] The application builds successfully, where applicable.
- [ ] Relevant tests have been run.
- [ ] No secrets or sensitive personal information are included.
- [ ] Documentation has been updated when needed.
- [ ] UI changes include screenshots where helpful.
- [ ] Database and authorization changes are documented.
- [ ] The pull request describes what changed and why.

Pull requests may receive feedback or require revisions before merging.

## 🐛 Reporting Bugs

When opening a bug report, include:

1. A clear title.
2. A description of the issue.
3. Steps to reproduce it.
4. Expected behavior.
5. Actual behavior.
6. Browser, operating system, or relevant environment details.
7. Sanitized logs or screenshots, if useful.

Please search existing issues before creating a duplicate.

## 💬 Suggesting Features

Feature proposals should explain:

- The problem being addressed.
- The intended users.
- The proposed behavior.
- Potential implementation considerations.
- Security, privacy, and accessibility implications.

Large changes should be discussed before development begins.

## 🔐 Security Issues

Please do not disclose exploitable vulnerabilities, credentials, or sensitive student information in public issues.

Follow the instructions in `SECURITY.md` or contact the project maintainer through an appropriate private channel.

## 📄 License

By contributing, you agree that your contributions will be distributed under the project's **Apache License 2.0**, subject to the applicable license terms.

See the `LICENSE` file for details.

## 🙌 Thank You

Every useful contribution helps improve CampusOne.

Thank you for helping build a better digital campus experience.

**CampusOne — One Campus. One Platform. Infinite Possibilities.**
