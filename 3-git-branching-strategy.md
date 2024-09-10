# TOC
1

## Common Git Cmds - 
Here is a list of the top 10 Git commands that I use daily in my work:

- 💫 git clone: Clone a repository into a new directory.
- 💫 git status: Show the working tree status.
- 💫 git add: Add file contents to the local staging area.
- 💫 git commit: Record changes to the repository.
- 💫 git push: Update remote refs along with associated objects.
- 💫 git pull: Fetch from and integrate with another repository or a local branch.
- 💫 git checkout: Switch branches or restore working tree files.
- 💫 git branch: List, create, or delete branches.
- 💫 git merge: Join two or more development histories together.
- 💫 git log: Show commit logs.
- 💫 git rebase: allows you to move or combine a sequence of commits to a new base commit. It is often used to maintain a clean and linear project history

𝟭. 𝗴𝗶𝘁 𝗺𝗲𝗿𝗴𝗲 𝘃𝘀 𝗴𝗶𝘁 𝗿𝗲𝗯𝗮𝘀𝗲:
- 𝘨𝘪𝘵 𝘮𝘦𝘳𝘨𝘦 combines branch changes with new merge commits
- 𝘨𝘪𝘵 𝘳𝘦𝘣𝘢𝘴𝘦 moves branch changes on top, creating a linear history

𝟮. 𝗴𝗶𝘁 𝗿𝗲𝘀𝗲𝘁 𝘃𝘀 𝗴𝗶𝘁 𝗿𝗲𝘃𝗲𝗿𝘁:
- 𝘨𝘪𝘵 𝘳𝘦𝘴𝘦𝘵 undoes changes and moves the branch pointer, discarding subsequent commits
- 𝘨𝘪𝘵 𝘳𝘦𝘷𝘦𝘳𝘵 creates new undo commits, preserving history

𝟯. 𝗴𝗶𝘁 𝗳𝗲𝘁𝗰𝗵 𝘃𝘀 𝗴𝗶𝘁 𝗽𝘂𝗹𝗹:
- 𝘨𝘪𝘵 𝘧𝘦𝘵𝘤𝘩 downloads remote changes without auto-merging
- 𝘨𝘪𝘵 𝘱𝘶𝘭𝘭 fetches and auto-merges remote changes

