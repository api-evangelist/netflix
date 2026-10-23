---
title: "Behind the Scenes: Evolving Netflix’s Ads Event Pipeline for Live — Part II"
url: "https://netflixtechblog.com/behind-the-scenes-evolving-netflixs-ads-event-pipeline-for-live-part-ii-826ebf9ad9fb?source=rss----2615bd06b42e---4"
date: "2026-10-14"
author: "Netflix Technology Blog"
feed_url: "https://netflixtechblog.com/feed"
---
By Yogesh Nagarur Introduction In Part 1 of this series , we shared how Netflix built the Ads Event pipeline and approached it as a system design problem: replacing fragmented pipelines with a centralized collection, enrichment, and a standard data contract. The result was Ads Event Publisher, the system that collects ad telemetry from client devices, enriches it with the context of the ad that was actually served, and publishes a single, unified stream of ad events to every downstream consumer: frequency capping, metrics, billing, measurement partners, and reporting. Any member viewing or acc
