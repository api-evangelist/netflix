# Netflix GraphQL Schema

## Overview

Netflix does not publish a general-purpose public GraphQL API. This schema is a conceptual representation of the Netflix data model derived from publicly available information, including the Netflix Tech Blog, open-source projects (Conductor, Zuul, Falcor), partner documentation, and the Netflix device/partner certification program. It is intended as a reference for understanding how Netflix structures its internal catalog, user, and streaming data.

## Background

Netflix's engineering organization has published extensive detail about its internal data and service architecture through the Netflix Tech Blog and open-source projects. Netflix pioneered the use of Falcor (a JavaScript library for data fetching using a JSON graph) rather than GraphQL, though the underlying data model it exposes maps cleanly to GraphQL types. Netflix's partner APIs (Open Connect, Partner Help Center) are CDN- and device-integration-focused rather than catalog APIs.

Key public resources:
- Netflix Tech Blog: https://netflixtechblog.com/
- GitHub Organization: https://github.com/Netflix
- Open Connect (CDN): https://openconnect.netflix.com/
- Partner Help Center: https://partnerhelp.netflixstudios.com/

## Data Model

The schema models Netflix's core domains:

### Content Catalog
Types covering the full title hierarchy: `Title`, `Movie`, `TVSeries`, `TVSeason`, `TVEpisode`, `Trailer`, `Clip`, `Preview`, `BehindTheScenes`, and `LocalOriginals`. Each title carries genre, maturity rating, production metadata, and availability windows.

### People and Credits
`Person`, `PersonRole`, `Cast`, `CrewMember`, `ProductionCompany`, `Studio`, and `Distributor` model the creative and business entities attached to content.

### Classification and Discovery
`Genre`, `Category`, `SubCategory`, `TopList`, `Trending`, `Popular`, `NowPlaying`, and `NewRelease` support browse and discovery surfaces.

### Availability and Rights
`Availability`, `Country`, `Language`, `StreamingRights`, and `LicenseWindow` model where and when content can be watched.

### Streaming Technical Details
`StreamInfo`, `VideoQuality`, `AudioQuality`, `Codec`, `AudioTrack`, `Subtitle`, and `Chapter` describe the technical characteristics of playback streams.

### User and Profile
`UserProfile`, `ProfileType`, `WatchHistory`, `WatchEntry`, `QueueItem`, `DownloadRecord`, `RatingRecord`, and `EarlyAccess` model per-profile personalization and activity data.

### Recommendations and Search
`Recommendation`, `TitleRecommendation`, `SimilarTitle`, and `SearchResult` support algorithmic and query-driven discovery.

### Awards, Events, and Live
`Award`, `Event`, `LiveEvent`, and `SportEvent` cover newer content types Netflix has expanded into.

### Ratings and Certification
`Rating`, `Certificate`, and `Maturity` model content rating systems across markets.

## Schema Source

Conceptual — derived from public Netflix engineering documentation, open-source projects, and partner program materials. Not an official Netflix API artifact.

## Types Count

72 named types defined in `netflix-schema.graphql`.
