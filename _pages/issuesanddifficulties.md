---
layout: page
title: Issues and Difficulties
include_in_header: true
---

# *What took the most time? The least? Any surprises?*

Throughout the development process of the app, there were a few scenarios in which more time was allocated to completing and implementing certain tasks and features compared to others which seemingly had much less overall time spent on them compared to the more time-intensive tasks. The following three tasks appeared on both ends of the spectrum and varied in the time spent taken to fully complete.

## **Database**

Out of all the tasks and features implemented through the entirety of the apps development time, setting up, and testing that the database was correctly implemented took by far the longest out of any feature or task combined, managing to carry over across all iterations. The key challenges that contributed to such a long development time were:

### *Lack of Documentation*

* When working with HSQLDB, we encountered a lacking amount of documentation on the subject. This lack of resources meant we had to rely heavily on forums to find solutions that others may have found, trial-and-error methods, and then mercilessly testing it to ensure all dependencies were set up properly and that tables would connect with each other as initially planned.

### *Library Imports*

* We had to spend a significant amount of time ensuring that we were importing the correct versions of certain libraries, configuring them properly, and resolving any conflicts that arose because of them. Like the previous point, a lack of documentation on necessary imports and understanding what exactly was required caused the specifics of library imports in android studio to also take a large chunk of time in handling.

### *Database Storage Location*

* Determining where the database file should stored and figuring out how to directly access it was another hurdle that cost plenty of time. We had to refactor some of our folders at this point such that the folders, and its files could correctly point to the location with our data base. Ensuring that the data persistence was being handled properly was also at the crux of this issue as we also required verification from each instance of database access since we needed to confirm if data was being written to and retrieved properly.

### *SQL Language Differences*

* HSQLDB had its own set of SQL syntax and features that differed from what we learned in COMP 3380. Thus, we had to modify our queries to adhere to the specific functionalities and limitations of HSQLDB’s SQL implementation. This process, while not as time consuming as some of the other aspects still took time to get adjusted to, as expected with learning a similar query language.

### *OS Dependencies*

* The way the database file for our app was handled varied depending on the operating system of whoever was running tests. Issues related to file permissions, paths, and retrieval methods were noticeable when trying to run the tests on Mac vs. Windows. This added complexity to the testing phase as we needed to find ways to avoid platform-specific issues before an iteration release in the event that whomever may be running tests may do it on a platform that had issues before.

Overall, this process was full of surprises and required a lot of trial and error. However, the effort paid off as it allowed us to circumvent future issues and achieve a stable setup for usage and future testing.

## **Search Feature**

### *Planning*

* One aspect of the *search* feature taking so long is because it was a task that we underestimated the time for before the iteration began. In hindsight we should have had two developer task tickets instead of 1, in other words, we should have split the general "search" term into both a "campaign search" and "user search". We didn't account for the fact that there was two different entities we would be searching for, which caused the innaccurate times due to miscommunication of the feature.

### *Database Functionality*

* While the feature itself was still in development, our group was still in the process of setting up the database alongside making this feature, so there were some delays in the process because the campaigns specific database functionality wasn't set up at that point. Meaning we had come to the decision to temporarily stall the search feature until the database functionality had been set up. This aspect also plays into the previous aspect in how we should have split this developer task up even further.

### *Small Bugs*

* In the initial implementation of the search feature, we didn't think to account for wildcard characters, which was a bug we later had to fix causing a delay in the expected completion time of this feature. These characters were often non-alphanumeric characters like **'_', '-', '/',** and so on.

### *Query*

* The query itself took some time to implement from the preperation phase, but was the most interesting and fun part of the feature. We wanted an SQL query that provided the search results by order of compatibility based on the tags attached to a specific user via their profile page. Because of the way this query was to be implemented, it resulted in many ways that a user could search as they could use a mix of both user tags and specific user names or campaign names.

### *Potential Technical Debt*

* **LIKE** is the operator that we chose for searching by user names and campaign names, however, LIKE is very case-sensitive, so this is technical debt which could unintentionally hide specific users or games from users due to a character being accidentally upper or lower-case.

Overall, the search feature, while it was by far the most interesting and rewarding to implement, saught a lot of database and implementation related issues that resulted in the actual completion time exceeding the expected completion time by a fair bit.

## **Matchmaking Feature**

One of the most surprising features from all iterations in terms of implementation was the matchmaking, feature, of which we had initially thought would require an allocation of time similar to how search was implemented. The result however was that implementing the search feature first took nearly all the weight off of the actual implementation, only requiring a small change in the paramaters of a search query.

Because of this, we had drastically over estimated the difficulty and expected time of this feature which resulted in our group being surprised with just how quick we were able to get through the task. Due to such an over estimation and under estimation for tasks related to finding other players and games through our app. 

## **Overall**

We learned from the issues faced in iteration 2 and used them to make sure that with iteration 3 underway, that we were now properly considering whether a task was being split up fairly by making sure no specific developer task overweighed others in terms of expected time to completion. With a more streamlined process, we can now recognize a potentially larger task right from the get-go instead of struggling with a task midway through development, refining our task breakdown, preperation, and consideration to be more reflective of the experience we gained working through some of the troubling and surprising aspects of features and database development that varied in a large and small amount of wasted time.