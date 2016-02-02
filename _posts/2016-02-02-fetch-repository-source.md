---
layout: post
title: "Feature: Fetch source code from repository in a Hackathon"
description: "New feature which allows a team to fetch source code from a
public repository."
category:
tags: [Hackathon, Sprint, Feature]
---
{% include JB/setup %}

Teams or individuals participating in a hackathon on HackerEarth now have the option of fetching their source code as a zipped file from a public repository.

### How to use this feature ###

Whenever you submit or edit your hackathon project, you'll see a new checkbox below the repository link field. All you have to do is enter the public github or bitbucket repository URL and the zipball of the repository will be fetched automatically and attached in the source code field of the submission.

Please refer to the screenshot below -

<img src="/images/sprint_repo_fetch.png"/>

The repository is fetched asynchronously and does not block your submission process. Once you submit your project with the option checked, you'll see the status on the right panel. Please keep in mind that the status will only be updated once you refresh the page.

<img src="/images/sprint_repo_fetch_2.png"/>

If the fetching is successful, you can view your submission using the 'View Submission' button. Here, you can verify if your source zipball has been properly attached to your submission.

<img src="/images/sprint_repo_fetch_3.png"/>

This feature will definitely help save a lot of time for the teams, especially when they are on a low bandwidth internet connection.

*Posted by [Arindam Mani Das](http://hck.re/arindam/).*  
*Follow me [@arindammanidas](http://twitter.com/arindammanidas)*

