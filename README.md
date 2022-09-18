## Buddysco.com

#### Hugo installation and running the website locally
1. Install hugo using the [Hugo installation guide](https://gohugo.io/getting-started/installing/)
2. Clone this repository
```
git clone git@github.com:BuddyUpEng/buddyupeng.github.io.git
```
3. Open terminal in the repositories directory and run the following to start the website
```
hugo server -D
```

#### How to add a blog 
1. To add a blog you need to create a markdown ( blog-file.md ) file in `content/blog' directory. 
2. For example to create a blog with title "Amazing Blog Title", with a feature image stored in the repository at `static/images/allpost/allPost-7.jpg`, tags as ['productivity', 'study group'] and content as 'amazing content', you need to add a markdown file at `content/blog/amazing-blog.md` with the following content.
```
---
title: "Amazing Blog title"
date: 2020-07-13T12:00:00+06:00
featureImage: images/allpost/allPost-7.jpg
postImage: images/single-blog/feature-image.jpg
tags: ['productivity', 'study group']
categories: blog
---

amazing content
```

#### Hugo Website Creation steps
```
hugo new site buddysco.com
cd buddysco.com
git init
git submodule add git@github.com:StaticMania/portio-hugo.git themes/portio
cp -r themes/portio/exampleSite/* ./
hugo server -t portio
```

### Hugo Github pages deployment
Follow the steps mentioned [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/).
