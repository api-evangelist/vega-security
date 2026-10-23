---
title: "Hidden Complexities of Distributed SQL"
url: "/posts/distributed_search_optimizations/"
date: "2025-05-22"
feed_url: "https://blog.vega.io/index.xml"
---
Introduction Query planners are a cool piece of software that exists in every database or SQL engine out there. You give it a query like: SELECT user_id, COUNT(*) FROM events GROUP BY user_id; And the planner’s job is to figure out the most efficient way to run this query. That involves: Understanding the structure and statistics of the underlying data Applying transformation rules to optimize the query plan Choosing between different join algorithms, aggregation strategies, and execution orders Splitting work across nodes while minimizing data shuffling It all starts with a logical plan (what
