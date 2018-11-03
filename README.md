# Design Justification - G.T.H.C. </br>
This document serves to describe how the team justified the design of the software the way that this project is laid out. 

# Deciding Design </br>
Website Design </br>
In the beginning we were not certain whether we should create our own designs or use a pre-existing template. And if we were going to choose a pre-existing library, which library should we choose and for what reasons. We decided to choose a design that best fit these criterias
1. Flexible features that can be used on both React and React Native
2. Members of the team have experience with the design 
3. Library most user friendly with the WIX calendar library we are using for the MVP of the product 

Backend 
We were unsure of whether to use a SQL or a NoSQL database. Our team members have experience building databases using PostgreSql and writing functions that could query data. However, we had heard about useful third party Databases like Firebase, Parse, Kinvey, etc. 

# Choice Ultimately Made </br>
# Material UI → Makes up the Icons, Containers, Nav, Organization </br>
Material UI was our choice we ultimately made for the library that we intended to import into our design considerations. 

Justification: 
1. Flexible features that can be extended to many applications of use
2. Created by Google; therefore, open source code is reliable on multiple platforms
3. Teammate has experience working with Material UI before. Therefore, decreasing learning curve
4. Material UI easily compatible with other frameworks as well 
5. Easy to work with → simple imports into our script
6. Clean designs in the library
7. Importing icons were key in our project

Alternatives/Tradeoffs: 
React Toolbox
 1. React Toolbox Advantage </br>
    i. React Toolbox library is written with style-components which is consistent with React Code </br>
    ii. Most amount of documentation on React and ReactToolbox </br>
 2. React Toolbox DisAdvantage </br>
    1. It is not coupled with React, can be used with any 3rd party JS platform...important if we use Angular, Vue, etc. for further editions of the product </br>
    ii. JSS is easier to mount, which is important with sharing and manipulation of data in our application 
Team Members don’t have experience with this platform </br> 

Assumptions: </br>
1. Material UI is built by Google so it has performed multiple tests on Internet based platforms. 
2. Material UI is the most popular React platform being used right now, so it probably is the best and encompassing what we are working on

Dependencies: </br>
Material UI is compatible with few of the calendars we were deciding from. One of the Calendars had been built on Material UIs design, while the other was built on React Bootstrap. The functionalities of both calendars were the same. The Material Ui dependant one won!! </br> 

# Firebase API → </br>
The API for our backend was something we have been contemplating on. We ultimately came upon the decision to utilize Firebase our main database. </br> 

Justification: 
1. Real time data synchronization with app and backend
2. NoSQl and data already managed by application 
3. Commonly utilized database that has a lot of documentation on its use 
4. Created by Google; therefore, open source code is reliable on multiple platforms
5. Secure database which was necessary for storing personal information and demanded by our clients 
6. Consist of notification, messaging, and other api endpoints 

Parse-Server
1. Advantages </br>
<ul> Completely open source, not dependant on price model </br>
<ul> Provides you a very complete range of prebuilt SDKs to plug into your app project </br>
<ul> Comes with a plethora of features that offer a better user experience </br>
2. Disadvtanges </br>
<ul> It’s not multi-tenancy App compliant </br> 
<ul> Does not have messages as a feature -> future edition of the app </br> 

Postgre
1. Advantages </br> 
All of us have built a PostgreSQL database
Aman had already built out database for previous project
Data organized
2. Disadvantage </br> 
No Realtime database synchronization
Data is not visual organized for developers
Does not have API endpoints already implemented 


# Updated Test Plan - G.T.H.C </br> 

This document serves to describe how the team intends to verify the project’s quality
such that anyone who understands the project can figure out how the individual features
will be tested. Both expected and unexpected input/interactions would be shown and
ensures this team is committed to providing a working project.

# Testing Goals and Strategies </br> 

The Game Tenting Help Center will serve as the forefront to Krzyzewski-Ville’s centralized communication. 
We continue to strive to achieve this goal and in order to do so, we have put forth the following testing goals and strategies: 

1. Deploy the application to focus groups and line monitors to see whether it would fit their needs during a real game situation 
2. Intend to deploy a beta version in KVille or simulation of KVille in order to see whether the application will be deployable in the spring tenting season
    a. Strategy → Use our resources and students right here at Duke to find little things the developer may not catch

