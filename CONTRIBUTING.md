# Contributing Guide

English | [中文](./CONTRIBUTING_CN.md)

Thank you for considering contributing to JLU Software! This document outlines the guidelines for contributing to our projects.

## Table of Contents

- [Contributing Guide](#contributing-guide)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
  - [Development Process](#development-process)
  - [Pull Request Guidelines](#pull-request-guidelines)
  - [Coding Standards](#coding-standards)
    - [Python](#python)
    - [C++](#c)
    - [JavaScript/TypeScript](#javascripttypescript)
  - [Commit Message Guidelines](#commit-message-guidelines)
  - [Documentation](#documentation)
  - [Testing](#testing)
  - [Issue Guidelines](#issue-guidelines)
    - [Bug Reports](#bug-reports)
    - [Feature Requests](#feature-requests)
  - [Review Process](#review-process)
  - [Questions?](#questions)

## Getting Started

1. Fork the repository
2. Clone your fork:

   ```bash
   git clone https://github.com/your-username/repository-name.git
   ```

3. Add the upstream repository:

   ```bash
   git remote add upstream https://github.com/jlu-software/repository-name.git
   ```

4. Create a new branch for your feature/fix:

   ```bash
   git checkout -b feature/your-feature-name
   ```

## Development Process

1. Keep your branch up to date:

   ```bash
   git pull upstream main
   ```

2. Make your changes in small, logical commits
3. Write tests for your changes
4. Update documentation as needed
5. Run local tests before submitting
6. Push changes to your fork
7. Create a Pull Request from your branch to the main repository

## Pull Request Guidelines

- Fill out the PR template completely
- Link any related issues
- Include screenshots/GIFs for UI changes
- Update relevant documentation
- Add/update tests as needed
- Ensure all CI checks pass
- Request review from relevant team members

## Coding Standards

### Python

- Follow PEP 8 style guide
- Use type hints for function parameters and return values
- Document functions and classes using docstrings
- Maximum line length: 88 characters
- Use black for code formatting

Example:

```python
def calculate_distance(point_a: Tuple[float, float], point_b: Tuple[float, float]) -> float:
    """Calculate Euclidean distance between two points.

    Args:
        point_a: Tuple of (x, y) coordinates for first point
        point_b: Tuple of (x, y) coordinates for second point

    Returns:
        Float value representing the distance between points
    """
    return math.sqrt((point_b[0] - point_a[0])**2 + (point_b[1] - point_a[1])**2)
```

### C++

- Follow Google C++ Style Guide
- Use modern C++ features (C++14 or later)
- Document classes and functions using Doxygen style
- Maximum line length: 100 characters
- Use clang-format for code formatting

### JavaScript/TypeScript

- Follow Airbnb JavaScript Style Guide
- Use ESLint and Prettier for formatting
- Use TypeScript for new features
- Maximum line length: 80 characters

## Commit Message Guidelines

Follow the conventional commits specification:

```plaintext
<type>(<scope>): <description>

[optional body]

[optional footer]
```

Types:

- feat: New feature
- fix: Bug fix
- docs: Documentation changes
- style: Code style changes (formatting, etc)
- refactor: Code refactoring
- test: Adding or updating tests
- chore: Maintenance tasks

Example:

```plaintext
feat(navigation): add path planning algorithm

Implemented A* algorithm for robot path planning.
Added unit tests and documentation.

Closes #123
```

## Documentation

- Document all public APIs
- Keep README.md up to date
- Add comments for complex algorithms
- Include usage examples
- Document setup and deployment procedures

## Testing

- Write unit tests for new features
- Maintain test coverage above 80%
- Include integration tests where necessary
- Test edge cases
- Document test scenarios

## Issue Guidelines

Before creating an issue:

1. Search existing issues
2. Use the issue template
3. Provide clear reproduction steps
4. Include system/environment details
5. Add relevant labels

### Bug Reports

- Describe expected vs actual behavior
- Include steps to reproduce
- Attach screenshots/logs if applicable
- Specify environment details

### Feature Requests

- Clearly describe the problem to solve
- Suggest possible solutions
- Explain benefits
- Consider potential drawbacks

## Review Process

1. Code review required for all changes
2. Changes must pass all CI checks
3. Documentation must be updated
4. Tests must pass
5. Review comments must be addressed

## Questions?

Feel free to ask questions in:

- GitHub Discussions
- Team chat channels
- Developer meetings

Thank you for contributing to JLU Software! 🎉
