---
title: "Stop Answering the Same Question Twice: Interval-Aware Caching for Druid at Netflix Scale"
url: "https://netflixtechblog.com/stop-answering-the-same-question-twice-interval-aware-caching-for-druid-at-netflix-scale-22fadc9b840e?source=rss----2615bd06b42e---4"
date: "Mon, 06 Apr 2026 22:15:14 GMT"
author: "Netflix Technology Blog"
feed_url: "https://netflixtechblog.com/feed"
---
By Ben Sykes In a previous post , we described how Netflix uses Apache Druid to ingest millions of events per second and query trillions of rows, providing the real-time insights needed to ensure a high-quality experience for our members. Since that post, our scale has grown considerably. With our database holding over 10 trillion rows and regularly ingesting up to 15 million events per second, the value of our real-time data is undeniable.
