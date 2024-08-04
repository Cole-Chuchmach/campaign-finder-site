---
layout: page
title: The Team
---

# *A list of the team members, the contributions they made, and the developmental skills they learned*

## Cole Chuchmach

### *Contributions Made:*

* Learned Jekyll and developed the 'CampaignFinder' project website. 
* Developed the UI and Logic for the login and create-an-account page:
    * Verifies that new account information doesn't consist of information that is already in use.
    * Verifies information provided for logging in before determining whether to admit the user.
* Developed the UI and Logic for the inner edit profile page:
    * Built a dynamic RecyclerView UI to show selected player tags and contact methods.
    * Created Java adapter files that bring up a small UI for selecting new tags and entering new contact information.
    * Implemented buttons for saving changes, logging out, and deleting an account.
* Implemented the logic for matching with other players based on user chosen profile tags.
* Developed a dynamic and abstract results page:
    * Allows for player specific results which include player names, title, and tags with the option to view their account.
    * Or, will present joinable campaigns which include the name, tags, and number of slots left, with the option to view the listing.
* Implemented a navigation bar present on all pages of the application to allow for easier traversal between pages.
* Tested application:
    * Unit testing in Iteration 1.
    * Both unit testing and some integration testing in Iteration 2.
    * Acceptance and System testing in Iteration 3.
    * Run throughs of the application in attempts to find ways to break or crash the application.

### *Developmental Skills Gained:*

* Familiarity with android studio and its UI interfaces.
* Learned how to write XML.
* Better ability to identify code smells, and how to mitigate them through refactoring.
* Learned how to write unit, integration, and acceptance/system tests.
* Identified a version control strategy that worked best for the team.
* Prepared for future iterations through planning boards and reflective estimates based on completed work.
* Communicated ideas and listened to/appreciated feedback on development tasks.
* Implemented features and its cooresponding code while keeping layers separated from each other.
* Learned how to handle exceptions on the back end while providing enough details to users on the front end.
* Successfully worked and collaborated on a project with multiple team members accessing it at once.

## Enoch Olaniyi

### *Contributions Made:*

* Gitlab Board Management (up to Iteration 2):
    * Organized and created features, developer tasks, and user stories.
    * Developed a storyboard to maintain consistency and transparency for all team members.
    * Conducted code reviews and enforced coding standards.
    * Labeled tasks to provide clarity for both markers and developers.
* Documentation Management (up to Iteration 2):
    * Created and maintained architecture documentation and diagrams.
    * Regularly updated project documentation and the hand-in package.
* HSQLDB Mock Database Development:
    * Designed database schema and table relationships specifically for stored objects.
    * Maintained the database with update, insert, and delete queries for all persistent objects.
    * Seamlessly integrated the database with the application, deprecating test stubs.
    * Implemented all necessary database functionality.
* UI and Logic Development:
    * Developed the UI and logic for the profile page, including creating a tag adapter class.
    * Developed UI and logic for campaign hosting and editing:
        * Implemented logic for saving changes and deleting campaigns.
        * Properly linked campaign objects to pages for accurate display of information.
    * Enabled object serialization for passing objects between pages.
* Major Code Refactoring:
    * Refactored the majority of the codebase in Iteration 2 to ensure proper layer separation.
    * Removed code smells and reinforced SOLID principles.
    * Moved logic from the UI layer to independent logic layers.
    * Separated the database layer from objects, implementing database calls in the logic layer.
* Error Handling:
    * Created the majority of exceptions and updated functions to handle errors appropriately.
* Testing:
    * Rewrote Iteration 1 unit tests in Iteration 2 and added new unit tests.
    * Developed all database unit tests for Iteration 2.
    * Imported and implemented Mockito for creating a mock HSQLDB database for testing.
    * Conducted manual stress tests on the UI during code reviews.

### *Developmental Skills Gained:*

