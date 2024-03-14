# 1. centralised vs. distributed version control
- No disadvantage if you move from Central to git
- [Gitlab](https://about.gitlab.com/blog/2020/11/19/move-to-distributed-vcs/)
- [Atlassin](https://www.atlassian.com/blog/software-teams/version-control-centralized-dvcs)

# 2. How to Synchronize Local and Remote Repositories
To synchronize our local and remote repositories, we first fetch the change history from the remote repository and merge it into our local repository using the pull command. Then we push our local change history to the remote repository using the push command.
- https://www.freecodecamp.org/news/create-and-sync-git-and-github-repositories

# 3. Changeset 
[Azure Repo - TFVC](https://learn.microsoft.com/en-us/azure/devops/repos/tfvc/find-view-changesets?view=azure-devops)
- [changesset - github](https://davistobias.com/articles/adding-changeset/)
- it is not in git 

# Branching for release management and maintenance
![](https://miro.medium.com/v2/resize:fit:828/format:webp/0*G2z5FjDvIsQRfKvM.png)
- [Branching Strategies](https://medium.com/@selvamraju007/git-branching-strategies-a6eafe4541ae)
- HotFIx: They arise from the necessity to act immediately upon an undesired state of a live production version. When a critical bug in a production version must be resolved immediately, a hotfix branch may be branched off from the corresponding tag on the master branch that marks the production version.
- ## [MUST-CHECK](https://dev.to/zigrazor/git-hotfix-branches-the-final-guide-1mll)

# Resolving multi-user conflicts
[Admin needs to Edit manually - what to keep ](https://sentry.io/answers/resolve-merge-conflicts-in-git/)

--------------------------------------------------------------------------
## Visual Studio Team Explorer - Just like Vs Code 
[MS Docs](https://learn.microsoft.com/en-us/azure/devops/user-guide/work-team-explorer?view=azure-devops)


# [DOUBT - NEED RE_CHECK]
### Now TFVC is Outdated amd Windows Explorer = File Explorer
[MS DOCS](https://learn.microsoft.com/en-us/azure/devops/repos/tfvc/use-source-control-explorer-manage-files-under-version-control?view=azure-devops)
Team Foundation Version Control (TFVC) integration with Windows Explorer allows you to seamlessly interact with your TFVC repositories directly from the Windows File Explorer interface. Here's how you can set it up:

1. **Install Visual Studio**:
   Ensure you have Visual Studio installed on your machine. TFVC integration typically comes with Visual Studio installation.

2. **Team Explorer**:
   Open Visual Studio and navigate to the "Team Explorer" tab. If you don't see it, you can find it under the "View" menu.

3. **Connect to Your Repository**:
   - Click on the "Connect" button in Team Explorer.
   - Choose "Manage Connections" and then "Connect to a Project."
   - Enter the URL of your TFVC repository and authenticate if required.

4. **Map a Workspace**:
   - Once connected, you need to map a workspace to a local directory on your machine.
   - In the Team Explorer, under the "Home" tab, select "Source Control Explorer."
   - Right-click on the folder where you want to map your repository and choose "Map."
   - Follow the prompts to map the workspace.

5. **Access from Windows Explorer**:
   - Once you've mapped your workspace, you can access it from Windows Explorer.
   - Navigate to the directory you've mapped your repository to.
   - You should see your TFVC repository files and folders here.
   - You can perform standard file operations like add, edit, delete, and check-in directly from Windows Explorer.

6. **Additional Tips**:
   - Ensure you have the necessary permissions to access the TFVC repository.
   - Make sure you're using an account that has access to the repository.
   - Keep Visual Studio updated to ensure compatibility and access to the latest features.

By following these steps, you can seamlessly integrate TFVC with Windows Explorer and manage your source control operations directly from your file system.

# 6. CI

# 7. Monitor 
[Query Backlog](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/filter-backlogs-boards-plans?view=azure-devops)
[Kanban boards](https://learn.microsoft.com/en-us/devops/plan/what-is-kanban)
[Tarck Bugs](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/manage-bugs?view=azure-devops)
