# Explaion SDLC 
# DevOps Server
[Azure DevOps Express vs Azure DevOps Server](https://learn.microsoft.com/en-us/azure/devops/server/download/azuredevopsserver?view=azure-devops)
- Azure DevOps Server Express is free, simple to set up on both client and server operating systems, and supports all the same features as Azure DevOps Server. The `only difference` is that it is limited by licensing agreements to `five or fewer active users`.
- [Azure Devops service vs Server](https://learn.microsoft.com/en-us/azure/devops/user-guide/about-azure-devops-services-tfs?view=azure-devops)
- [install azure devops server](https://learn.microsoft.com/en-us/azure/devops/server/install/get-started?view=azure-devops-2022&viewFallbackFrom=azure-devops)
- [DevOps sever administrative console](https://learn.microsoft.com/en-us/azure/devops/server/admin/open-admin-console?view=azure-devops-2022)
- [Collections - DevOps server](https://learn.microsoft.com/en-us/azure/devops/server/admin/manage-project-collections?view=azure-devops-2022)
- [permissions](https://learn.microsoft.com/en-us/azure/devops/organizations/security/about-permissions?view=azure-devops-2022&tabs=preview-page)

# Azure Boards - 3 and 4 
- [Process template](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=agile-process)
- [Customize a process template](https://learn.microsoft.com/en-us/azure/devops/reference/process-templates/customize-process?view=azure-devops)
- [Upload or download a process template](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/guidance/manage-process-templates?toc=%2Fazure%2Fdevops%2Freference%2Ftoc.json&view=azure-devops)
- EXPLAIN WORK ITEMS EPIC USER STORY
- SPRINT BASICS
- [Backlogs - Agile](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/backlogs-overview?view=azure-devops)
- [Sprits - scrum](https://learn.microsoft.com/en-us/azure/devops/boards/sprints/scrum-overview?view=azure-devops)
- [Team collaboration](https://learn.microsoft.com/en-us/azure/devops/organizations/settings/add-teams?view=azure-devops&tabs=preview-page)
- [ Monitoring team progress ](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/configure-sprint-burndown?toc=%2Fazure%2Fdevops%2Fboards%2Ftoc.json&view=azure-devops&tabs=remaining-work%2Cmay)
- https://learn.microsoft.com/en-us/azure/devops/organizations/settings/add-teams?view=azure-devops&tabs=preview-page
  

> if you prioritize a comprehensive set of DevOps tools for software development and delivery, Azure DevOps might be the right choice. However, if your focus is on project management and agile methodologies, Jira can be the better fit.

```html
👑Epics

👑Website Updates for www.thecloudopscommunity.org
  📗Homepage
     ☑Designing a homepage header
     ☑Standardizing fonts
     ☑Fixing the homepage CSS to make it mobile responsive
  📗About Us Page
  📗Secure Sign-In
  
👑Cloud Migration
👑CICD Implementation
```


## TimeLines
1. Scheduling start and end dates for releases and Sprint
[Ms Docs](https://learn.microsoft.com/en-us/azure/devops/boards/sprints/define-sprints?view=azure-devops)
2. Estimating and prioritising work item
- https://www.simplilearn.com/project-estimation-techniques-article
 - [Scrum Key Concepts](https://learn.microsoft.com/en-us/azure/devops/boards/sprints/scrum-key-concepts?view=azure-devops)
 - [Sprint Burndown](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/configure-sprint-burndown?toc=%2Fazure%2Fdevops%2Fboards%2Ftoc.json&view=azure-devops&tabs=remaining-work%2Cmay)

 ## Azure Work Items Basics 
 - Use work items to track features and requirements you're developing
- Differs based on Process Type
- Backlog =
- below describe {WHAT CUSTOMER ACTUALLY WANT / SAID} : the customer value of the work to do and provide fields to track information about that work.
- User Stories (Agile) == Issues (Basic) == Product Backlog Items (Scrum) == Requirements (CMMI)
- **Problems** : nonwork project elements that can affect work getting done. *By default, they don't appear on any backlog or board.*
- Example : Issue (Agile and CMMI) and Impediment (Scrum)
- [Track bugs - show them on board/backlog](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/about-work-items?view=azure-devops&tabs=agile-process#track-bugs-as-requirements-or-tasks)
- Leave `it blank and assign it later, during a planning meeting` - Iteration and Area Path

## [Real World - HOw to Add Work Item Methods and Best Parctices](https://www.vivienfabing.com/azure-devops/2020/04/30/azureboards-practical-example-before-sprint-planning.html)
  
#### Assignment 
- You can assign a work item to one and only one user at a time.
- If work is split across two or more users, consider creating separate work items that you'll assign to each user responsible for the work to complete

#### [Work item states](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/about-work-items?view=azure-devops&tabs=agile-process#track-active-open-resolved-or-closed-work-items)

## Areas 
> areas will be used by teams to determine what shows up on the team's backlog and what work items the team is responsible for.

## Iterations
- Teams plan and track work at regular time intervals, commonly referred to as an iteration or sprint. 
- The iterations selected below will appear in the Sprints hub for your team. Each iteration will have a backlog and board to help your team plan and manage work.

## Automation
org sesttings >> All processes >> Project Name >> Process Type >> Work item type 
- specify layout, state, automation rules

### Create Work Item Templates 
[Helps In repetable task](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/work-item-template?view=azure-devops)
- create work item => capture template
- next create new (same work item type) => 3 dots => click on your template name

### [Boards all portal options](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/about-work-items?view=azure-devops&tabs=agile-process#track-work-in-the-web-portal)

> **The product owner owns the product backlog. The development team owns and maintains the sprint backlog. The product backlog forms part of a product's long-term strategic plan and evolves with the product. The sprint backlog is a short-term plan to accomplish a series of tasks within a sprint.**

### Product Backlog 
> product owner is a role on a Scrum team that is responsible for the project's outcome.
> [From Scrum Docs](https://www.scrum.org/resources/what-is-a-product-owner)
- Product owners should review the backlog before each iteration planning meeting to ensure prioritization is correct and feedback from the last iteration has been incorporated.
- product owner is free to re-prioritize work in the backlog at any time due to customer feedback, refining estimates, and new requirements. 
- [Blog Attlasian](https://www.atlassian.com/agile/scrum/backlogs)

- Teams can use the board to update the status of requirements, and the Taskboard to update the status of tasks.
![](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/guidance/agile-process-workflow?view=azure-devops)

![image](https://github.com/user-attachments/assets/1c441c4f-a525-4f30-be11-ea439e60492d)

## Boards and Backlogs in left side
- boards : for PM : shows high level overwiew
- backlogs: in agile you add the user story you need to work with
- then (+) to add task within that user story
- also in left side sprint (same thing show up) => change state from drop down => auto updated in azure boards boards
- column name setting scroll down it shows what state = what column
### Wiki
- [ms docs]()
- shows up every `md` file from selected folder (continuos sync)
- [Md vs Readme vs Wiki - they complement](https://learn.microsoft.com/en-us/azure/devops/project/wiki/about-readme-wiki?view=azure-devops)
- [How your Readme file should be?](https://learn.microsoft.com/en-us/azure/devops/project/wiki/about-readme-wiki?view=azure-devops#readmes)

talking about a project repository :
> A README should contain only the necessary information for developers to get started using and contributing to your project. Longer documentation is best suited for wikis.
> getting started information (i.e. local setup), and leave the long form information such as application features, design principles, etc. in the wiki.
- `Readme.md` is the packaging
- `wiki pages` is made for development/contributors documentation
- `gh-pages` branch hosts user documentation
- https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis
- https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

## Dashboards 
1. Write Queries [Suggestions from MS Docs here](https://learn.microsoft.com/en-us/azure/devops/boards/queries/example-query-charts?view=azure-devops#maintain-backlog-hygiene)
2. Save Query to `Shared Folder`
3. top ribbon => charts => select chart => `+add to dashboard`
4. Its `vIsible in Dashboard Now`
5. `Continous Sync => Add work items => shows Up :) `
6. **[Track progress with status and trend query-based charts](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/charts?view=azure-devops)**
   
## Burndown Charts
Burndown charts are useful for determining how quickly work is progressing based on a numeric field value, such as Story Points, Effort, or Remaining Work, or on a count of work items.
> burndown chart of tasks, select the Sum operator for Remaining Work.
[Youtube video on how to interpret it](https://youtu.be/DxGc9mqiLlU?si=ymLjFIW7JMy9hXVG)

## Velocity - [MS Docs](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/team-velocity?view=azure-devops&tabs=in-context)
Velocity metrics provide useful information, so teams can plan and forecast sprints and determine how well they estimate and meet planned commitments. You can get an indication of how much work a team can complete during a sprint based on either a count of work items completed or the sum of estimates made for effort (product backlog items), story points (user stories), or size (requirements). Use velocity as an aid to determine team capacity and don't confuse it with key performance indicators.

## Connect Power BI with Azure boards analytics view 
[DDocs](https://learn.microsoft.com/en-us/azure/devops/report/powerbi/create-quick-report?view=azure-devops)


