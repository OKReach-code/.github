# 🛠️ Development Guidelines

Welcome to the official development guidelines for our organization.  
Please follow these standards carefully to ensure smooth collaboration, consistent quality, and integration with our project management systems.

---

## 📂 Version Control System
We use **Git** with **GitHub** for source control.

---

## 🐛 Issues
- Every task must be tracked with a **GitHub Issue**.
- Always link:
  - Labels
  - Branches
  - Pull Requests (PRs)
- Helpful resources:
  - [Using Labels and Milestones](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels#applying-a-label)
  - [Creating a Branch for an Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-a-branch-for-an-issue)
  - [Linking a Pull Request to an Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)

---

## 🏷️ Labels
Apply labels correctly on issues and PRs:

| Label         | Meaning |
|:--------------|:--------|
| `bug`         | Unexpected problem or unintended behavior |
| `doc`         | Documentation improvements or additions |
| `enhancement` | New feature requests |
| `help wanted` | Request for help on an issue or PR |
| `question`    | Requires clarification |
| `wontfix`     | Work on issue/PR will not continue |

---

## 🌿 Branch Naming Convention

| Purpose | Naming Example |
|:---|:---|
| Hotfix | `hotfix/fix-login-bug` |
| Feature | `feature/add-user-profile` |
| Documentation | `docs/update-api-guide` |
| Module Development | `dirty/module-login` |

**Notes:**
- **Do not include Monday Item IDs** in the branch name.
- Use clear and descriptive names.

---

## 👥 Repository Owners
- Two repository owners per repo: one from our team and one from yours.
- **Both must approve** PRs before merging into `staging`.
- Responsibilities:
  - Merging to `staging`
  - Assigning issues
  - Enforcing guideline compliance
- **Protected branches**: `staging` and `production`.

---

## 🚀 Deployment
- Staging must be a mirror of production.
- Deployment to production should be automated using GitHub Actions.
- Manual functional testing must be completed on **staging** before merging to **production**.

---

## 🧪 Testing
- Define and document a testing protocol.
- Automate tests where possible (consider GitHub Actions for automated testing pipelines).

---

## 🎨 Formatting & Linting
- Use a **unified code formatter and linter**.
- This avoids unnecessary diff noise and keeps PRs clean.

---

## 🎉 Releases
- Define clear release versions and requirements.
- Use GitHub Releases to manage them.

---

## 📚 Linked Monday.com Tasks
- All PRs **must** be linked to a **Monday.com Item ID**.
- The **Monday Item ID must be included inside the PR description**.
- **Do not include** the Monday Item ID in the branch name.

- CI will **block** any PRs missing a Monday Item ID.
- Monday Item IDs are plain numeric (e.g., `1931962436`), no prefixes needed.

---

## 🛡️ Pull Request Requirements
Every Pull Request must:
- Follow the PR template.
- Include a valid Monday Item ID in the PR description.
- Pass all CI checks (including Monday ID validation).
- Be reviewed and approved by both repository owners.

---

## 📋 Pull Request Template

```markdown
# 🚀 Pull Request Overview

## 📄 Summary
> Short description of what this PR does.

## 🔗 Linked Monday Task
- [x] Monday Item ID: <!-- Example: 1931962436 -->
- [x] Link to Monday Item: [Paste link here](https://yourteam.monday.com/boards/board-id/pulses/item-id)

## 🧪 Testing Instructions
> How to test this PR locally.

## 📸 Screenshots or Evidence (if applicable)

## ✅ PR Checklist
- [ ] Monday Item ID is included in the PR description.
- [ ] All tests pass.
- [ ] Linting and formatting applied.
- [ ] Code is self-reviewed.
- [ ] Documentation updated (if needed).

## 🧹 Reviewer Notes
> (Optional for reviewers.)


# 📬 Contact

For any questions regarding these guidelines, reach out to the DevOps team.
german.ferrando@okreach.ai