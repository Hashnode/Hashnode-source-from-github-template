# Hashnode-source-from-github-template
A template with boilerplate structure for Hashnode's Github as source feature

Please note: A **README.md** at the root is always ignored.

If you don't find a log in your publication dashboard on Hashnode, but have made a commit to your connected repo, then make sure

*   the file ends with .md extension, we support markdown files only.
*   you have connected the same repo as you made a commit to.
*   you added the correct blog domain in your markdown file.
*   Frontmatter: Make sure each article has these details at the top of the file.
    
```
---
title: YOUR_TITLE_HERE **(Required)**
subtitle: YOUR_SUBTITLE_HERE
/* The pathname of your article url 
 * Ex. In https://engineering.hashnode.com/how-we-autodetect-spam-using-googles-vertex-ai 
   "how-we-autodetect-spam-using-googles-vertex-ai" is the slug */ 
slug: CUSTOM_ARTICLE_SLUG_HERE (Will be created automatically if not provided)
tags: TAG_SLUG_1, TAG_SLUG_2 **(Required)** - You can find the list of tags here https://github.com/Hashnode/support/blob/main/misc/tags.json
/* You need to upload your image to https://hashnode.com/uploader 
and use the uploaded image URL as COVER_IMAGE_URL */ 
cover: COVER_IMAGE_URL
domain: YOUR_HASHNODE_BLOG_DOMAIN_NAME_HERE (e.g. sandeep.dev or sandeep.hashnode.dev) **(Required)** 
/* When you have a team publication and a publication member has created an article */ 
/* Please note that this param is only supported while creating an article and not updating */ 
publishAs: USERNAME_OF_AUTHOR_OF_ARTICLE 
/* When your article is republished and you want to use  the origin url as canonical url */ 
canonical: CANONICAL_URL_OF_ARTICLE 
/* Only if you don't want this article to be published yet */ 
ignorePost: Boolean (default: false)
/* If you want to post it only on your blog and hide it from Hashnode community feed */
hideFromHashnodeCommunity: Boolean (default: false)
---

Enter article body here
```        
*   List of tags can be found here https://github.com/Hashnode/support/blob/main/misc/tags.json
*   Make sure you haven't included **ignorePost** in the frontmatter by mistake.
*   Uninstalling app via Github will remove it from all the publications that the repo was connected to. If you want to specifically remove the installation from a particular publication, do it from it's Dashboard (Integrations section).
*   Creating an article with same slug as another article in the publication will overwrite the old article.
*   Do note that maximum of 10 file changes are respected in one particular commit.



