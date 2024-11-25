# Welcome to Djangomatic Pro 🚀

Djangomatic Pro is a cutting-edge platform designed to streamline and simplify the development, deployment, and management of advanced applications. This GitHub organization hosts all repositories related to the Djangomatic Pro ecosystem, including the core Django backend API, the Next.js client application, and supporting tools like development templates.

## Summary

Djangomatic Pro offers a comprehensive suite of tools and repositories to facilitate efficient development workflows. Contribute by following our guidelines to ensure high-quality, maintainable code across all projects.

## Repositories

1. **[djangomatic-python-backend](https://github.com/td-automation-team/djangomatic-python-backend.git)**  
    The Django-based backend API that powers the Djangomatic Pro platform. It manages data processing, and integrations with the database.
2. **[djangomatic-next-client](https://github.com/td-automation-team/djangomatic-next-client.git)**  
    A modern Next.js client that interfaces seamlessly with the backend API, delivering an intuitive and efficient user experience.
3. **[template-repo-python](https://github.com/td-automation-team/template-repo-python.git)**  
    A repository template replicating the Django backend environment. Use this template when creating new repositories for Python-based development.

## How to Contribute 🎉

We value clean, maintainable, and scalable code. To ensure a seamless development experience, follow these guidelines when contributing to any repository.

### 1. Forking and Cloning

1. Fork the repository you wish to contribute to.
2. Clone your fork locally:

    ```bash
    git clone https://github.com/td-automation-team/<repository-name>.git
    cd <repository-name>
    ```

### 2. Creating Branches

- Always work on a new branch and use the following naming conventions:
  - **Feature branches:** `feature/<short-description>` (e.g., `feature/add-authentication`)
  - **Bug fixes:** `bugfix/<short-description>` (e.g., `bugfix/fix-login-error`)
  - **Hotfixes:** `hotfix/<short-description>` (e.g., `hotfix/critical-deploy-issue`)

    ```bash
    git checkout -b feature/<short-description>
    ```

### 3. Writing Clean Code

#### For Python (Django Backend)

- **PEP 8 Compliance:** Follow the PEP 8 style guide.
- **Type Annotations:** Use type hints wherever possible.

  ```python
  def fetch_data(user_id: int) -> dict:
        ...
  ```

- **Docstrings:** Use proper docstring conventions for modules, classes, and functions.

  ```python
  """
  Module description: Handles user authentication.
  """
  ```

- **Testing:** Write unit tests using pytest. Place test files under a `/tests` directory, mirroring the project structure.

  Example:

  ```python
  def test_function_name():
        assert func() == expected_output
  ```

#### For TypeScript (Next.js Client)

- **Linting:** Adhere to the configured ESLint rules.
- **Type Safety:** Use TypeScript types and interfaces for better maintainability.

  ```typescript
  interface User {
        id: number;
        name: string;
  }
  ```

- **Component Comments:** Use JSDoc for React components.

  ```typescript
  /**
    * Renders a user profile card.
    * @param props - User data to display.
    */
  ```

- **Testing:** Write tests using Jest or React Testing Library. Place tests in a `__tests__` directory or alongside the component with `.test.tsx`.

### 4. Writing Git Commits

- Keep commit messages concise yet descriptive.
- Use the following format for commit messages:
  - **Feature addition:** `feat: add feature description`
  - **Bug fix:** `fix: resolve issue description`
  - **Refactor:** `refactor: update/refactor logic`
  - **Documentation:** `docs: update README`
  - **Testing:** `test: add/remove tests for xyz`

    Example:

    ```bash
    git commit -m "feat: implement JWT-based authentication"
    ```

### 5. Opening a Pull Request (PR)

1. Push your branch to your fork:

    ```bash
    git push origin feature/<short-description>
    ```

2. Open a PR from your branch to the main repository’s `dev` branch (not `main` unless for hotfixes).
3. **PR Title:** Clearly describe the changes (e.g., Add user authentication flow).
4. **PR Description:** Include:
    - What was changed
    - Why it was changed
    - How to test the changes
5. Ensure your PR has been tested locally and passes CI checks.

### 6. Code Reviews

- Be open to feedback and constructive criticism.
- Address requested changes promptly.

### 7. Testing and CI/CD

- Tests are run automatically with GitHub Actions. Ensure you run all tests locally before pushing changes:

  ```bash
  pytest  # for Python
  npm test  # for Next.js
  ```

- Ensure your branch passes all CI checks before requesting a merge.

## Using GitHub Effectively 🛠️

### Issues

- **Bug Reports:** Use the issue template to report bugs. Provide a clear title, description, and steps to reproduce.
- **Feature Requests:** Outline the problem, proposed solution, and potential alternatives.

### Discussions

Use GitHub Discussions for non-critical topics like brainstorming, questions, and team updates.

## Best Practices 🌟

- **Documentation:** Maintain clear and thorough documentation in the codebase and README files.
- **Comments:** Explain complex logic, but avoid over-commenting obvious code.
- **DRY Principle:** Avoid duplicating code. Create reusable functions and components where applicable.
- **Modular Design:** Break large features into smaller, reusable modules.

Welcome to the team!
