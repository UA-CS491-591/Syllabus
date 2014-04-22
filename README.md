![Screenshot](https://raw.github.com/UA-CS493/Syllabus/master/Resources/Images/header.png)

Maintainable and Scalable Systems through Collaboration, VCS, and Open Source Software (CS 493)
========

The class syllabus lives here. Make sure to watch this repository so you can be notified if things change. You can click the little eye at the top of the page to change your settings so you receive email notifications if things change. This class is highly experimental in its techniques and class structure, but is actually very modern in its approach to using the current and respected tools of the day for efficient and maintainable software engineering practices. Below you will find the meta about the class as well as a tentative schedule of assignments and tests. Happy Coding!

## Table of Contents
* [Class Structure](#class-structure)
* Topics
  * [Mac Crash Course](#mac-crash-course) -History,core,apps,navigation
  * [Git and Github](#git-and-github)
     * [Git Basics](#git-basics) -dvcs,repositories,line change tracking, the origin
     * [Git Usage](#git-usage) -push,pull,clone,commit
     * [More Git](#more-git) -ignore, branch/merge, gitflow, tagging, stashing
     * [Github Basics](#github-basics) -registration,star,fork, watch, trending, gists, collaborators, readme/markdown, repository creation/rename/deletion, issue tracking
     * [Github Best Practices](#github-best-practices) -releasing, semantic versioning, being considerate
     * [SourceTree](#sourcetree) -installing,connecting github (or any .git endpoint),using sourcetree,
     * [Other Technologies](#other-technologies) SVN,mercurial,tfs
  * [IDE Basics](#ide-basics)
     * [Installation and Setup](#installation-and-setup)
     * [First App](#first app)
     * [Getting Around](#getting-around) - editor,project nav,console,debugger
     * [Project Structure](#project-structure) - mvc,entry points, good organization,searching,theming,resources,virtual folders
  * [OOP Basics](#oop-basics)
     * [Classes and Objects](#classes-and-objects)
     * [Inheritance](#inheritance)
     * [Variables](#variables) - private, public
     * [Methods](#methods) - static,non-static,inherited(overrrided methods)
  * [Objective-C](#objective-c)
     * [Class Structure](#class-structure) -.h,.m,interface
     * [Variables and Properties](#variables-and-properties)
     * [Methods in Objc](#methods-in-objc) +,-,public,private,no parameter,single parameter,calling
     * [Includes](#includes)
  * [iOS SDK Basics](#ios-sdk-basics)
     * [] 
     * [Data Structures](#data-structures) - NSArray, NSDictionary (NSSet) 
  * [](#)
  * [](#)
  * [](#)
  * [Guest Speaker](#guest-speaker)
  * [Android Dev](#android-dev)
  * [Deploying Apps](#deploying-apps)

## Class Structure

The bulk of this class will be entirely run on the GitHub platform. GitHub is a social coding tool that emphasizes Open Source and creative collaboration. GitHub is built entirely off of the [Git](http://en.wikipedia.org/wiki/Git_(software)) distributed version control platform. Git is used in development teams around the world for maintaining code bases in an extremely efficient manner, as well as being a tool for pushing code to production servers and maintaining a record of pushes to track down and eliminate bugs before they become a problem.

**Get a GitHub Account!**

First things first - you have to have a GitHub account. No account, no grade. You can create a free account by clicking the sign up button in the top-right of the browser window. Don't read any further until you have created your account.

**What you're graded on**
* 8 Assignments (40% of your grade)
* 2 Tests (60% of your grade)

That's it. There are no papers and no extra-credit.

## About the Assignments

Each assignment will be a separate repository inside of the UA-CS493 organization, and those links can be found in each Assignment section in this Syllabus as they are posted. Assignments in this class aren't your typical CS assignment; each one is created, maintained and graded through GitHub. Each assignment contains a <code>README.md</code> file in the top-level directory of the repository which contains all of the information about the assignment, the rubric used to grade your assignment, and any instructions/tips necessary to complete the project. Below is the order of operations of beginning, working on, and completing an assignment.

**Order of Operations**
* Fork the assignment
* Create a new folder with your name in the top-level
* Work on and complete the assignment inside your own Forked version of the repository
* Once completed, open a Pull Request to merge your repository with the master class repository
* Ace the assignment! (if you did well, of course)
 
**Committing your Work**

A commit is the process of saving the state of your work, which you can revert or look back onto any time you wish. This is very helpful for tracking bugs that started after a certain commit, where you can look at not only what files changed, but also what lines of code are different - a useful tool for efficiently tracking and eliminating bugs/design flaws in larger systems. For these assignments, you should commit often - and a commit log will be checked to see your creative process through the duration of the course, and to verify assignments were completed on time.

**Forking Repositories**

If you look up at the top of the page, you'll notice a button under your username that says "Fork." What a fork does is take the repository and port it over to your code base. You can make edits, change things and then commit - all without affecting the master repository you forked from. This enables you to do the assignment, until you're happy with the result and then you can make a Pull Request to "turn it in."

**Pull Requests**

A Pull Request is the process of merging the changes in your forked repository into the master repository. This works by finding differences in the files you forked and adding them in. A full history of your git commits is added into the master commit logs as well.

**GitHub Issues**

Issues are an auxilliary part of the GitHub platform; a separate tool built to be used in conjunction with Git. We are going to use Issues in this class to provide feedback on assignments, ask for help on assignments, and to show where in your commit history you were doing good things, or where things went wrong. This is an extremely helpful tool for collaboration as you will see in your group assignments in this class.
