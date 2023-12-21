## VCS Use and Management Report

---

#### Difficulties and challenges during development
During the MusoPlan development stage, learning to use GitHub as distributed version control system can be challenging. It involves understanding the concepts such as branches, commits, push/pull, merging, and other operations related to managing the VCS. When merging branches, it is always necessary to make sure that there are no conflicts in the codes and may require a proficient understanding of it. Working alone in a project may have less conflicts in your files. Assuming that VCS are designed with collaboration in mind, it means that the team should have efficient communications to avoid conflicts in the main repository.
#### Organisational requirements compliance
To ensure compliance with the organisational requirements, the following steps are made:
- Version Control Systems
  - GitHub is used to serve as the distributed version control system for this software project. Contributors are given links to reference material on how to operate Git using terminal and the web.
  - Feature branch is created prior to the start of creating the class, function, and software files. This branch is used to contain such files before merging it to the main branch upon completion.
  - Commit message are relevant to the updates being pushed to the remote repository.
- Software Development
  - The program is made using JavaScript and operates on the Node.js runtime environment.
  - User manual is provided to serve as a guide on how to operate the program.
  - All functions and classes are verified to work as intended by checking actual output compared to the expected output.
  - Codes are written with brief description.
- Software Testing
  - Jest is used to perform automated test and by using jest coverage to check the areas covered the the testing.
  - Manual testing report are provided to present the test inputs and the comparison between the actual and expected outputs.
  - JUnit xml file is included in the report document.
#### VCS performance verification
- ##### Branches
  To verify that branches are working, switching to the new branch by using *git checkout* are done and verify that it is current indicated in the branch list.
- ##### Stages
  Every updates, files are checked by using *git status*, the adding files to be committed by performing *git add* in the CLI.
- ##### Commits
  This is where the brief description of the update are described as commit message by using *git commit -m \"commit message\"* in prompt.
- ##### Merges
  Prior to merging feature branch to the main branch, it is important to make sure that the branch is ahead and updated to avoid conflicts.
- ##### Push/Pull from local to remote repository
  After staging and committing the files, the remote repository is updated by pushing the updated local files using *git push*. On the other hand, using *git pull* will download latest remote repository to the current local directory.
- ##### Commit log
  This log helps to track and monitor update so the commmit messages that was previously added after every stage are useful to determine the changes done in every update.

#### Integrating changes to main repository from forked repository
  To integrate the update from forked repository, pull request should be done to notify and let the main repository manager check the updates and decide on how to add the updates to it.