# Resources </br> 
The core features of the first edition of the application include a schedule builder, push notifications, and proper user 
authentication. The schedule builder will need mock Tenter information including names, class schedules, and weekly times they 
can work shifts. This would include the user going in and submitting the information to the database. Another piece of essential 
information is tenting rules and information which will be implemented on the application in a step by step intuitive process for 
the user to understand. 

# Deployment </br> 
We plan to separate our test environment from our production environment by ensuring branches are utilized on our project Github. 
Our team intends to always have a working model on our test environment so that at any point we may be able to test it for our client
or any focus groups that can give us feedback. 

# Test Scenarios </br> 
The test scenarios are as follows: 
1. Functionality Testing <br />
    a. Online Code Checkers (W3C Validator, CSS, etc) <br />
    b. Purpose: See if application can run properly on most internet browsers including chrome and safari <br />
    c. Assumptions: OUR UI built out on material UI, assuming the designs will be consistent on each platform <br />
    d. Steps: Test Cases with Safari, Chrome, IE <br />
2. Navigation/Links/URL Testing <br />
    a. Internal Links <br />
    b. External Links <br />
3. Database Testing <br />
    a. Firebase Test -> Use the Firebase Test Plan <br />
    b. Purpose:  Make sure Firebase is updating application continuously <br />
    c. Assumption: Firebase is very reliable  <br />
    d. Steps: Documentation on Firebase Test plan <br />
4. Performance Testing  <br />
    a. Run Audit Testing <br />
    b. Utilize the Google Chrome Inspect Feature  <br />
    c. Audits Testing will give many performance details about the website on a scale of 1 to 100 <br />
5. Usability Testing <br />
    a. Feature: For Calendar and Tenting 101 Component <br />
    b. Purpose: Make sure product being made is what customers want <br />
    c. Assumptions: our designs is not the best but we can improve on it <br />
    d. Steps: Multiple iterations <br />
    e. Outcome: more intuitive calendar UI and tenting 101 <br />
6. Other Error Testing <br />

Each test scenario above will include:
1. Label or ID
2. Feature
3. Purpose
4. Pre-conditions (assumptions)
5. Steps
6. Post-Conditions (expected outcome)

<br />
<br />

# Release Management Plan - G.T.H.C </br> 

This document serves to describe how the team intends to manage the release of the application so that anyone can read and understand how our application will be distinguished from the current development version as well as any dependencies. This document serves to clarify packaging and delivery for our product. 

# Software Configuration Management (SCM) </br> 

Our team intends to ensure that the dynamically changing aspects of our products are clearly laid out. Any kind of change or modification to the application in the future will have to go through the following steps: 

1. Change proposal 
2. Identify components that are needed to be changed
3. Review and evaluate that proposal 
4. Approve or Deny the change
5. Implement change 
6. Test the change
7. Notify users after fully accepting the change 

By going through these thorough steps for any kind of modification, we can ensure that the client will be satisfied when we need to roll through with any changes/modification. Ideally, the changes are implemented in the offseason of tenting so that taking down and putting the site backup is not a problem. However, if any immediate altering is necessary then we will implement as needed. 

Technicalities:
Before making a release, we will need to have the features of a release broken down into tasks for each team member to work on. Each task will be worked on it’s own branch, and a completed task will be assigned to a Pull Request. This will allow us to individually test each tasks and/or features before merging them and sending it into production. Moreover, using pull requests will allow us to setup Continuous Integration tools such as CircleCI or Travis to automate tests to make sure the new feature is functional on the higher level, and it is also the responsibility of other team members to review their peers’ Pull Requests before pushing onto a higher branch. Reviewing Pull Requests require the reviewer to look both at code quality and functionality before approving a merge. Each Pull Request has been set up to require team approval before pulling. Overall, the stages are the following:

Standalone branch for feature/task → Pull Request → CI → Team Approval → Staging Branch (Built and Deployed on staging) → Master Branch (Build and Deployed on production)


# Build Management </br> 

