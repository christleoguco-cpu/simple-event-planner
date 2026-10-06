# Simple Event Planner

## Project Purpose - Easy Event Organization

The Simple Event Planner is a small application designed to help users organize and manage events.
## Functional Requirements
- FR-01: Create Event
- FR-02: View Events
- FR-03: Update Event
- FR-04: Delete Event

## Team Members
- Christle Ogu - GitHub Username: christleoguco-cpu
- Annette Ndu - GitHub Username: Annettedarlyn

## Git Workflow

Our team used GitHub branches to work on different features without making changes directly to the main project at the same time. Each team member created feature branches and made meaningful commits related to the functional requirements.

The feature branches included work for creating, viewing, updating, and deleting events. After completing the work, pull requests were created and the feature branches were merged into the main branch.

## Merge Conflict Resolution

To demonstrate conflict resolution, both team members changed the Project Purpose heading in README.md differently. One version used "Project Purpose - Event Organization" while the other used "Project Purpose - Easy Event Planning."

GitHub detected a merge conflict because the same line had been changed differently. We reviewed both changes and resolved the conflict by combining them into:

"Project Purpose - Easy Event Organization"

The resolved file was committed and the pull request was successfully merged into the main branch.

## Environment Configuration

The repository contains separate example configuration files for development and production:

- `.env.development.example`
- `.env.production.example`

These files contain placeholder values only. No real passwords, API keys, tokens, or other secrets are stored in the repository.

## Deployment Strategy - Blue-Green Deployment

The Simple Event Planner will use a Blue-Green deployment strategy. The Blue environment will represent the current stable version of the application, while the Green environment will contain the new version being prepared for release.

Before releasing the Green version, the team will test important features such as creating, viewing, updating, and deleting events. If the tests are successful, users will be directed from the Blue environment to the Green environment.

If a serious problem is discovered after deployment, traffic can be switched back to the stable Blue environment. This provides a quick rollback and reduces the risk of releasing a faulty version.
