---
layout: post
title: "Improvement: Data Compression Support in Code API v3"
description: "HackerEarth Code API v3 now serves compressed API responses."
category:
tags: ["Code API", "HackerEarth Code API" ]
---
{% include JB/setup %}


[HackerEarth Code API
v2](https://www.hackerearth.com/docs/api/developers/code/legacy/) doesn't supports compression of the API responses.
Due to this, in the cases where the output of the code requested by a client
turns out to be huge(>100KBs), the request/response cycle will be too time
consuming. This also adds to the cost associated with network transfer out
of the code checker machines.
     HackerEarth Code API v3 now uses gzip compression and returns all the API
responses as gzip compressed content by default.

*Send email to support@hackerearth.com for any bugs or suggestions.*
*Contact [me](mailto:praveen@hackerearth.com) if you are interested in using HackerEarth API.*

*Posted by [Praveen Kumar](https://hackerearth.com/users/praveen97uma).*
