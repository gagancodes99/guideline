# Branching Strategy

We use a structured branching model to enusre efficient collaboration and a smooth workflow.

## Main Branches

- **`main` (or `master`)**: This is the production-ready branch. All code here is stable and deployed to production.
- **`development`**: This is the integration branch where all features are merged before being released.

## Supporting Branches 

- **Feature Branches**: Used for developing new features.
  - Naming conventions: `feature/<short-desctiption>` (e.g., `feature/login-page`).
  - Merge into `development` once the feature is complete.

- **Bugfix Branches**: Used for fixing bugs in `develop` or `main`.
  - Naming convention: `bugfix/<short-description>` (e.g., `bugfix/header-crash`).
  - Merge into `develop` or `main`.

- **Release Branches**: Used when preparing for a release from `develop`.
  - Naming convention: `release/<version>` (e.g., `release/1.0.0`).
  - Merge into both `main` and `develop`.

- **Hotfix Branches**: Used for urgent fixes in `main`.
  - Naming convention: `hotfix/<short-description>` (e.g., `hotfix/login-bug`).
  - Merge into both `main` and `develop`.

## Example Workflow


1. **Start a new feature branch**:
   
   git checkout -b feature/add-user-profile

2. **Push the branch and collaborate**:

   git push origin feature/add-user-profile

3. **Merge feature into `development` once complete**:
   
   git checkout develop
   
   git merge feature/add-user-profile

4. **Create a release branch**:
   
   git checkout -b release/1.0.0

5. **Merge release branch into `main` for production**:
   
   git checkout main
   
   git merge release/1.0.0

By following this branching strategy, we ensure that features, fixes, and releases are managed consistently across teams.
