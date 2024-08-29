[Branching Strategy in GIT](https://medium.com/@dmosyan/version-control-branching-strategies-e68e8d5ef1e0)

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
What are some popular deployment strategies used in CI/CD pipelines?

- 🔮 Rolling Deployment: Incrementally replaces instances of the previous version of an application with the new version without downtime.

- 🔮 Blue-Green Deployment: Involves two identical environments, one hosting the current version (blue) and the other hosting the new version (green). Traffic is switched from blue to green once the new version is ready.

- 🔮 Canary Deployment: Releases the new version to a small subset of users before rolling it out to the entire user base. This strategy allows for testing in production with real users and workloads.

- 🔮 A/B Testing: Similar to canary deployments but specifically targets testing new features or changes among different user segments to compare performance.

- 🔮 Feature Toggles (Feature Flags): Allows teams to enable or disable features in the application without deploying new code. This facilitates testing and gradual rollout of new features.
