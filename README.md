# Get a Jumpstart on Collaboration and Code Review in GitHub

This is a transcript of a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give at [DjangoCon](https://2017.djangocon.us), [PyLadies Remote](http://remote.pyladies.com), and other events.

<!--
* [Original slide deck]()
* [Video recording]()
-->

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016/). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

## Transcript

<table>


<tr><td width="30%">

![Slide 0]()

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 1]()

</td><td>

### Welcome 

I'm thrilled to have the opportunity to talk to you about getting a jumpstart on collaboration and code review in GitHub

</td></tr>


<tr><td width="30%">

![Slide 2]()

</td><td>

### About Me 

* DjangoCon Website Chair
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

I hope you've had a chance to take a good look at the DjangoCon website. I'm so proud of what the team has accomplished. It's truly a beautiful website.

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### What This Talk Is and Is Not

There are many variations to how things can be done in GitHub. This talk is not about teaching you all of those variations. At the end of this talk, you will find links to the official documentation of Git and GitHub where you can find info about variations. This talk is about teaching you the essential process and the underlying common thread between collaboration and code review, so that you can get started as quickly as possible. 

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### The Journey

<!--
There is a saying, "Don't miss the forest for the trees". It means, don't focus so much on the details that you don't see the larger picture.
-->

Let’s pretend we’re going on a journey. The journey is to learn collaboration and code review. I've made this Journey Before. When you are making a journey, often you are engrossed in each step. When you complete the journey, looking back, perhaps you see the larger picture and have learned something. If I were to start my journey of learning collaboration and code review over again, knowing what I know now, I would do things differently from the beginning. 

I want to impart some of my knowledge to you, to save you the time and frustration of learning by trial and error the way that I did, because I want all of you to get started more quickly than me.

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### What is the Destination?

Do you remember a time before you were interested in building things with code? There is a lot of power and value in the ability to make things. You can apply collaboration and code review skills in an unlimited number of situations. GitHub is a very popular place to work on open-source code. Check out GitHub Showcases and Trending to see some of the awesome projects.  
Some benefits of learning collaboration and code review
* If you are a student: being prepared for your studies and career
* If a developer: perhaps you can get a promotion
* In general: you can make cool stuff, make choices that influence product

</td></tr>


<tr><td width="30%">

![Slide 6]()

</td><td>

### How My Own Journey Began

I first signed up for GitHub on April 18, 2013. I knew using GitHub was a good idea. But my account sat unused for months. I felt a bit intimidated and I didn't know how to get started. Later on in this talk, I will debunk some of the myths that I believed at the time. 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### TacoFancy: A Taco Recipe Sharing Project on GitHub!

One day, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

I was looking through the Taco Fancy repo and saw one sentence made a big impact on me: "Are You New to Github But Want to Contribute?" I had been secretly wanting to contribute for months, but wasn't sure how, and now was my chance. I didn't quite feel like I knew what I was doing, but I was extremely motivated. I struggled through and submitted a pull request on November 3, 2013, which was about 7 months after I joined GitHub

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### 3 More Years to Get Started Doing Code Review

It would take almost 3 more years for me to begin doing code review. Now that I do it, I wonder, why did it take so long?! To me, it feels like a combination of perceived territoriality and lack of knowledge. This doesn't make sense in terms of the number of maintainers. 

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### A Few Notes

* This talk uses GitHub examples, but similar features and workflows could be found in Bitbucket or other services (which some people prefer)
* The examples I will be using will focus on public, organizational repos and “Shared Repository Model”, because that is where most of the collaboration and code review are done
* I will identify best practices any time possible
* Some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions

<!--
Example- some operating systems do not use dollar signs $ as command line prompts.
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### Getting Help

