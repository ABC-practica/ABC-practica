# Contributing

Thank you for contributing to our applications! This guide outlines the process for proposing code changes, creating branches, testing, and submitting pull requests.

---

## Table of Contents

- [Raising an Issue](#raising-an-issue)
- [Assigning Issues](#assigning-issues)
- [Notifications](#notifications)
- [Creating a Branch](#creating-a-branch)
- [Testing Changes](#testing-changes)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Code Review](#code-review)
- [Merging](#merging)

---

## Raising an Issue

All proposed code changes should start with an issue in the repository.

### Issue Types

- **Bug Report:** A bug or unexpected behavior in the application
- **Feature Request:** A new feature or enhancement to existing functionality
- **Documentation:** Improvements to code documentation or README files

### Creating an Issue

1. Navigate to the **Issues** tab in the repository on GitHub
2. Click **New Issue**
3. Select the appropriate issue template (Bug Report, Feature Request, or Documentation)
4. Fill in the following:
   - **Title:** Clear, concise description of the issue
   - **Description:** Detailed explanation including:
     - What is the problem or proposal?
     - Current behavior (for bugs) or desired behavior (for features)
     - Steps to reproduce (for bugs)
     - Relevant context or screenshots
   - **Labels:** Tag the issue (e.g., `bug`, `feature`, `enhancement`, `documentation`)
   - **Priority:** Mark as low, medium, or high

---

## Assigning Issues

### Self-Assignment

If you plan to work on an issue:

1. Open the issue
2. Click **Assignees** on the right panel
3. Select yourself from the dropdown
4. Click **Assign**

### Assigning to Others

If you want someone else to work on the issue:

1. Open the issue
2. Click **Assignees** on the right panel
3. Search for and select the team member's name
4. Click **Assign**

---

## Notifications

### GitHub Notifications

- **Automatic:** Being assigned to an issue or pull request automatically sends a GitHub notification
- **Configure notifications:** Go to your GitHub settings → Notifications to adjust frequency and channels

### Microsoft Teams Direct Messages

To notify a team member about an issue or assignment:

1. Open Microsoft Teams
2. Search for the team member's name or click **New chat**
3. Send them a direct message with:
   - Link to the issue: `https://github.com/organization/app-name/issues/123`
   - Brief summary of what you're assigning them
   - Any urgent context or deadlines

**Example message:**
```
Hey! I've assigned you to issue #123: Add dark mode toggle. 
Please take a look when you get a chance. It's marked as high priority.
```

---

## Creating a Branch

Once an issue is assigned to you, create a feature branch for your work.

### Naming Convention

Use the following format: `feature/issue-number-short-description` or `fix/issue-number-short-description`

**Examples:**
- `feature/123-add-dark-mode-toggle`
- `fix/456-resolve-button-alignment`
- `docs/789-update-readme`

### Steps

1. Clone the repository (if you haven't already):
   ```bash
   git clone https://github.com/organization/app-name.git
   cd app-name
   ```

2. Update your local main branch:
   ```bash
   git checkout main
   git pull origin main
   ```

3. Create a new branch:
   ```bash
   git checkout -b feature/issue-number-description
   ```

4. Make your changes and commit with clear messages:
   ```bash
   git commit -m "Issue #123: Add dark mode toggle functionality"
   ```

5. Push your branch to the repository:
   ```bash
   git push origin feature/issue-number-description
   ```

---

## Testing Changes

Before submitting a pull request, thoroughly test your changes.

### Testing Checklist

- [ ] Your changes work as intended and solve the issue
- [ ] Test across different browsers and devices (mobile, tablet, desktop)
- [ ] Verify no existing functionality was broken (regression testing)
- [ ] Check that all design tokens are used correctly (no hardcoded colors, spacing, or typography values)
- [ ] Run any automated tests available in the project
- [ ] Verify code formatting and linting passes

### General Testing Process

1. Run the application locally and navigate to the areas affected by your changes
2. Test the feature or fix thoroughly with various inputs and scenarios
3. Check that the application still performs well and there are no new errors or warnings
4. Ensure visual consistency with the design system tokens

---

## Submitting a Pull Request

Once your changes are tested and pushed, create a pull request.

### Steps

1. Navigate to the repository on GitHub
2. You should see a prompt to **Compare & pull request** for your branch—click it
3. Alternatively, click **Pull Requests** → **New Pull Request** and select your branch

### Pull Request Details

Fill in the following information:

- **Title:** Clear description of the changes (e.g., "Add dark mode toggle to settings")
- **Description:** Include:
  - What changes were made?
  - Which issue does this resolve? (Link it: `Fixes #123`)
  - What testing was performed?
  - Any breaking changes or side effects?
  - Screenshots or screen recordings (if applicable)

**Example PR Description:**

```
## Description
Adds a dark mode toggle to the settings panel, allowing users to switch between light and dark themes.

## Fixes
Fixes #123

## Changes
- Added dark mode toggle component to settings
- Updated design token references for dark mode
- Implemented theme switching functionality
- Added tests for toggle functionality

## Testing
- Tested on Chrome, Firefox, Safari
- Tested on mobile (iOS and Android)
- Verified all existing features still work
- Confirmed design tokens are used throughout (no hardcoded values)

## Screenshots
[Attach screenshots showing before/after or new feature]
```

### Assign a Reviewer

1. On the pull request page, click **Reviewers** on the right panel
2. Select one or more team members to review your code
3. Click **Request**

### Notify Reviewers on Teams

Send a Microsoft Teams direct message to your reviewer(s):

```
Hi! I've submitted a PR for issue #123: Add dark mode toggle
Please review when you get a chance: [PR link]
Any questions, let me know!
```

---

## Code Review

Your pull request will be reviewed by one or more team members.

### Reviewer Responsibilities

Reviewers should check:
- Code quality and adherence to style guidelines
- Design token usage (no hardcoded values)
- Test coverage and thoroughness
- Documentation updates
- Potential performance impacts
- Breaking changes

### Author Responsibilities

- Respond to review comments promptly
- Make requested changes on your branch
- Push updates (the PR will auto-update)
- Request re-review once changes are complete

### Review Process

1. Reviewer leaves comments or requests changes
2. Author makes updates and pushes to the same branch
3. Reviewer approves or requests additional changes
4. Once approved, the author or a maintainer merges the PR

---

## Merging

Once your PR is approved:

1. Click **Merge pull request** on the pull request page
2. Select **Squash and merge** (to keep commit history clean) or **Create a merge commit** as per your team's preference
3. Delete the branch after merging (GitHub will prompt you)
4. Close the associated issue if not auto-closed by the PR

### Post-Merge

- Monitor for any issues in the deployed application
- Update related documentation if needed
- Celebrate your contribution! 🎉

---

## Questions?

If you have questions or need help, reach out to the development team on Microsoft Teams or open a discussion in the repository.

Thank you for contributing!
