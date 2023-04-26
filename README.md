# teaching-github
A repository for my team to learn and understand GitHub.

# GitHub pre-requisites
Visit [GitHub's documentation](https://docs.github.com/en/get-started/quickstart/set-up-git#setting-up-git) to install Git Bash and set-up everything on your local system.

## Cloning this repository
This is important to be able to work on this repository on your local system. Run the following on Git Bash or Command Line Interface of your system.
```
git clone https://github.com/vish-rt/teaching-github.git
```

## Making changes
You can open this project within VSCode or any other preferred IDE. While working you may notice such changes within your IDE:

![VSCode](https://user-images.githubusercontent.com/93420999/234667643-1af9b861-eb0f-4b51-a88c-7fe3b57ae74a.png)
- `M` stands for Modified Files (i.e: the files which already exist on the repository but are modified on your local)
- `U` stands for Untracked Files (i.e: the files which do not exist on the repository and were crreated by you on your local)

# Reflecting your changes on GitHub

At any given time, you can check the status of your modifications on the local:
```
git status
```

## Staging Area
- Staging Area in Git is is the middle ground between what you have done to your files and what was last committed in the repository.
- Before reflecting your changes on GitHub, all files are needed to be added to this staging area.
- To add files to staging area, use the following command:
```
git add file.txt
```
- This adds file.txt to the staging area. If you want to add all files, use `git add .`

## Commits and Pushes
- GitHub is a version control tool. To track all past versions, GitHub uses `commits` made by contributors to show changes made to the files.
- To reflect your local changes on GitHub, they need to be committed first with the following command:
```
git commit -m "<your commit message>"
```
- You must ensure that `<your commit message>` is a valid explanation of the changes you have made to the files.

Finally, once all of the above are done, push your changes to GitHub:
```
git push
```

# Branches and Pull Requests
Many organizations like TCET - Open Source, follow the **Pull Request (PR) Model** to add their contributions on GitHub. It is necessary to understand how they work in order to contribute to any repository.

## Branching
- For multiple contributors working on various parts or features of a project, GitHub makes use of `branches` in order to let you work on your code and push it without interfering the code being worked on by other contributors.
- To create your branch, use the following syntax:
```
git checkout -b <your branch name>
```
- This enables you to create a branch and switch on it. One must ensure that the branch names are not random and reflect the feature it is used to work on.

- To list all branches of a repository use the following command:
```
git branch -a
```
- For switching between branches, use the `git checkout <branch name>` command, replacing it with the actual branch name.
- Before committing any changes you need to ensure that you are pushing to the correct branch using `git branch` command, otherwise you may make a fellow contributor very unhappy.

## Pull Requests
- Usually in organizations, the `main` branch is locked by the repository admin to ensure that no outside contributor directly edits the main source code of the project.
- Upon pushing to your branch, you would be able to see updates on GitHub:
![Branch Update](https://user-images.githubusercontent.com/93420999/234677770-d5061b9c-1e88-40a0-9edd-71115a05d166.png)
- You can click on `Compare and Pull Request` (or alternatively, visit your branch and click on `Contribute`) to **create a Pull Request**.

By following the above step, you will be able to edit the PR on GitHub's editor. As a good developer practice, you should elaboratively describe what changes you have made to the code and highlight them in the description.
![Pull Request](https://user-images.githubusercontent.com/93420999/234678121-d4ddf6d9-ab59-45c6-92aa-da06bb7ff3e6.png)

- Upon submitting the pull request, the administrator is notified of your changes and can approve, reject or add suggestions to your merge.
- You can also notify repository maintainers and engage conversations with them on the pull request. An example of such conversation can be observed here:
![Conversation](https://user-images.githubusercontent.com/93420999/234681510-61361da1-c493-4f14-94a1-5737271d49e7.png)

Once a maintainer approves your changes, then finally your pull request will be merged to the `main` branch.

# Conclusion
Take everything one step at a time. Everything here may feel overwhelming as there are too many things to be aware of, but following this guide will help you grasp the concepts of Git and GitHub, from basic cloning to creating your first pull request.

If you're stuck or confused or have any suggestions, reach out to me by creating an issue in this repository or via Discord. I'll be happy to help!