# Hashnode-source-from-github-template
A template with boilerplate structure for Hashnode's Github as source feature

Please note: A **README.md** at the root is always ignored.

If you don't find a log in your publication dashboard on Hashnode, but have made a commit to your connected repo, then make sure

*   the file ends with .md extension, we support markdown files only.
*   you have connected the same repo as you made a commit to.
*   you added the correct blog domain in your markdown file.
*   Frontmatter: Make sure each post has these details at the top of the file.
    
```
title: YOUR_TITLE_HERE  
subtitle: YOUR_SUBTITLE_HERE  
slug: CUSTOM_SLUG_HERE  
tags: TAG_SLUG_1, TAG_SLUG_2  
cover: COVER_IMAGE_URL  
domain: YOUR_DOMAIN_NAME_HERE (e.g. sandeep.dev or sandeep.hashnode.dev)   
/* When you have a team publication and a publication member has created a post */   
publishAs: USERNAME_OF_AUTHOR_OF_POST   
/* When your post is republished and you want to use   
the origin url as canonical url for this post */   
canonical: CANONICAL_URL_OF_POST   
/* Only if you don't want this post to be published yet */   
ignorePost: true


Enter article body here
```        
    
*   Make sure you haven't included **ignorePost** in the frontmatter by mistake.
*   Uninstalling app via Github will remove it from all the publications that the repo was connected to. If you want to specifically remove the installation from a particular publication, do it from it's Dashboard (Integrations section).
*   Creating a post with same slug as another post in the publication will overwrite the old post.
*   Do note that maximum of 10 file changes are respected in one particular commit.



