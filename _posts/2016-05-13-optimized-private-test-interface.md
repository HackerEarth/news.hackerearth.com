---
layout: post
title: "Feature: Private test interface optimized for slow internet"
description: "Private test interface has been optimized for slow internet connections"
category:
tags: [Assessment]
---
{% include JB/setup %}

The Private Test Interface has been optimized for slow internet connections.
Several changes have been made to the interface which resulted in reduced
roundtrip to the server. Now, the initial load may take little longer because
all the resources are being loaded at once, to avoid requests later.

Once the interface is loaded, the candidate can solve the questions smoothly
even if the internet connection is slow.

*Posted by [Chandrakant](http://hck.re/ck).*