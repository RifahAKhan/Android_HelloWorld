# Project build to understand the concepts of Git and GitHub.
> Summarizing the concepts learnt.
* Created a project in [Android Studio](https://developer.android.com/studio)<br/>
*Before installing Android Studio make sure that you've installed JDK on your system*\
*https://www.oracle.com/java/technologies/downloads/*<br/>
* Created a GitHub repository<br/><br/>
## **Important Commands**
  1. Learnt to initialize an empty Git repository at a specific location.
  2. Learnt to stage or add files.
  3. Learnt to commit and update the changes made.
  4. Learnt to link GitHub repository to local Git.
  5. Learnt to push commits in the local branch to remote branch.

## **Branches**
  1. Created Multiple Branches and learnt to push branches created in the local repository to remote repository.
  2. Created a branch within another branch and learnt to change text and push it to the GitHub repository.
  3. Learnt how to switch between branches and also display the list of branches created.
  4. Learnt to create and merge pull request.
  5. Learnt how to pull the updated code from GitHub to local repository.
  6. Learnt how to delete and also forcefully delete a branch.
  7. Learnt how to resolve conflicts when merging branches.

      ### *<ins>Why do conflicts occur when we merge branches?* :raised_eyebrow:
      A conflict arises when two separate branches have made edits to the same line in a file, or when a file has been deleted in one branch but edited in the other.
      A merge conflict is an event that takes place when Git is unable to automatically resolve differences in code between two commits. Git can merge the changes automatically 
      only if the commits are on different lines or different branches. Assume that there are two developers A and developer B. Both of them pull the same code file from the
      remote repository and try to make various changes in the file. After making the changes, Developer A pushes the file back to remote repository from his local repository.
      Now, when Developer B tries to push that file after making the changes from his end, he is unable to do so, as the file has already changed in the remote repository.
      To prevent such conflicts, developers work in separate isolated branches. The Git merge command combines seperate branches and resolves any conflicting edits.

      ### *<ins>What are the two types of Merge conflicts?*
       1. **<ins>Starting the merge process**\
       If there are any changes in the working directory's stage area for the current project, merging won't start.<br/>
       In this case, conflicts happen due to pending changes that need
       to be stabilized using different Git commands.

       2. **<ins>During the merge process**\
       The failure during the merge process indicates that there is a conflict between the local branch and the branch being merged.<br/>
       In this case, one can resolve conflicts in the terminals section in android studio or directly make changes in GitHub and then merge.

### <ins>*What are the steps involved in the prodution process of an application also called as CICD Pipeline?*
### <ins> What is a Pipeline?
It is a logical step or a series of steps which define how software development life cycle occurs.
### <ins>*What is DevOps?*
DevOps is a software development approach which involves Continuous Development, Continuous Testing, Continuous Integration, Continuous Deployment and monitoring through its
development cycle.

#### <ins>*Stages involved in DevOps*
  1. **<ins>Version Control System- Source Code Management** : Maintains different versions of the code.
  What deoes version mean?
  Consider that there are multiple developers writing a code for a particular application. Then, How will the lead know which developer has made what commit at what time and
  exactly which commit is causing the error and if the lead wants to revert back that particular commit and make changes? So, this can be managed by using Version Control or 
  Source code management like Git, Subversion etc.

  2. **<ins>Continuous Integration - Continuous Build** : Compile, Validate, Code Review, Unit testing, Integration Testing
  It basically means building your application continuously. Consider that the developer wants to makes changes in the source code. Here the Continuous Integration server 
  i.e the Jenkins Server that is used must be able to pull the code and prepare a build using Maven or Gradle.
  What does Build mean?
  Build not only means compiling the code, but also validating, reviewing the source code and also performing Unit testing, Integration testing and Pachage Applications.
  What does Unit Testing mean?
  When the source code is devided to small individual chunks or parts and tested to check if it produces the desired result.
  What does Integration testing mean?
  When all these chunks or parts are integrated and tested to check if it produces the desired result.
  What does Packages in Android mean?
  Android Application Package(APK) is the package file format used by the Android Operating System for distribution and installation of apps and middleware. 
  Where Middleware is a software that lies between an operating system and the applications running on it.

  3. **<ins>Continuous Delivery - Continuous Testing** : Deploying the build application to test servers, performing UAT.
  4. **<ins>Continuous Deployment - Configuration Management and Containerization** : Deploying the tested application on the prod server for release.
  Consider a continuous Integration tool such as Jenkins that will deploy code(code deployment means that once the developer has written code for an application it has to be 
  placed on the servers that can contain code that fixed bugs, adds new features or upgrades the underlying platform) on to the test servers to perform User Application Testing
  with the help of tools like Selenium or J unit.
  What is UAT?
  This is the final stage of an Application development cycle.
  This is when the actual users test the application to see if it is able to carry out the required tasks it was designed to address in real-world situations.
  Once the application passes the UAT it is deployed onto the production or prod servers for release that is done by using Docker, Puppet etc. If this release is done
  automatically it is called Continuous Deployment and if it this step is done manually i.e if somebody has to approve it then it is known as Continuous Delivery.

  And now when the application is in life it is continuously monitored by tools like Nagios which will provide the relevant feedback to the concerned teams and once the 
  team gets the feedback they take the feedback and solve the bug and then the application again goes through the complete cycle. 

