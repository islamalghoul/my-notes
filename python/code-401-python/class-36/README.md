[MainPage](../../../README.md)
# What is SWR?
SWR stands for stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861. It basically means that it performs data fetching in 3 steps:


Returns cached data first (stale)
Sends the fetch request (revalidate)
Returns the up-to-date data
SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package. It is a layer built on top of Fetch API and therefore provides additional features on top of just data fetching. These features include caching, pagination, auto revalidation and more.


Why use SWR?
1. Built-in Cache + Real-Time Experience
When we use Fetch or Axios for data fetching in React, we usually need to show the user some loading message or spinner while data is being fetched. Using SWR’s strategy, the user sees the cached (stale) data first and requests are automatically being cached. Components will always be constantly updated with the most recent data, ensuring UI will always be fast and reactive.
Instead of having to write your own logic with Fetch or Axios to paginate data or create an infinite loading UI for your app, SWR provides a simple Hook called useSWRInfinite to handle this for you.


4. More Features + Benefits of SWR
There are many more reasons why you should use SWR in your React apps. Some of them are:


Local mutation
Dependent fetching
Smart error retry
Supports fetching from both REST and GraphQL APIs
Typescript and React Native read


2. Auto Revalidation
SWR ensures that the user sees the most up-to-date data. So even with multiple tabs or windows, the data is always fresh and in sync when the window/tab is refocused.