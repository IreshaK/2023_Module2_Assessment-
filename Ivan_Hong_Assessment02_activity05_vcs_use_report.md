# MusoPlan GitHub VCS Use Report

## Difficulties or Challenges During Development

### Technical Glitches

The initial stages of setting up MusoPlan on GitHub encountered technical glitches during VCS initialization. The issues were resolved through a combination of careful configuration and troubleshooting. Online resources and GitHub documentation played a crucial role in ensuring a smooth start.

## Conflict Resolution

### Scenario 1: Direct Overwrite Conflict

In this scenario, I made changes to a file in my local repository and tried to push these changes to the remote repository. However, the same file in the remote repository had been modified directly on GitHub. Git flagged this as a conflict because it didn't know which changes to prioritize.

To resolve this conflict, I performed the following steps:

1. Stashed my local changes using `git stash`.
2. Ran `git pull` to fetch and merge the changes from the remote repository.
3. Applied my stashed changes using `git stash pop`. This brought back my local changes and if there were any conflicts, Git marked the conflicting areas in the file.
4. Reviewed the changes and decided which ones to keep.
5. Edited the file to resolve the conflict, then saved the file.
6. Ran `git add` to stage the resolved file for commit.
7. Committed the resolution with `git commit`.
8. Finally, pushed the resolved changes back to the remote repository with `git push`.

### Scenario 2: Non-overlapping Changes

In this scenario, I added "a" to a file in my local repository, and "b" was added to the same file in the remote repository. However, "a" and "b" were added to different parts of the file that do not overlap.

When I ran `git pull`, Git was able to automatically merge these changes. The result was a file that includes both "a" and "b". This demonstrates how Git can merge non-conflicting changes from the remote repository into the local repository.

## Learning Curve

Adapting to GitHub's specific workflow and branching strategies presented a learning curve. This challenge was overcome through an exhaustive exploration of GitHub documentation and leveraging online resources. This approach facilitated a better understanding and implementation of effective strategies.

<br/>

## Compliance with Organisational Requirements

Ensuring compliance with organizational requirements was pivotal to MusoPlan's development on GitHub.

### Feature Branch Commitment

Adhering to organizational best practices, all development work occurred on feature branches. This commitment maintained a clean version history, making it easier to track changes and isolate features during the development process.

### Clear Commit Messages

Commit messages adhered to industry standards, using the present tense and imperative mood. Each commit included a concise description of the specific change made, enhancing the clarity of the version history for better project understanding.

### Author Information

GitHub was configured to include the author's name and email address with each commit. This practice ensured proper attribution of changes, contributing to accountability throughout the development process.

<br/>

## Verification of GitHub Behaviours

Thorough testing was conducted to validate various GitHub functionalities.

### Branching

Creating feature branches and switching between them underwent rigorous testing to ensure effective isolation. It was verified that changes made in one branch did not impact others, maintaining a structured development environment.

### Staging and Commits

GitHub's staging of changes and committing to the version history were repeatedly tested. This ensured that only intended changes were included in each commit, maintaining a logical progression of the codebase.

### Merging and Conflict Resolution

GitHub's merging capabilities, especially conflict resolution during merges, underwent extensive testing. Simulated scenarios involving making concurrent changes were employed to ensure smooth conflict resolution.

### Push/Pull and Remote Handling

The process of pushing and pulling changes to and from remotes was validated on GitHub. This involved confirming accurate remote repository updates and synchronization of changes.

### Pull Requests

Pull requests, designed for collaboration, were tested for their effectiveness in reviewing and merging changes. Even in a solo project, the practice of reviewing changes before merging was maintained for consistency and documentation purposes.

<br/>

## Integration of Changes to Central Repository

While MusoPlan was not forked from another repository, a hypothetical integration approach was considered.

### Pull Requests for Integration

If the repository were forked, changes would be proposed back to the central repository using pull requests. This involves submitting a request for the integration of changes, accompanied by a clear description of the modifications made.

### Communication

Effective communication with the maintainers of the central repository on GitHub would be established. This ensures transparency about proposed changes and facilitates a smooth integration process.

### Testing in Isolation

Before submitting changes for integration, thorough testing would be conducted in isolation to guarantee that the modifications meet the project's quality standards.

<br/>

## Overall Reflection

The use of GitHub significantly impacted the development process. It improved collaboration, maintained a clean version history, and provided a systematic approach to feature development. Adhering to organizational requirements ensured consistency and accountability throughout the project's lifecycle on GitHub.
