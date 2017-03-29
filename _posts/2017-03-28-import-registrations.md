---
layout: post
title: "Feature: Import Registrations on Sprint"
description: "Import externally collected registrations for hackathons on to HackerEarth Sprint"
category:
tags: [HackerEarth, Sprint]
---
{% include JB/setup %}

Hackathon organizers can now import user registrations that they have collected from external sources onto HackerEarth Sprint. Post importing, the users will be registered for the hackathon and they will start receiving hackathon notifications from Sprint.

The process can be started by a click on the `Import Registrations` button on the `Registrations` tab of the `Admin Dashboard` of a hackathon.

<img src="/images/import_reg_step0.png">


The hackathon organizer needs to go through 5 steps to successfully complete the importing process.


### Step 1: Choose a file upload format (csv/xls/xlsx)
The import can be done via a csv or an xls/xlsx file. Each row in the file would represent a user, and each column would represent a specific data of the user.

<img src="/images/import_reg_step1.png">

### Step 2: Upload the file
The file uploaded can have a maximum size of 5MB.

<img src="/images/import_reg_step2.png">


### Step 3: File Meta Verification
Upon upload, the file will be checked if it contains atleast the emails of the users to be registered. An error will be raised in this case, prohibiting the process to continue until the right data is present in the file.

The system will also check what other data the hackathon organizer wants to collect but are missing from the file. It will raise a warning in this case, but will let the process to continue.

<img src="/images/import_reg_step3.png">


### Step 4: Setup custom email notification
The hackathon organizer may want to send a customized email to the user upon successful registration. This step can be skipped, and HackerEarth will send an auto generated email to the user. The user will receive his login credentials over email, if his account didn't exist at the time of importing.

<img src="/images/import_reg_step4.png">


### Step 5: Registering users
This is the last step where the users will be registered for the hackathon and they will receive an email notification about the same. All the admins of the hackathon will also receive an email with a detailed log of the import process upon completion.

<img src="/images/import_reg_step5.gif">

## Here is a visual representation of the entire process:

<img src="/images/import_reg_step6.gif">

Send any suggestions and feedback to *[sdeep@hackerearth.com](mailto:sdeep@hackerearth.com)* or *[support@hackerearth.com](mailto:support@hackerearth.com)*.

<i>Posted by [Souradeep](http://www.hackerearth.com/users/desouradeep/).
Follow me [@desouradeep](http://twitter.com/desouradeep).</i>
