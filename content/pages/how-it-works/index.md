---
title: "How it Works"
slug: how-it-works
cover: ./cover.png
disqus: false
description: "The page explain how this service help freelancers to promote their work."
---

[Admin Dashboards](https://appseed.us/admin-dashboards) is an [open-source project](https://github.com/admin-dashboards/), created to promote the work of freelancers and small agencies in front of **big sharks**, using content submitted by developers.  

## The motivation

If you are a freelancer or a small startup, and you have in your portfolio an admin dashboard product, trying to promote it and sell it, can be challenging without a serious budget. The first page in Google for the keyword “admin dashboards” is full of well-positioned companies like ColorLib, WrapBootstrap, and other companies at the same level.

## The plan 

To get Google's attention, we need to pass this simple checklist:
 - A fast, well-structured website
 - Specific content
 - No bullshit or spam 
 - Good referrals  

## Implementation

 - The domain name **admin-dashboards.com**, match 100% the keyword we are targeting. And it was free. This fact forced me to think 'God is a hacker' 
 
 - **The speed**. I was testing a few static website generators (Hugo, Gridsome, Jekkyl) but the winner was [GatsbyJS](https://www.gatsbyjs.org/). The result: this app scores more than 90 on Lighthouse and is a clone of this [gatsby starter](https://www.gatsbyjs.org/starters/GatsbyCentral/gatsby-v2-starter-lumen/). There is no login, registration, the entire app is plain HTML, that follows best SEO, and usability practices. You may read [here](https://www.gatsbyjs.org/docs/conceptual-guide/) about Gatsby.  

 - **The website structure**:
    - Categories are keywords related to the `admin dashboard` keyword. The winners (selected by the search volumes) are:
    - `react dashboard` - 2.9k mo searches
    - `vue dashboard` - 1k mo searches
    - `angular dashboards` - 2.9k mo searches
    - `flask dashboard` - 0.7k mo searches
    - Products. Each dashboard will be listed in two places: as an item in the mother category, and as a single page, in the root of the website. See the website files structure bellow, for more information

 - **The content**: the information for each product will be curated to provide only relevant information to the audience. 
 
 - **The referrals** The Github repository was created to follow the domain signature. `github.com/admin-dashboards`. Also, the products, with a little bit of traction from the audience, will have a correspondent project on Github, on address `github.com/admin-dashboards/killer-dashboard`. Google loves this kind of s**t, and will rank the project better than others, because the information (keyword, content) is consistent, across multiple domains.    

```
## Site structure

<root>
   |
   |---/react-dashboards #category, with paginated items
   |---/vue-dashboards   #category, with paginated items
   |---/flask-dashboards #category, with paginated items
   |
   |   # bellow are products, listed directly in website root, 
   |   # using a SEO friendly URL
   |   # If we have an admin dashboard named Killer Dashboard, 
   |   # coded by Alien Agency in React, the URL is
   |   #
   |   # react-dashboard-killer-dashboard-by-alien-agency  
   |   #
   |
   /react-dashboard-killer-dashboard-by-alien-agency 
   |
   /flask-dashboard-black-creative-tim 
   |
   /react-dashboard-shards-lite
   |
   /flask-dashboard-black-creative-tim
   |
   | __________________________________
```

<br />

## Links

 - Read the full story on Medium [Admin-Dashboards — goes open source](https://medium.com/@appseed.us/admin-dashboards-com-goes-open-source-2a95862b5eab)
 - Upvote [Admin-Dashboards](https://www.producthunt.com/posts/admin-dashboards) on Product hunt, and help us grow
 - Upvote on [Admin-Dashboards on Reddit](https://www.reddit.com/r/reactjs/comments/c64vw2/react_dashboards_opensource_released_under_the/)