* Technical Skills:
    * Gained familiarity with Android Studio, including its UI interfaces and component logic.
    * Improved ability to perform major refactoring and implement n-tier architecture.
    * Enhanced skills in identifying potential issues and code smells during reviews.
    * Developed a strong understanding of database relationships and query writing with HSQLDB.
    * Strengthened testing skills through the use of mock objects and stubs with Mockito.
    * Learned to properly import and utilize libraries such as Espresso and Mockito.
    * Implemented effective version control strategies for the team.
* Project Management:
    * Enhanced management and organization skills through planning boards and reflective estimates.
    * Prepared for future iterations by planning tasks and setting realistic deadlines.
    * Developed communication skills by sharing ideas and incorporating feedback from team members.
    * Successfully collaborated on a project with multiple team members working simultaneously.
* Best Practices:
    * Ensured code separation by implementing features and corresponding logic across different layers.
    * Handled exceptions on the back end while providing user-friendly error messages on the front end.

## Victoria Iskandar

### *Contributions Made:*

* For fun: contributed a architectural flow-chart <a href="https://www.figma.com/board/XWM954nIhiz7dwAMYjdJor/CampaignFinderTemplate?node-id=0-1">Figma diagram<a> for the entire application, which signifanctly help create a unified vision for the application’s UI and the flow of the app. 
* Wrote vision for project, the Coding Standards document, Velocity Graph, all the README’s, and the Retrospective document. 
* Created all DSO classes.
* Wrote all DSO class unit tests.
* Created the Sign In XML page.
* Chose the colour theme for the project for a uniform look (it’s not the prettiest, but it’s consistent).
* Generated artwork for the project using Bing Co-pilot.
* Built and refactored the logic/database functions for the Search feature, which included constructing a query that returns all users or campaigns that match a search criteria, in order of compatability with the logged in user via tags.
* Consistently provided code reviews, performed merge requests, and tested features to detect bugs (by interacting with the application), provided ideas and took feedback.
* Wrote the integration tests for Search feature (and matchmaker feature)
* Made the home page UI, and for host/manage campaign
* Consistently made bug fixes when bugs were discovered
* Organized Tasks and Issue board for Iteration 3.
* Refactored some of the java UI components so the code can be more re-usable (NavBarUtility, StringUtility, ProfilePicUtility, ToggleUtility)
* Refactored UI xml pages to utilize string.xml and themes.xml to reduce duplicated code and reduce warnings in Android Studio. 
* Wrote the System tests for host/manage campaign feature.

### *Developmental Skills Gained:*

* Learned XML, and how to work with HSQLDB for database connections.
* Learned how to build apps with Android Studio, and how to work with Java packages in Android Studio.
*  How to spot areas in code that can be refactored to reduce code duplication and smells, and provide more thorough feedback during code reviews.
* Learned that we could (in the future) set up the campaigns and campaign members objects to follow the Observer design pattern, so campaigns can notify their members of events.
* Successfully deployed a release on gitlab (and learned how that process is done)
* How to work with and properly organize issue board and break up user stories into dev tasks.
* Learned how to write unit, integration, and acceptance/system tests.
* Learned how to work with github flow version control and tickets on issue boards.
* Learned how to better use git rebase, thanks to Enoch’s help.
* Learned how to handle merge conflicts (while familiar, a little practice doesn’t hurt)
* Honed skills on reaching out to team members for advice or help: Cole was very helpful in picking up extra tasks, Enoch was always available to help when I got stuck. Francis was always willing to learn and pick up tasks, Mustaba offered great insight at the start for how to implement the stub database, and was always willing to help. I feel honoured to have learned from and worked with this team.
* Helped oranize team meetings to plan for future iterations. Was always available to help and answer questions.
* Communicated ideas and listened to/appreciated feedback on development tasks.
* How to develop for a specific layer, in isolation from others, without breaking the application.
* Learned that custom exceptions are always better than more general ones, and when to use them.
* Successfully worked and collaborated on a project with multiple team members accessing it at once.