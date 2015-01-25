---
layout: post
title: "Implementation: Reddit ranking algorithm in Notes"
description: "Trending HackerEarth notes now uses reddit ranking
algorithm for sorting."
category:
tags: [Notes, Reddit Ranking]
---
{% include JB/setup %}

Reddit ranking algorithm to sort hot stories is quite robust and works out
of the box. Moreover, Reddit is open sourced and code is free
available.

We picked out the same ranking algorithm and applied it on
[HackerEarth Notes](http://www.hackerearth.com/notes/). The results were
exactly what it intended to do and served our purpose.

Below is the code in Python, which you can use in similar scenarios.
We made a small modification to the hot() function arguments as we don't
support downvote in Notes.

    """
    Reddit ranking algorithm.
    """

    from datetime import datetime, timedelta
    from math import log

    epoch = datetime(1970, 1, 1)

    def epoch_seconds(date):
        """Returns the number of seconds from the epoch to date."""
        td = date - epoch
        return td.days * 86400 + td.seconds + (float(td.microseconds) / 1000000)

    def score(ups, downs=0):
        return ups - downs

    def hot(ups, date, downs=0):
        """The hot formula."""
        s = score(ups, downs)
        order = log(max(abs(s), 1), 10)
        sign = 1 if s > 0 else -1 if s < 0 else 0
        seconds = epoch_seconds(date) - 1134028003
        return round(order + sign * seconds / 45000, 7)

Enjoy reading some of the best technical content at
[HackerEarth Notes](http://www.hackerearth.com/notes/).

*Send email to support@hackerearth.com for any bugs or suggestions.*

*Posted by [Vivek Prakash](http://hck.re/vivekprakash).*
