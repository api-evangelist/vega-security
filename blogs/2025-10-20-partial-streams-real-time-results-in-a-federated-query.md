---
title: "Partial Streams: Real-Time Results in a Federated Query Engine"
url: "/posts/partial_stream/"
date: "2025-10-20"
feed_url: "https://blog.vega.io/index.xml"
---
We all know the feeling of running a query, staring at some spinner for minutes (or more), waiting, and waiting… For a lot of types of queries, waiting is actually unnecessary. A query engine holds the in-progress state somewhere (memory / disk), as it calculates the query results. Specifically in Vega’s use case of security analytics / threat hunting, users don’t need the exact results every time, they want to see a sample or to get a feel for their data, and iterate quickly with a short feedback loop.
