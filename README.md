![Screenshot](https://raw.github.com/UA-CS493/Syllabus/master/Resources/Images/header.png)

Maintainable and Scalable Systems through Collaboration, VCS, and Open Source Software (CS 491/591)
========

The class syllabus lives here. Make sure to watch this repository so you can be notified if things change. You can click the little eye at the top of the page to change your settings so you receive email notifications if things change. This class is highly experimental in its techniques and class structure, but is actually very modern in its approach to using the current and respected tools of the day for efficient and maintainable software engineering practices. Below you will find the meta about the class as well as a tentative schedule of assignments and tests. Happy Coding!

<b>Where: </b> SERC 2039       <b>When: </b> 9AM-12PM

## Table of Contents
* [Class Structure](#class-structure)
* Topics
  * [Mac Crash Course](#mac-crash-course) -History,core,apps,navigation
  * [Git and Github](#git-and-github)
     * [Why we use VCS](#why-we-use vcs) - changes, sharing, tracking, versioning
     * [VCS Options](#vcs-options) - CVCS:SVN,TFS DVCS:git,mercurial,bazaar
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
     * [Class Structure](#class-structure) -.h,.m,interface, implementation
     * [Variables and Properties](#variables-and-properties) http://rypress.com/tutorials/objective-c/properties.html
     * [Primitives](#primitives) - int,float,double,char, short, long 
     * [Methods in Objc](#methods-in-objc) +,-,public,private,no parameter,single parameter,calling
     * [Imports](#imports)
     * [Protocols](#protocols)
  * [iOS SDK Basics](#ios-sdk-basics)
     * [SDK Primitive Aliases](#sdk-primitive-aliases) - NSInteger, CGFloat
     * [Data Structures](#data-structures) - NSArray, NSDictionary, NSSet
     * [Other Foundation Classes](#other-foundation-classes) NSDate,
  * [UIKit Basics](#uikit-basics)
     * [View Hierarchy](#view-hierarchy)
     * [No Storyboards](#no-storyboards)
     * [No Nibs](#no-nibs)
     * [Animations](#animations)
     * [Event Handling](#event-handling) Through nib and code only
     * [Navigation](#navigation)
  * [GCD, Concurrency and blocks](#gcd-concurrency-and-concurrency)
     * [Anatomy of an App](#anatomy-of-an-app)
     * [Blocks](#callbacks) http://rypress.com/tutorials/objective-c/blocks.html
     * [Basic Async Tasks](#basic-async-tasks)
     * [Callbacks](#callbacks)
     * [NSOperationQueue](#nsoperationqueue)
  * [Web Programming](#web-programming)
     * [The need for communication](#the-need-for-communication)
     * [The Internet Protocol Suite](#the-internet-protocol-suite)
     * [HTTP/HTTPS](#https/https)
     * [Ports](#ports) http://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers
     * [HTTP Request](#http requests)
        * [URL](#url)
        * [Verbs](#verbs) GET,POST,PUT,DELETE
        * [Headers](#headers) http://en.wikipedia.org/wiki/List_of_HTTP_header_fields
        * [Body](#body)
     * [Basic Web Calls](#basic-web-calls)
     * [Project API Reintroduction](#project-api-reintroduction)
        * [Web Methods](#web-methods)
        * [URL Breakdown](#url-breakdown)
        * [Data Interchange Languages](#data interchange languages) or "Organizing things in the message body"
           * [Why](#why)
           * [Popular Formats](#popular-formats)
           * [Breaking Down JSON](#breaking-down-json)
     * [NSObject+ObjectMap](#nsobject+objectmap)
  * [Testing](#testing)
     * [Why We Test](#why-we-test)
     * [Assertions](#basic-assertions)
     * [Library Testing Example (DateTools)](#library-testing-example-(datetools))
     * [Testing UI Components](#testing-ui-components)
  * [Maps](#maps)
     * [Setup](#setup)
     * [Basics](#basics) zooming,panning,tilting,map types,(reverse) geocoding,
     * [Render Hierarchy](#render-hierarchy)
     * [Annotations](#annotations)
     * [Layers](#layers)
  * [URI Schemes](#URI-Schemes)
  * [Third Party Libraries](#third-party-libraries)
  * [Cocoapods](#cocoapods)
  * [Guest Speaker](#guest-speaker)
  * [Android Dev](#android-dev)
  * [Deploying Apps](#deploying-apps)
     * [ItunesConnect](#itunes-connect)
     * [Archiving](#archiving)
     * [Analytics](#analytics)
  * [Resources](#resources) 

## Class Structure

The bulk of this class will be entirely run on the GitHub platform. GitHub is a social coding tool that emphasizes Open Source and creative collaboration. GitHub is built entirely off of the [Git](http://en.wikipedia.org/wiki/Git_(software)) distributed version control platform. Git is used in development teams around the world for maintaining code bases in an extremely efficient manner, as well as being a tool for pushing code to production servers and maintaining a record of pushes to track down and eliminate bugs before they become a problem.

**Get a GitHub Account!**

First things first - you have to have a GitHub account. No account, no grade. You can create a free account by clicking the sign up button in the top-right of the browser window. Don't read any further until you have created your account.


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


##Git and Github


####Why We Use VCS
- changes, sharing, tracking, versioning

 
####VCS Options
- CVCS:SVN,TFS DVCS:git,mercurial,bazaar


####Git Basics
-dvcs,repositories,line change tracking, the origin


####Git Usage 
-push,pull,clone,commit

####More Git
-ignore, branch/merge, gitflow, tagging, stashing

[Gitflow](http://nvie.com/posts/a-successful-git-branching-model/)

####Github Basics
-registration,star,fork, watch, trending, gists, collaborators, readme/markdown,

##Deploying Apps

####Apple Developer Site

[https://developer.apple.com/](https://developer.apple.com/)

The developer site handles signing of apps and provisioning devices

####Itunes Connect

[https://itunesconnect.apple.com/WebObjects/iTunesConnect.woa](https://itunesconnect.apple.com/WebObjects/iTunesConnect.woa
)

Itunes Connect handles deployment and app store analytics/management.

##Resources
Below are a list of blogs and tutorials that you may find helpful in learning objective-c
 
#### Language
* [Rypress Objective-C Tutorial](http://rypress.com/tutorials/objective-c/)
 
#### Platform
* [Ray Wenderlich Tutorials](http://www.raywenderlich.com/tutorials)
* [Appcoda Tutorials - No Storyboards](http://www.appcoda.com/ios-programming-course/)
* [Tutorials Point](http://www.tutorialspoint.com/ios/index.htm)
* [Start Developing iOS Apps Today](https://developer.apple.com/library/IOs/referencelibrary/GettingStarted/RoadMapiOS/index.html#//apple_ref/doc/uid/TP40011343-CH2-SW1)
 
Also, **[StackOverflow](http://stackoverflow.com/) is your best friend.** Google "iphone sdk" then whatever your question is for best results.
 
#### More Advanced
* [ObjC.io](http://www.objc.io/)
* [NSHipster](http://nshipster.com/)