![image](https://github.com/user-attachments/assets/ddc507cd-3bbf-4af1-b097-5b0daec53eb9)

  > However, it's crucial to exercise caution while executing certain commands, such as git revert versus git reset. The first question to ask is whether the commit is public (i.e., pushed to a remote server like GitHub). If it's public, then revert should be used; otherwise, reset is appropriate. Moreover, if any sensitive information is accidentally pushed, a different approach is necessary. Since GitHub doesn't support pre-commit actions, using post-commit actions like git filter-branch or tools like bfg may be required or use scanning solution like synk.
Similarly, deciding between merge vs rebase depends on the team's workflow. Some teams prefer not to rewrite commit history, while others may use rebase in interactive mode to squash or edit commits. Additionally, GitHub now supports ort base merge, resulting in new commits for each merge, while locally, fast forward merge can be performed. As a result, all these tools are highly opinionated based on the team's practices.

[Branching Strategy in GIT](https://medium.com/@dmosyan/version-control-branching-strategies-e68e8d5ef1e0)

## Trunk Based 
Trunk based branching strategy

Trunk-based development is a branching strategy where developers work on a single branch, often called the "trunk" or "main" branch. In this strategy there is a continuous integration and frequent commits to the main branch, promoting collaboration and reducing the complexity of merging changes.

- 🔶 Main Branch:
All developers commit their changes directly to the main branch. The main branch is always in a deployable state.
- 🔶 Short-Lived Feature Branches:
If feature branches are used, they are short-lived and merged back into the main branch quickly. Feature branches are typically used for very short-term work, such as a few hours to a couple of days.
- 🔶 Continuous Integration:
Developers integrate their changes frequently, often multiple times a day.
Automated tests and builds are run on each commit to ensure the main branch remains stable.
- 🔶 Feature Flags:
Feature flags (or toggles) are used to enable or disable features in the codebase. This allows incomplete features to be merged into the main branch without affecting the production environment.

- 💠Workflow:
Developers will pull the latest changes from the main branch, make changes and commit frequently to the main branch and push changes to the remote repository. They create a short-lived feature branch which are created from the main branch for specific tasks and work on the them and commit and push the changes to the remote repository and merge the feature branch back into the main branch as soon as possible.
![image](https://github.com/user-attachments/assets/d194db80-2ad7-4689-8909-5b7e7a7b6ad5)

## Git Flow 
Git Flow is a branching strategy designed to streamline the development process and ensure code quality. It is widely used in software development projects and the detailed explanation is below:

- 🔶 main branch:
This branch contains which is production-ready code means only stable and tested code is merged into this branch. Release are tagged in this branch.
- 🔶 develop branch:
This is the branch in which all the developers push their code and it acts as a staging area for all new code before it is merged into main.
- 🔶 feature/* branch:
This is used for developing new features by developers and it is created from the develop and merged to develop branch once done.
- 🔶 release/*:
This is the branch in which the code sits before the new release and it is created from the develop and merged to main. Allows for minor bug fixes and preparing meta-data for a release.
- 🔶hotfix/*:
This is used for critical fixes in production. It is created from the main and merged back into both main and develop after the fix.

![image](https://github.com/user-attachments/assets/e0b4cb2a-ceec-4ec9-bdf3-5d2307895a74)

--
## What are some popular deployment strategies used in CI/CD pipelines?

- 🔮 Rolling Deployment: Incrementally replaces instances of the previous version of an application with the new version without downtime.

- 🔮 Blue-Green Deployment: Involves two identical environments, one hosting the current version (blue) and the other hosting the new version (green). Traffic is switched from blue to green once the new version is ready.

- 🔮 Canary Deployment: Releases the new version to a small subset of users before rolling it out to the entire user base. This strategy allows for testing in production with real users and workloads.

- 🔮 A/B Testing: Similar to canary deployments but specifically targets testing new features or changes among different user segments to compare performance.

- 🔮 Feature Toggles (Feature Flags): Allows teams to enable or disable features in the application without deploying new code. This facilitates testing and gradual rollout of new features.

--------------

## SAST and DAST

🔶 SAST (Static Application Security Testing) is a white-box testing method that analyzes the source code, byte code, or binary of an application to detect vulnerabilities.
🔹 Analyzes code for vulnerabilities during development.
🔹 Integrate tools like SonarQube or Checkmarx in your CI to catch issues early.


🔶 DAST(Dynamic Application Security Testing) is a black-box testing method that tests the running application for vulnerabilities.
🔹Tests the running application for security flaws.
🔹 Use tools like OWASP ZAP or Burp Suite or Fortify after deployment to staging.

❓Why Use Both
SAST finds issues early in the code. DAST detects vulnerabilities in the live application. By combining SAST and DAST, you can catch and fix security issues throughout the development lifecycle, ensuring a more secure application.

## CodeQL

CodeQL is an advanced code analysis tool built by GitHub. It is code as data, which means allowing developers to write queries that identify patterns and potential vulnerabilities within the codebase. CodeQL basically turns your code into a large database that you can query to perform exhaustive semantic analyses. It checks for security vulnerabilities, bugs, and helps enforce coding standards across variety of programming languages. 

By treating code as data and querying it to find patterns that could indicate security flaws, CodeQL helps developers secure their applications in the development phase, aligning with the principles of SAST.
> In practice, many organizations use both tools complementarily: SonarQube for ongoing code quality monitoring and CodeQL for deeper, security-focused analysis, especially in security-critical projects.
