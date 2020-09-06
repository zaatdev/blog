---
title: Guideline for adding an article to Zaat.dev blog
date: 2020-09-03T18:00:03.284Z
description: Let me take over the steps that you need to know, in order to publish your article to zaat.dev/blog
author: Zaatbot
author_title: Keeping things run smoothly
author_company: Zaat.dev
author_twitter: zaatbot
author_github: zaatbot
image: ./picture_add_blog.png
tags: meta, markdown, gatsbyJS, writing, tutorial
issue_number: 6
---



## Publish your blog, at Zaat.dev. 


So you decided you wanan write an article in Zaat's blog, great we are happy to hear that, sharing information and knowledage is one of our core values at Zaat. 

First thing first make sure your that the content of your article is align with Zaat's valus. 

### Conditions 

**Orginal, Non-duplicate content only**.
  
By publishing to zaat blog you agree that the content of the article wasn't and will not be published else somewhere else. Aslo that you are the orginal "Owner" author the cotnent. 
We undersatnd that preventing writer to publish their content to other platform say like [meduim](https://medium.com/) or [dev.to](https://dev.to/), sounds like a confilct with our values of spreading knowldge, however we added this restriction inorder to prevent SEO from lowering the zaat.dev ranking because of _duplicarted contents_. Once zaat.dev would be establied and such factor wouldn't matter, we wouldn't think twice before removing this restriction.  


**No Harming Content or bad faith** 

This is not the place for sharing info about how to hack into someone computer, or how use a premuim software freely. make sure to go over our [about](https://zaat.dev/about/) and [privacy](https://zaat.dev/privacy/) pages.  


### Guidline

In order to add your blog content to zaa't blog, you would need to have a github account since the content of the zaat blog is parsed from this [github repo](https://github.com/zaatdev/blog). 

1. clone the repo, cd to it. e.g. `git clone <repo-url> && cd blog`
2. create a new branch e.g. `git -b <artilcle-title>`
3. create folder in `/content` e.g. ` mkdir article-title-example && cd article-title-example`
4.Create an md file where all the coentent will be parsed from,  `touch index.md`. 
5. Start writing! you use your favourite editor to write, we also support emoji :tada:.   
6. Done writing ?, alright add these frontmatter info **At top the md file, before evrtying else**. 
```
--- //must starts with three dashes "---"
title: <Yur blog title is here> // blog title that will be used for HTML title tag 
date: <time-in-iso> //e.g.2020-09-03T18:00:03.284Z 
description: a short description about the article // can be one or two sentence, 
author: <your-name> // Can be first name and last name
author_title: <your-job-title> // what do you people to call you
author_company: <your-compnay-name-or> // if its not relevant for you, you can just say "freelancer" or whatever make sense to you
author_twitter: <your-twitter-handle/> 
author_github: <your-github-handle/>
image: ./<image.file_name.fileextension> // (The file should be same root as the md file, e.g. blog/content/artivle-title`For SEO)
tags: tag1, tag2, tag3, tagn // sepearted by coma, (don't add a trailing coma)
issue_number: <issue number> // open an issue at (https://github.com/zaatdev/blog/issues) then just insert issue number *This for commments functionility* >
--- //must ends with three dashes "---"
```
**Note** There sohuld be **:** after each property name and there should be **one space** between the **:** and the property **value**


Still confused, take a look at this the frontmatter of **this** blog post: 

```
---
title: Guideline for adding an article to Zaat.dev blog
date: 2020-09-03T18:00:03.284Z
description: Let me take over the steps that you need to know, in order to publish your article to zaat.dev/blog
author: Zaatbot
author_title: Keeping things run smoothly
author_company: Zaat.dev
author_twitter: zaatbot
author_github: zaatbot
image: ./picture_add_blog.png
tags: meta, markdown, gatsbyJS, writing, tutorial
issue_number: 6
---
```
Also take a look at the files at [content/adding-artile](https://github.com/zaatdev/blog/tree/main/content/adding-article). 

7. Frontmatter ready?, add, commit changes, open a PR.
8. We review the content, if its aligns with our conditions/values, we merged. 
9. Merged!, say no more, I will get a request from github actions, then I will rebuild site. 
10. your artilce is ready, url is  "zaat.dev/blog/artilce-title-example" // same as folder name from step 3

11. Okay thats it, Happy Writing!. 
