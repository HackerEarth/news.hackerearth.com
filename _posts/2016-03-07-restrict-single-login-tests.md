---
layout: post
title: "Feature: Restrict single login in tests"
description: "Restricting single login for a candidate for a test"
category:
tags: [Recruiter, Assessment]
---
{% include JB/setup %}

Candidates can be restricted from attempting a test from multiple machines at the same time.

This is a configurable feature. If enabled on a test and the candidate tries to access the test
from another machine while accessing it from another machine, he will see following screen -

<img src="/images/ss_stonewall.png" />

He can choose to log out from other active session and continue on this machine. In which case, he will
be logged out from the machine which has the active session.

<img src="/images/ss_logout.png" />

This feature enables the recruiters to proctor the test even more strictly.

*Send email to [support@hackerearth.com](mailto:support@hackerearth.com) for any bugs or suggestions.*

*Posted by [Chandrakant](http://hck.re/ck).*