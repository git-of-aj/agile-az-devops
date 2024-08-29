Branching Strategy in GIT - Git Flow

Git Flow is a branching strategy designed to streamline the development process and ensure code quality. It is widely used in software development projects and the detailed explanation is below:

🔶 main branch:
This branch contains which is production-ready code means only stable and tested code is merged into this branch. Release are tagged in this branch.
🔶 develop branch:
This is the branch in which all the developers push their code and it acts as a staging area for all new code before it is merged into main.
🔶 feature/* branch:
This is used for developing new features by developers and it is created from the develop and merged to develop branch once done.
🔶 release/*:
This is the branch in which the code sits before the new release and it is created from the develop and merged to main. Allows for minor bug fixes and preparing meta-data for a release.
🔶hotfix/*:
This is used for critical fixes in production. It is created from the main and merged back into both main and develop after the fix.

![image](https://github.com/user-attachments/assets/e0b4cb2a-ceec-4ec9-bdf3-5d2307895a74)
