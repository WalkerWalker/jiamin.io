---
title: From Owning Domain To Hosting Website
layout: page
tags: tech
---

Now I have purchased the domain jiamin.io, how do I make a website such that everyone on earch can visit it through jiamin.io?  I know it is possible but not sure how. 

In most of the tutorial with title "Create your personal webpage in 5 minutes", it starts with buying a domain and along the way hosting service is also purchased. Wordpress can be installed on the hosting service control panel (cpanel) and then we are good to go. It took me 10 minutes to realize that hosting service costs extra money because it gives some storage space on a server. I already have a server on aws so there is no point in paying more. {robably I should install wordpress on my server.

Before messing up my centos server with *yum -y update*, ~~I create a snapshot of the server in case anything goes wrong~~ I found out [Github Page](https://pages.github.com/) is another awesome option. The website will just be hosted on github server and it's free. This soon becomes the obvious choice after I gave it a bit more thought. 

- I don't need to pay for or set up a server and it's free.
- I'm use github regularly. (add, commit, push).
- I like writing articles with markdown. 
- I can fork an existing blog repo, change the content and still be completely ignorant of web development.

I'm particularly proud, insteand of shamed, of being able to NOT know how the web development works (hthml, css, jekyll etc). Just replace images, delete all the existing posts and add my own. How cool is that. 

The only tricky part is [Using a custom domain with GitHub Pages](https://help.github.com/en/articles/using-a-custom-domain-with-github-pages). Terminologies like *A, ALIAS, ANAME record, apex domain, CNAME* are all new to me. It turns out the help pages from github are clear and easy to follow, as long as you find the [right one](https://help.github.com/en/articles/setting-up-an-apex-domain#configuring-a-records-with-your-dns-provider). Also special thanks to Wei for helping me clean up the mess of my DNS setting and explain the "redirect" flow.

```
https://username.github.io/reponame 
---CNAME--->  https://jiamin.io 
---A RECORD--->   github ip address 
---Github Pages Magic--->  webpage returns to browser
```

Obviously this reveals there are a lot that I don't know. At least now I know what I don't know. What a progress. 