<!--
* [Using Keyboard Shortcuts](https://help.github.com/articles/using-keyboard-shortcuts)
-->

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### Prerequisite Checklist

* Install Git on your computer
* Create a GitHub account online
* Find and open your terminal (a.k.a. command line) on your computer
* The ability to navigate via terminal would be helpful (example: know how to change directory)
* You might also want to have a text editor of your choice installed, to use to edit files

<!--
Bash command list, text editor recommendations
There are a ton of tutorials out there for getting started. I am going to be focused on workflow because there are fewer tutorials out there for what I am going to explain. 
-->

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### Browser Versus Command Line

<!--
GitHub desktop, Hub

I want to point out that you can create a branch through the browser, but I will be showing you how to create a branch through terminal/command line, because it's what you will use terminal/command line often with code review. 
-->

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### Getting Started: Basics

What are Git and GitHub?

High level explanation: Git is a version control system that you install on your computer and use via your terminal. GitHub is a web-based dashboard that you can use in conjuction with Git. I kind of think of GitHub as being like Facebook for developers. You have a profile where you store your code in repositories (a.k.a repos) and you have a newsfeed where you can see the activity of developers you follow. Organizations can have accounts too. If you want to work on code, you can clone or download a repo onto your personal computer, make your changes, then push the changes back to the repo on GitHub. Meanwhile, other users can add their own changes. Git and GitHub will record every change to a file and will tell you if there is a conflict between the changes of two different people. 

<!--
Recap:
What is a repo?
What is a fork?
What is a pull request?
-->

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### Read/Write Access and Why It Matters

An important concept in GitHub collaboration: Do you have read/write access to the repo you want to contribute to? It doesn't matter what kind of repo you are contributing to, the way that you contribute to a project depends on whether you have read/write access to it. 

What does read/write access allow you to do? 

<!--
List
Tip: You have to have read/write access to push directly to a repository
-->

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Read/Write Access Examples

* A repo you have created in your own user account (you have read/write access as the owner)
* A repo in someone else's user account that the owner has given you read/write access to as a collaborator (less common)
* A repo in an organizational account that an owner has give you read/write access to as a maintainer (more common)

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### User Versus Organizational Account

Using an organizational account rather than a user account for collaboration has some advantages:
* With a user account, one owner and the collaborators have access to one repo
* With an organizational account, owner(s) can create teams and permissions, with team members working across multiple repos
* Otherwise, the repo shared repository settings are similar

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### Two Collaborative Development Models

The question of read/write access leads us to collaborative development models. Collaborative development model is just a fancy term for how people work on software together. The two collaborative development models basically correspond to whether you have read/write access.

There are two collaborative development models: 
* “Fork and Pull” Model
* “Shared Repository” Model

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### The Differences Between the Two Collaborative Development Models

If you have read/write access to the repo you want to contribute to, you can make changes directly within the repo. This is the "Shared Repository" Model. I do want to point out though that when you are made a collaborator in a project, there is often a level of trust involved. The code in the repo might be live. Whether or not you should be making changes directly into a live branch depends on your level of comfort with a project. It's often best to have another maintainer review your work through a pull request.

If you do not have read/write access to the repo you want to contribute to, you will need to make a copy of the repo, called a fork, in your user account to work on and submit your pull request using the fork. This is called the "Fork and Pull" Model. The fork will be an exact copy at the time that it was forked, in your account, with your username in the URL. You will be the only person with read/write access to it unless you give read/write access to someone else. If you make changes to it, the repo you want to contribute to will not be affected unless you submit a pull request and it is accepted. 

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Switching Between Multiple Tasks

There is an overall theme to this talk. In order to be able to increase your level of responsibility, you need to be able to switch between multiple tasks. 
* Keep your code up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### Example of a Not-Scalable Workflow

* Fork a repo, make changes directly into the branch you want to change, then submit a pull request. You are then stuck waiting until the pull request is accepted. If you delete the fork, the pull request can still be accepted, but it's considered inactive and you will not be able to add follow-on commits. 

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Best Practice Workflow

It's a best practice to use branches. You can switch between multiple tasks by using "branches". If you learn to use branches, you will have the fundamentals skills and freedom that will help you to do both collaboration and code review. 

What is a branch? 

Within your a repo is a codebase. You can make a copy of the codebase within the repo. The copy is called a branch. When you are finished making changes to a branch, you can submit a pull request and if the pull request is accepted, your changes will be merged into the codebase. Git will replace the old part of the codebase with your changes, and keep everything else the same. Meanwhile, you can keep your codebase up to date and make unlimited new branches. When you review pull requests, the pull requests will also be in the form of branches. 

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### General Branch Process

The process for working with branches is very similar, regardless of which collaborative development model you are using. Parts of this process can also be used during code review.

* If you do not have read/write access to the repo you want to contribute to, fork the repo
* Clone or download the organizational or forked repo (whatever your origin is, which I'll explain in a minute)
* Change directory
* Verify which branch you are checked out on
* Create and switch to a branch (note how local files switch to the files of the branch you switch to)
* Make your change to the files
* Add, commit, create a message
* Push branch to organizational or forked repo (whatever your origin is)
* Submit pull request


<!--
# Clone/Download and Push Feature Branch to Repo (Almost Same Process for Forked Repo or Organizational Repo)

Switch perspective
* URL of the repo you have read/write access to
* Fork an organizational/user account repo, perhaps clone locally
* Go to the fork, which will be in your user account, perhaps clone locally
* Go directly into the forked branch you are contributing to

Typical "fork and pull" situation/process: a user forks a repo within GitHub. New repo will appear in user account, with username in repo URL. The user will make a change in the browser, or clone the repo locally, and make change and push back to user account (which is the origin). User will submit pull request via own account. 

Typical situation/process: a user has been given read/write access to an organizational repo. User clones the repo locally using the organizational repo URL (the organizational repo is the origin). User creates a feature branch, pushes new branch to organizational repo, and submits pull request from within organizational repo.

The two main differences are that if you are using the "Fork and Pull" Model:
* You need to fork the repo before you clone it
* You need to check a box when you make the pull request if you want the maintainers to be able to change your pull request
-->

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### A Note About Remotes

What is origin?

When you clone a repo locally, the remote will automatically assigned the remote name "origin". That means that when you push changed files to origin, you are pushing the files to the repo that you cloned from. For example, if you cloned from a fork, you will be pushing to the fork. If you cloned from an organizational repo, you will be pushing to the organizational repo. Then, you will submit a pull request from there.

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### General Branch Process

Perspective: 

Clone an organizational repo (organizational repo will be "origin")

```bash
$ git clone https://github.com/<organization-name>/<repo-name>
```

Clone a user account repo (repo needs to have already been forked to user account, forked repo will be "origin")

```bash
$ git clone https://github.com/<user-name>/<repo-name>
```

Change directory (folder name will be the repo name)

```bash
$ cd <repo-name>
```

Verify which branch you are checked out on (important if more than one branch)

```bash
$ git branch
```

Create and switch to a branch (note how local files switch to the files of the branch you switch to)

```bash
$ git checkout -b <branch-name>
```

If not working from within the branch you are branching off of, need to specify which branch branching off of

```bash
$ git checkout -b <branch-name> <branch-branching-off-of>
```

Make your change to the files, then add, commit, create a message

```bash
$ git add .
$ git commit -m "Your note"
```

Push branch to GitHub

```bash
$ git push origin <branch-name>
```

There will now be a new branch in the repo that is your origin. The branch will not be affecting anything else. 

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### How to Add Additional Commits

You can continue to push changes to the branch. Anyone else who has read/write access to the branch can also fetch it, make a change, and push to the branch too. The process is the same as earlier. If a pull request has already been made, the additional commit(s) will be automatically added to the pull request. 

Add, commit, create a message

```bash
$ git add .
$ git commit -m "Your note"
```

Push changes to GitHub

```bash
$ git push origin <branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### Submit a Pull Request

In the browser, go to the repo you want your pull request to be merged into. There should be a message prompting you to submit a pull request because GitHub will detect your branch. Be forewarned, that if you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure that base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, you might want to leave the box checked to give repo maintainers permission to amend the pull request. This gives them read/write access to the branch and later I'll explain how to amend it.
* Create the pull request

Like I said earlier, you, or anyone with read/write access to the branch, can continue to make changes to the pull request until it is merged.

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### What Are You Doing When You Review a Pull Request?

Switch perspective: now a maintainer working from within an organizational repo, with read/write access to the organiational repo, but without read/write access to a forked repo, unless permission has been given to amend a pull request.

If you are a repo maintainer, firstly, you will receive a message to let you know there is a pull request (by browser or email, based on your notification preferences). You go to the pull request and look at it in the browser. The pull request is in the form of a branch. Let's say, you have the organizational repo cloned to your computer and you are working from within it. If needed, you will fetch the pull request branch to the folder and switch to it. You can then run the code and evaluate the change. An example would be a website. Within the pull request branch, you can go through the normal setup process, then run the website code. You will look at the website in your browser as it runs on a local server to literally see the change proposed by the pull request. You then decided how to proceed.  

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### Code Review Options

* When you look at the pull request in the browser, you can tell it can be accepted (for example a typo) and click merge
* You run the code locally, but you do not need to make a change; you go back to the browser and click merge
* You run the code locally, and you think a change needs to be made; you ask the contributor to update the pull request
* You run the code locally, and you think a change needs to be made; you update the pull request branch locally (add, commit, create a message), merge the branch locally via command with the branch it is intended to change, and push to GitHub
* You run the code locally, and you think a change needs to be made; you push additional commits to the pull request

<!--
Check out pull request, run it like normal, for instance, a website

- [ ] Fetch an organizational pull request
- [ ] Merge pull request via browser- regular, squash, or rebase
- [ ] Merge pull request via command line
- [ ] Request a review from a specific person
- [ ] Close pull request via browser
- [ ] Close an issue via commit message by using keyword
-->

By the way, you can sometimes make a change to the pull request inside of the browser

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### Pull Request Process

When you go to the pull request in the browser, there will a set of instructions for reviewing the pull request locally (on your own computer). The set of instructions will be slightly different depending on whether the pull request was submitted via "Fork and Pull" Model (remote branch) or "Shared Repository" Model.  

I actually want to show you a slightly different way to do it that I think is easier to understand. 

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### Simple Code Review Process

Fetch the individual pull request into your folder

```bash
$ git fetch origin pull/<pull-request-number>/head:<branch-name>
```

Switch to the branch (note how local files switch to the files of the branch you switch to)

```bash
$ git checkout <branch-name>
```

Make your change to the files, then add, commit, create a message

```bash
$ git add .
$ git commit -m "Your note"
```

Push additional commits to organizational repo pull request

```bash
$ git push origin <branch-name>
```

Push additional commits to forked repo pull request (contributor needs to have given permission, and local branch name and remote branch name need to match)

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo pull request if local branch name is different than pull request branch name

```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

<!--
git fetch origin pull/8/head:Mariatta-patch-1
git push https://github.com/Mariatta/practice Mariatta-patch-1
git push https://github.com/Mariatta/practice Mariatta-patch-1-test:Mariatta-patch-1
-->

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Forked Repo Model Pull Request

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Shared Repo Model Pull Request

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Tidy Up

<!--
* [Viewing Branches in Your Repository](https://help.github.com/articles/viewing-branches-in-your-repository)
-->

* Close pull request
* Revert pull request (if needed)
* Delete feature branch (local and remote)

Delete a branch

```bash
$ git branch -d  <branch-name>
```

Force delete branch

```bash
$ git branch -D  <branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Should Your Project Use a Develop Branch?

Some projects will involve both a master and develop branch. For example, a mission critical project with a high volume of users is likely to use a develop branch and staging to gate-keep updates before going live. Use the workflow that is right for the projects. They all have pros and cons. 

If you choose to use a develop branch:
* In addition to the master branch, create the develop branch
* Choose a default branch

If you want to know much more about this, see: A Successful Git Branching Model.

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### Go Further with Advanced Workflow

* Git Flow (similar to process I’ve explained)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer

</td></tr>


<tr><td width="30%">

![Slide 34]()

</td><td>

### 10X Developers

</td></tr>


<tr><td width="30%">

![Slide 35]()

</td><td>

### Documentation

<!--
### Communication- General

- [ ] Create and implement your communication strategy
- [ ] Draft community guidelines
- [ ] Get to know GitHub Flavored Markdown

### Documentation- Forums

- [ ] Understand what wikis is
- [ ] Understand what GitHub pages/Jekyll are
- [ ] Understand what gists are

### Documentation- Files

- [ ] Make a README.md
- [ ] Make a LICENSE (auto-generate)
- [ ] Make a CODE_OF_CONDUCT.md (auto-generate)
- [ ] Make a CONTRIBUTING.md
- [ ] Make a PITCHME.md

# Issue and Pull Request Documentation

- [ ] Make an ISSUE_TEMPLATE
- [ ] Find the Issues Tab
- [ ] Make a PULL_REQUEST_TEMPLATE
- [ ] Find the Pull Requests Tab
-->

</td></tr>


<tr><td width="30%">

![Slide 36]()

</td><td>

### Productivity Helpers

<!--
- [ ] Cache your password
- [ ] Set up special configs (example: line endings)
- [ ] Create saved replies
- [ ] Link to specific line number on GitHub
-->

</td></tr>


<!--
What Could Go Wrong?
Setting Up Repo Fail Safes
- [ ] Create a repo backup (third-party softwares)
- [ ] Protect your main branch(es)
- [ ] Require reviews for pull requests
- [ ] Require external status checks
- [ ] Delete a non-important branch locally and attempt to recover it!
- [ ] Create a dummy sensitive information file and remove it from the history
-->

<tr><td width="30%">

![Slide 37]()

</td><td>

### Go For It!

Tips for getting started:

</td></tr>


<tr><td width="30%">

![Slide 38]()

</td><td>

### Debunking Myths

</td></tr>


<tr><td width="30%">

![Slide 40]()

</td><td>

### Thank You :)

Useful Resources: Bitly Link

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>


</table>

## Useful Resources

GitHub and Bitbucket
* [GitHub](https://github.com) examples
* [Bitbucket](https://bitbucket.org)

Getting Set Up
* [Set Up Git](https://help.github.com/articles/set-up-git)
* [Getting Started Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [Homebrew Git Formula](http://braumeister.org/formula/git)

Git Official 
* [Git Homepage](https://git-scm.com)
* [Git Doc (Docs and Pro Git Book](https://git-scm.com/doc)
* [Git Documentation](https://git-scm.com/documentation)
* [Git Pro Git Book](https://git-scm.com/book/en/v2)

Glossaries and Cheatsheets
* [GitHub Glossary](https://help.github.com/articles/github-glossary)
* [Git Cheatsheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
* [GitHub Git Cheatsheet](https://help.github.com/articles/git-cheatsheet)

GitHub Help and Training
* [GitHub Help](https://help.github.com)
* [GitHub Guides](https://guides.github.com)
* [GitHub Training Guides YouTube](https://www.youtube.com/githubguides)

GitHub Try
* [Try Git](https://try.github.io)
* [GitHub Bootcamp](https://help.github.com/categories/bootcamp) 
* [GitHub Hello World Tutorial](https://guides.github.com/activities/hello-world)

GitHub Learning Resources
* [Git and GitHub Learning Resources](https://help.github.com/articles/git-and-github-learning-resources)

GitHub Open Source Guides
* [Open Source Guides](https://opensource.guide)

Collaborative Development Models and Permission Levels
* [About Collaborative Development Models](https://help.github.com/articles/about-collaborative-development-models)
* [Types of Collaborative Development Models](https://help.github.com/enterprise/2.7/user/articles/types-of-collaborative-development-models)
* [Permission Levels for an Organization](https://help.github.com/articles/permission-levels-for-an-organization)
* [Repository Permission Levels for an Organization](https://help.github.com/articles/repository-permission-levels-for-an-organization)
* [Permission Levels for a User Account Repository](https://help.github.com/articles/permission-levels-for-a-user-account-repository)

Advanced Collaborative Development Workflow Examples
* Git Flow
* [A Successful Git Branching Model](http://nvie.com/posts/a-successful-git-branching-model) (more advanced)
* [A Successful Git Branching Model Considered Harmful](https://barro.github.io/2016/02/a-succesful-git-branching-model-considered-harmful)
* [SemVer](http://semver.org) (subtopic)


* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)