At the moment, Heroku is our cloud platform of choice because it handles automated build process when deploying our projects. With Heroku’s automated deployment, we can make changes to our staging branches to our GitHub repositories (which Heroku can gain direct access to), and automate the entire build process from the moment that a pull request is given access to merge onto the staging branches.

# Packaging </br> 
As we are using the node js framework, all of our dependencies are managed by node’s packaging manager (npm), and in both development and on our production build, we use yarn as our main dependency management tool, which has been proven to be a faster, more space efficient, and a better developer experience alternative to npm.   

# Releasing to Production </br> 
When building any application that will eventually go into development, the main goal is to always replicate the production environment in development. Typically, the best solution is to set up a container that has its environment setup in a uniform fashion. For example, a docker container running an instance of ubuntu that has the same installation process each time you run it up for any depencies you may need, such as npm, and react. Due to the complexity and general team experience, we have decided to manually maintain a uniform environment in development. Maintaining our environment will make deployment to production much easier, as we can be assured with what works and does not work in development will be the same in production. Before releasing, we follow the steps mentioned above in SCM, and we will use our cloud platform (most likely Heroku, but could potentially be GCP or AWS) to build, run, and host our application. 

# Defect Tracking </br> 
As mentioned before, we can use a Continuous Integration (CI) tool, preferably CI, that will run tests automatically on PR before merges are allowed to catch any defects that we test for. This is useful because it will stop us from pushing defective code.

</br>
</br> 

# G.T.H.C. Project Plan 

This document clarifies the order of the project’s features and a thorough analysis of what is to
come. The document specifies the delegation of responsibilities between the team and our
project timeline to include making our short-term and long-term goals.

# Team Roles:

1. The following team roles have been delegated: <br />
    a. Web Application Development → Aman, Rikki <br />
    b. Mobile Application Development → Vinit <br />
    c. Design → Vinit, Rikki <br />
    d. Backend → Aman <br />
    e. Project Liaison to Client → Vinit <br />
    f. Project Liaison to Line Monitors → Rikki <br />

# Project Timeline

Sprint #2 <br />
    ❏ September 24th → Project Plan Gitlab Wiki <br />
    ❏ September 28th → Project Plan Gitlab Issues <br />
    ❏ September 25th → Prototype 1st Stage <br />
    ❏ September 28th → Prototype with basic features <br />
    ❏ September 29th → Client Demonstration, Team Sprint Report <br />
    
Sprint #3 <br />
    ❏ October 10th → Baseline Prototype With Core Functionality <br />
    ❏ Prototype Demonstration <br />
    ❏ October 24th → Baseline Demo <br />
    
Sprint #4 <br />
❏ October 31st → Alpha (Partial Functionality) <br />
❏ Alpha Demonstration 

Sprint #5 <br />
❏ November 14th → Beta (Full Functionality) <br />
❏ User Testing <br />
❏ November 28th → Beta Demonstration <br />

Sprint #6 <br />
❏ December 5th → Robust Full Functionality <br />
❏ December 10th → Technology transfer to client <br />

# Backlog & User Story
The following is a breakdown of the list of features for the project. <br />

Sprint #2 - Basic Features <br />
➢ The Prototype would include the following basic features: <br />
○ User Authentication <br />
○ Team Creation <br />
○ Basic calendar/schedule <br />
○ Navbar and Tabs <br />
○ Basic layout and navigation <br />

Sprint #3 - Core Functionality <br />
➢ This sprint will go more in depth on features including: <br />
○ Full Calendar/Scheduling <br />
○ When2Meet type functionality to record user availability <br />
○ Simple dashboard widgets to visualize important user data (Such # of 
hours spent tenting per teammate, upcoming information from line
monitors, etc.)
 
Sprint #4 - Partial Functionality <br />
➢ By this sprint, we intend to implement the following: <br />
○ Adding and Changing Shifts <br />
○ Full functioning dashboard <br />
○ Deploy project using one of many available cloud platforms (Google
Cloud, AWS, Heroku, etc.)

Sprint #5 - Full Functionality <br />
➢ The finishing touches and improvements would be made including the following: <br />
○ Final design <br />
○ Improvements from user testing <br />
○ Add data security <br />

    
    
