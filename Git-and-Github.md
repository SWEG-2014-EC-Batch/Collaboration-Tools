# Git & GitHub & GitHub flow

## Learning objectives
- Understand the concept of version control.
- Follow GitHub flow.
- Create branches that each have a different base branch.
- Open PRs in GitHub.

## What is a version control system? How is it related to Git and GitHub?

A version control system tracks the history of changes to files. It is especially useful in projects built by software development teams.
As the project evolves teams can run tests, fix bugs, and contribute new code with confidence that any version can be recovered at any time.
Reconstructing the edit history of various files can be useful for a variety of reasons, such as when you need to investigate when some change was introduced and why.
You are already familiar with Git and GitHub but it is also important that you understand how they relate to the concept of a version control system.

### Why is it important?

At Microverse you will use Git and GitHub to keep track of all the changes to your code as well as to collaborate with your peers.
Understanding what Git and GitHub are will make it much easier for you to join a company and get used to their workflow faster, because almost every single company that you can join uses a version control system.

### What's the difference between Git and GitHub?

**Git** is an example of a distributed version control system. **GitHub** is a Git hosting repository that provides developers with tools to ship better code.
Read the [10 minute long introduction article from the Git Handbook](https://guides.github.com/introduction/git-handbook/) and make sure that you understand this difference.

NOTE: Stop yourself from checking all links in this article! We will guide you through what to learn about Git and GitHub in future lessons, so do not try to learn everything about them right now.

## GitHub flow

GitHub flow is a detailed process for using branches with your team.

***SPOILER ALERT** GitHub flow is slightly different than Gitflow, even though their names look alike.*
*If you look for additional information, please make sure that you are using the correct name - GitHub flow. And worry not!*
*You will learn about another flow in a few more lessons!*

### Why is it important?

If everybody in your team uses the same flow, you collaborate more effectively because everyone knows how to track the history of changes in your shared code easily.

### How to use GitHub flow

In order to learn how to use GitHub flow with your team:
- Read this [GitHub Guides article](https://guides.github.com/introduction/flow/) that explains the concept of the GitHub flow with a nice visualization.
- Read [How to use GitHub flow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/github_flow.md), which will guide you through the entire concept.
- Skim through the [Multiple pull requests within one repo](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/multiple_pull_requests.md) article. You will see a reminder about that process in your first projects.

### Get Familiar with Git Basic Commannds
- [ ]  [Free play with Git](http://git-school.github.io/visualizing-git/) - Use this visualizer to understand the basic Git commands listed below.
    - *Expand the Git Basic Command below and copy the following Git commands one-by-one into the visualizer and check out what happens to the repository:*
    -git commit -m "Second commit"
    <details id=112>
       <summary><h4>Basic Git Commands </h4></summary>
    
        git commit -m "Third commit"
        git log

        git branch
        git branch my-feature
        git branch

        git checkout my-feature
        git log

        git commit -m "Fourth commit"
        git commit -m "Fifth commit"
        git log

        git checkout master
        git log
        git branch my-second-feature
        git commit -m "Sixth commit"
        git commit -m "Seventh commit"
        git log

        git checkout my-feature
        git branch bug-fix
        git branch

        git commit -m "Eighth commit"
        git commit -m "Ninth commit"
        git log

        git checkout bug-fix
        git commit -m "Tenth commit"
        git log

        git checkout my-feature
        git log

        git merge bug-fix
        git checkout my-feature
        git log
        git commit -m "Eleventh commit"
        git log

        git checkout master
        git log

        git merge my-feature
        git log
    </details>


### Additional materials

**These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.**

- [Atlassian's "Git feature branch workflow" article](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow).
- ![Git--distributed-is-the-new-centralized](https://git-scm.com/)
- ![Git Hub Docs](https://docs.github.com/en)

# Introduction to GitHub

_Get started using GitHub in less than an hour._

<!-- 
  <<< Author notes: Start of the course >>> 
  Include start button, a note about Actions minutes,
  and tell the learner why they should take the course.
  Each step should be wrapped in <details>/<summary>, with an `id` set.
  The start <details> should have `open` as well.
  Do not use quotes on the <details> tag attributes.
-->

<!--step0-->

People use GitHub to build some of the most advanced technologies in the world. Whether you’re visualizing data or building a new game, there’s a whole community and set of tools on GitHub that can help you do it even better. GitHub Skills’ “Introduction to GitHub” course guides you through everything you need to start contributing in less than an hour.

- **Who is this for**: New developers, new GitHub users, and students.
- **What you'll learn**: We'll introduce repositories, branches, commits, and pull requests.
- **What you'll build**: We'll make a short Markdown file you can use as your [profile README](https://docs.github.com/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).
- **Prerequisites**: None. This course is a great introduction for your first day on GitHub.
- **How long**: This course is four steps long and takes less than one hour to complete.

## How to start this course

1. Above these instructions, right-click **Use this template** and open the link in a new tab.
   ![Use this template](https://user-images.githubusercontent.com/1221423/169618716-fb17528d-f332-4fc5-a11a-eaa23562665e.png)
2. In the new tab, follow the prompts to create a new repository.
   - For owner, choose your personal account or an organization to host the repository.
   - We recommend creating a public repository—private repositories will [use Actions minutes](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions).
   ![Create a new repository](https://user-images.githubusercontent.com/1221423/169618722-406dc508-add4-4074-83f0-c7a7ad87f6f3.png)
3. After your new repository is created, wait about 20 seconds, then refresh the page. Follow the step-by-step instructions in the new repository's README.

<!--endstep0-->

<!-- 
  <<< Author notes: Step 1 >>> 
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

<details id=1>
<summary><h2>Step 1: Create a branch</h2></summary>

_Welcome to "Introduction to GitHub"! :wave:_

**What is GitHub?**: GitHub is a collaboration platform that uses [Git](https://docs.github.com/get-started/quickstart/github-glossary#git) for versioning. GitHub is a popular place to share and contribute to [open-source](https://docs.github.com/get-started/quickstart/github-glossary#open-source) software.
<br>:tv: [Video: What is GitHub?](https://www.youtube.com/watch?v=w3jLJU7DT5E)

**What is a repository?**: A [repository](https://docs.github.com/get-started/quickstart/github-glossary#repository) is a project containing files and folders. A repository tracks versions of files and folders.
<br>:tv: [Video: Exploring a repository](https://www.youtube.com/watch?v=R8OAwrcMlRw)

**What is a branch?**: A [branch](https://docs.github.com/en/get-started/quickstart/github-glossary#branch) is a parallel version of your repository. By default, your repository has one branch named `main` and it is considered to be the definitive branch. You can create additional branches off of `main` in your repository. You can use branches to have different versions of a project at one time.

On additional branches, you can make edits without impacting the `main` version. Branches allow you to separate your work from the `main` branch. In other words, everyone's work is safe while you contribute.
<br>:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

**What is a profile README?**: A [profile README](https://docs.github.com/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme) is essentially an "About me" section on your GitHub profile where you can share information about yourself with the community on GitHub.com. GitHub shows your profile README at the top of your profile page.

### :keyboard: Activity: Your first branch

1. Open a new browser tab, and navigate to this same repository. Then, work on the steps in your second tab while you read the instructions in this tab.
2. Navigate to the **Code** tab.
3. Click on the **main** branch drop-down.<br>
   <img alt="image showing my-first-branch entry" src="/images/my-first-branch.png"/>
4. In the field, enter a name for your branch: `my-first-branch`.
5. Click **Create branch: my-first-branch** to create your branch.
6. Move on to Step 2!<br>
   **Note**: If you made a public repository, and want to confirm you correctly set up your first branch, wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically close this step and open the next one.

</details>

<!-- 
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

<details id=2>
<summary><h2>Step 2: Commit a file</h2></summary>

_You created a branch! :tada:_

Creating a branch allows you to edit your project without changing the `main` branch. Now that you have a branch, it’s time to create a file and make your first commit!

**What is a commit?**: A [commit](https://docs.github.com/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits) is a set of changes to the files and folders in your project. A commit exists in a branch.

### :keyboard: Activity: Your first commit

The following steps will guide you through the process of committing a change on GitHub. Committing a change requires first adding a new file to your new branch. 

1. On the **Code** tab, make sure you're on your new branch `my-first-branch`.
2. Select the **Add file** drop-down and click **Create new file**.<br>
   ![create new file option](/images/create-new-file.png)
3. In the **Name your file...** field, enter `PROFILE.md`.
4. In the **Edit new file** area, copy the following content to your file:
   ```
   Welcome to my GitHub profile!
   ```
   <img alt="profile.md file screenshot" src="/images/my-profile-file.png"/>
5. For commits, you can enter a short commit message that describes what changes you made. This message helps others know what's included in your commit. GitHub offers a simple default message, but let's change it slightly for practice. First, enter `Add PROFILE.md` in the first text-entry field below **Commit new file**. Then, if you want to confirm what your screen should look like, expand the dropdown below.
   <details>
   <summary> Expand to see the screenshot.</summary>
   <img alt="screenshot of adding a new file with a commit message" src="/images/commit-full-screen.png" />
   </details>
6. In this lesson, we'll ignore the other fields and click **Commit new file**.
7. Move on to Step 3! <br>
   **Note**: Like before, you can wait about 20 seconds, then refresh this page (the one you're following instructions from) and [GitHub Actions](https://docs.github.com/en/actions) will automatically close this step and open the next one.

</details>

<!-- 
  <<< Author notes: Step 3 >>> 
  Just a historic note: the previous version of this step forced the learner
  to write a pull request description,
  checked that `main` was the receiving branch,
  and that the file was named correctly.
-->

<details id=3>
<summary><h2>Step 3: Open a pull request</h2></summary>

_Nice work making that commit :sparkles:_

Now that you’ve created a commit, it’s time to share your proposed change through a pull request!

**What is a pull request?**: Collaboration happens on a pull request. The pull request shows the changes in your branch to other people. This pull request is going to keep the changes you just made on your branch and propose applying them to the `main` branch.
<br>:tv: [Video: Introduction to pull requests](https://youtu.be/kJr-PIfLDl4)

### :keyboard: Activity: Create a pull request

You may have noticed after your commit that a message displayed indicating your recent push to your branch and providing a button that says **Compare & pull request**.

![screenshot of message and button](/images/compare-and-pull-request.png)

 If you want, feel free to click **Compare & pull request**, and then skip to step 6 below. If you don't click the button, the instructions below walk you through manually setting up the pull request.

1. Click on the **Pull requests** tab in your repository.
2. Click **New pull request**.
3. In the **base:** dropdown, make sure **main** is selected.
4. Select the **compare:** dropdown, and click `my-first-branch`. <br>
   <img alt="screenshot showing both branch selections" src="/images/pull-request-branches.png"/>
5. Click **Create pull request**.
6. Enter a title for your pull request: `Add my first file`.
7. The next field helps you provide a description of the changes you made. Feel free to add a description of what you’ve accomplished so far. As a reminder, you have: created a branch, created a file and made a commit! <br>
   <img alt="screenshot showing pull request" src="/images/Pull-request-description.png"/>
8. Click **Create pull request**.
9. Move on to Step 4! <br>
   **Note**: Like before, you can wait about 20 seconds, then refresh this page (the one you're following instructions from) and [GitHub Actions](https://docs.github.com/en/actions) will automatically close this step and open the next one. As a perk, you may see evidence of GitHub Actions running on the tab with the pull request opened! The image below shows a line you might see on your pull request after the Action finishes running.<br>
   <img alt="screenshot of an example of an actions line" src="/images/Actions-to-step-4.png"/>

</details>

<!-- 
  <<< Author notes: Step 4 >>> 
  Just a historic note: The previous version of this step required responding
  to a pull request review before merging. The previous version also handled
  if users accidentally closed without merging.
-->

<details id=4>
<summary><h2>Step 4: Merge your pull request</h2></summary>

_Nicely done friend! :sunglasses:_

You successfully created a pull request. You can now merge your pull request.

**What is a _merge_**: A [merge](https://docs.github.com/en/get-started/quickstart/github-glossary#merge) adds the changes in your pull request and branch into the `main` branch.
<br>:tv: [Video: Understanding the GitHub flow](https://www.youtube.com/watch?v=PBI2Rz-ZOxU)

As noted in the previous step, you may have seen evidence of an action running which automatically progresses your instructions to the next step. You'll have to wait for it to finish before you can merge your pull request. It will be ready when the merge pull request button is green.

![screenshot of green merge pull request button](/images/Green-merge-pull-request.png)
### :keyboard: Activity: Merge the pull request

1. Click **Merge pull request**.
1. Click **Confirm merge**.
1. Once your branch has been merged, you don't need it anymore. To delete this branch, click **Delete branch**.<br>
   <img alt="screenshot showing delete branch button" src="/images/delete-branch.png"/>
2. Check out the **Finish** step to see what you can learn next!<br>
   **Note**: Like before, you can wait about 20 seconds, then refresh this page (the one you're following instructions from) and [GitHub Actions](https://docs.github.com/en/actions) will automatically close this step and open the next one.

</details>

<!-- 
  <<< Author notes: Finish >>> 
  Review what we learned, ask for feedback, provide next steps.
-->

<details id=X>
<summary><h2>Finish</h2></summary>

_Congratulations friend, you've completed this course and joined the world of developers!_

<img src=https://octodex.github.com/images/collabocats.jpg alt=celebrate width=300 align=right>

Here's a recap of your accomplishments:

- You learned about GitHub, repositories, branches, commits, and pull requests.
- You created a branch, a commit, and a pull request.
- You merged a pull request.
- You made your first contribution! :tada:

### What's next?

  If you'd like to make a profile README, use the simplified instructions below or follow the instructions in the [Managing your profile README](https://docs.github.com/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme) article.
  1. Make a new public repository with a name that matches your GitHub username.
  2. Create a file named `README.md` in its root. The "root" means not inside any folder in your repository.
  3. Edit the contents of the `README.md` file.
  4. If you created a new branch for your file, open and merge a pull request on your branch.
  5. We'd love to see your new profile! Share your profile on social media and tag us!
  6. Lastly, we'd love to hear what you thought of this course [in our discussion board](https://github.com/skills/.github/discussions).

Check out these resources to learn more or get involved:
- Are you a student? Check out the [Student Developer Pack](https://education.github.com/pack).
- [Take another GitHub Skills course](https://github.com/skills).
- [Read the GitHub Getting Started docs](https://docs.github.com/en/get-started).
- To find projects to contribute to, check out [GitHub Explore](https://github.com/explore).

</details>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/skills/.github/discussions) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2022 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [CC-BY-4.0 License](https://creativecommons.org/licenses/by/4.0/legalcode)
