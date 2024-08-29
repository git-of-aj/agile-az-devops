# agile-az-devops

## AWS 
agile vs DevOps : https://aws.amazon.com/compare/the-difference-between-agile-devops/

## Labs:
1. [Devops End to ENd ](https://azuredevopslabs.com/labs/azuredevops/EndtoEnd/)
2. [Agile with Boards](https://azuredevopslabs.com/labs/azuredevops/agile/)
3. [Building a roadmap and tracking dependencies across teams with Delivery Plans](https://azuredevopslabs.com/labs/azuredevops/deliveryplans/)

-----
Azure Boards is a suite of Agile tools that helps manage software projects, providing features like Work Items, Kanban boards, Sprints, and Backlogs. Below is a breakdown of when and how to use Teams, Area Paths, Backlogs, and Sprints, along with how they work together:

### **1. Azure Boards Teams:**
- **What It Is:** Teams in Azure Boards allow you to organize people into smaller units, each responsible for specific parts of the project. A team has its own backlog, sprint schedule, and Kanban board.
- **When to Use:** You should create teams when you have a larger project with multiple groups working on different features or components. Teams can represent different product lines, feature teams, or departments.

### **2. Area Paths:**
- **What It Is:** Area Paths define logical groupings of work within a project. They allow you to segment your work into different areas, like modules or features.
- **When to Use:** Use Area Paths when you need to organize work across different parts of a system, components, or services. This is helpful for filtering and reporting on work items specific to certain areas of the product.

### **3. Backlogs:**
- **What It Is:** The backlog is a prioritized list of work items (features, bugs, tasks) that need to be completed. Azure Boards supports different levels of backlogs, such as product backlogs for higher-level work items (e.g., Epics, Features) and sprint backlogs for more detailed tasks.
- **When to Use:** Backlogs are used for prioritizing work. You should have a product backlog for long-term planning and sprint backlogs for short-term execution.

### **4. Sprints:**
- **What It Is:** Sprints represent time-boxed iterations where a specific amount of work is completed. Azure Boards lets you create sprint schedules, assign work items, and track progress.
- **When to Use:** Use sprints to manage and execute work in time-boxed iterations. They help with focusing on delivering small, incremental improvements in a predictable timeframe (e.g., every two weeks).

### **How They Work Together:**
- **Team Structure:** Each team has its own Area Path, Backlog, and Sprints. This allows teams to work independently but within the same project.
- **Planning Work:** The product owner or project manager can prioritize the overall backlog. Based on team capacity, work items are assigned to different teams, which can then plan their own sprints.
- **Area Paths & Reporting:** Area Paths allow you to assign work items to specific parts of the system. You can generate reports and track progress by Area Path, helping you understand how different parts of the project are progressing.
- **Backlogs into Sprints:** Teams pull work items from their backlog into their sprint during sprint planning. This ensures that only a manageable amount of work is committed to during each sprint.
- **Execution:** During the sprint, teams work on their assigned tasks, using the Kanban board to track progress. At the end of the sprint, work is reviewed, and completed tasks are moved to "Done."

### **Example:**
Imagine a large project with multiple teams working on different features:

1. **Team A** is working on the frontend of a web app.
2. **Team B** is working on the backend services.
3. **Area Paths** are created for "Frontend" and "Backend."
4. The **product backlog** contains user stories for both frontend and backend features.
5. Each team pulls from the product backlog into their **sprint backlog** during sprint planning.
6. Over the course of a two-week sprint, Team A completes frontend tasks, and Team B completes backend tasks.
7. The project manager can track progress across the entire project using the **Area Path** filters to see how much work is done in both the frontend and backend areas.

This structure ensures that each team works efficiently, but the overall project remains coordinated.
