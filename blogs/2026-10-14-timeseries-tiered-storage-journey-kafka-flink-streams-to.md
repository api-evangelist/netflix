---
title: "TimeSeries Tiered Storage Journey: Kafka/Flink Streams to Native Cassandra Cold Reads"
url: "https://netflixtechblog.com/timeseries-tiered-storage-journey-kafka-flink-streams-to-native-cassandra-cold-reads-e59d597c9d60?source=rss----2615bd06b42e---4"
date: "2026-10-14"
author: "Netflix Technology Blog"
feed_url: "https://netflixtechblog.com/feed"
---
By Oleksii Tkachuk , Rajiv Shringi , Chris Lohfink , Abe Ratnofsky , Kartik Sathyanarayanan Introduction In an earlier post , we introduced the TimeSeries Abstraction, our high-throughput, low-latency platform designed to store and query temporal event data at scale. It has since become the operational backbone for Netflix’s largest datasets, which now span multiple petabytes. However, managing such large datasets in hot storage, tuned for low-millisecond latency access , is not cheap.
