---
title: "Smarter Live Streaming at Scale: Rolling Out VBR for All Netflix Live Events"
url: "https://netflixtechblog.com/smarter-live-streaming-at-scale-rolling-out-vbr-for-all-netflix-live-events-c8f833b238cc?source=rss----2615bd06b42e---4"
date: "Thu, 02 Apr 2026 21:46:27 GMT"
author: "Netflix Technology Blog"
feed_url: "https://netflixtechblog.com/feed"
---
By Renata Teixeira, Zhi Li, Reenal Mahajan, and Wei Wei On January 26, 2026, we flipped an important switch for Live at Netflix: all Live events are now encoded using VBR (Variable Bitrate) instead of CBR (Constant Bitrate) . It sounds like a small configuration change, but it required us to revisit some of the foundational assumptions behind how we deliver Live video at global scale. VBR lets us tailor the bitrate to the actual complexity of the scene, instead of sending every second of video at roughly the same bitrate.
