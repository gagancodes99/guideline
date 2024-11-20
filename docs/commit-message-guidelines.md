# Commit Message Guidelines

This documen describes the standards for writing commit messages in our projects.By following  these guidelines, we ensure a clean,readable, and organized history of commits.

## Commit Message Structure

Every commit message should follow this format:

<type>(scope):<short description>[Optional body][Optional footer(s)]

## Commit Types

|**Type**    |**Description**
|------------|----------------------------------------------------------------------------|
|`feat`      | Introduces a new feature.                                                  |
|`fix`       | Fixes a bug or an issue.                                                   |
|`chore`     | Updates build tasks, package manager configs, or similar non-code changes. |
|`docs`      | Updates documentation.                                                     |
|`style`     | Changes code formatting or style (does not affect functionality).          |
|`refactor`  | Refactors code wiithout adding features or fixing bugs.                    |
|`test`      | Adds or updates tests.                                                     |
|`perf`      | Improves performance.                                                      |
|`ci`        | Changes related to CI/CD configurations.                                   |

## Commit Scope

- The scope should specify the area of the project impacted by the changes (e.g.,`auth`, `api`, `ui`, `notifications`, etc.)

### Commit Description

- Be breif and descriptive (max 50 characters).
- Use the imperative mood (e.g. "Add feature" instead of "Added feature").

### Example Commits

1.**Adding  a Feature**:
feat(auth):add login functionality

2.**Fixing a Bug**:
fix(ui):resolve button alignment issue

3.**Updating Documentation**:
docs(api):Update README with usage examples

### Optional Sections

### Commit Body

- The body should provide firthur context or explain *why* the change was made. Limit to 72 characters per line.

### Footer 

- The footer can include references to issues, breaking changes, or other relevant information.

BREAKING CHANGE:Refactor API endpoints for better consistency.

Resolves:#123

By following these guidelines, we maintain consistency and clarity across all commits.
