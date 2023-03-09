# How to host a online Resume on Github

*A simple online resume guide which powered by **Jekyll** and **Github Pages***

![GIF](/asset/gifs/resumegif.gif)

[View Online Resume](http://localhost:4000/changgeng.github.io/)

----

<div align="center">

**[Purpose](https://github.com/willproj/changgeng.github.io#-Purpose) • 
[Prerequisites](https://github.com/willproj/changgeng.github.io#%EF%B8%8F-prerequisites) • 
[Instructions](https://github.com/willproj/changgeng.github.io#%EF%B8%8F-instructions) •
[Embellishment](https://github.com/willproj/changgeng.github.io#%EF%B8%8F-instructions) • 
[More resource](https://github.com/willproj/changgeng.github.io#-more-resource) •
[Acknowledgments](https://github.com/willproj/changgeng.github.io#-acknowledgments) • 
[FAQs](https://github.com/willproj/changgeng.github.io#faq)**

</div>


# 🧐 Purpose

This project is a showcase of host resume online by using jekyll and Github pages. it is more than just an online resume site. In this README file it provide an simple approach of how to host an online resume in a static site by steps from preparation of the project to build and deploy the site online. It encourages people to build there online resume to be more attractive during job hunting and also provides a guide of how to use **Jekyll** and **Github pages**.

----

# ⚠️ Prerequisites

To start to use this guide you need to prepare a resume which is written by **markdown**. If you need to know how to use markdown to write a resume here is a nice tutorial about learning markdown in [More Resource](#-more-resource).

Also a Github account is also necessary since the resume will be hosted by Github pages. You can find steps of how to set up your Github account in Instruction step 2.

----

# ✍️ Instructions

**1. Installation**   
* Download [Git](https://git-scm.com/download/win)
* Download [Jekyll](https://jekyllrb.com/docs/) ( simply follow the instructions in jekyll official website)
* Download [visual studio code](https://code.visualstudio.com/download)   

**2. Set up Github account**   

* Sign up an Github account
* Navigating your Github main page to find a **green new button**
* Create an empty repository
* Name your repository as format: **yourname.github.io**
* Then just click Button **Create repository**   
  
**3. Set up local repository**
* Find a proper folder then install the jekyll and bundler gems by typing command in terminal:
  
  ```
  gem install jekyll bundler
  ```
* Create a jekyll site at **./yourname.github.io**.
  
  ```
  jekyll new yourname.github.io
  ```
* Drag your README file and Resume markdown file to this repository
* Use visual studio code to edit your content in this repository 


**4. Push your local repository to Github**
* use powershell in your local repository, by typing command:
  ```
  git init
  ```
* Create a github branch to deploy your site by tying command:
  ```
  git checkout -b gh-pages
  ```
* Push your repository to Github 

  ```
  git remote and add https://github.com/username/yourname.github.io.git 
  git add .   
  git commit -m "your own comment"   
  git push origin gh-pages
  ```  

**5.Test your Site**
* Open windows powershell terminal
* Navigate to your local repository
* Type command ```bundle exec jekyll serve```
* Once terminal says ```Server running... press ctrl-c to stop.``` then type url: localhost:4000 in browser.
* The page will be seen if it is correctly been set.
* To stop the server, get into the terminal by pressing ***ctrl-c***.Then type ***Y*** and ***enter*** to stop the running server.
      
**6. Keep local repository in sync with Github repository**
* Open terminal and navigate into your local repository
* Type command to add updated files
  ```
  git add .
  ``` 
* Type command to prepare the new push
  ```
  git commit -m "your own comments"
  ```
* Type command to push your new content into Github repository
  ```
  git push origin gh-pages
  ```
* Once your have initialized your project on Github then you only need to repeat commands in **step 6** to keep
  your local project in syc with your Github repository.If each time you woud like to see the files that would be changed
  in your Github respository you can simply type command ```git status .``` to check the changing files after using command
  ```git add .```

----


# 🤩 Embellishment
  **1.Change jekyll theme**
  * Navigate to [jekyll theme](https://rubygems.org/search?query=jekyll-theme) web then pick up a theme that you like.
  * Find **_Gemfile_** in your local repository,copy command under **_GEMFILE_** from website to your local **_Gemfile_**.
    also change the **theme name** in **__config.yml_**.
  * Open terminal in your local repository folder.
  * Type command ```gem install``` to install the theme.
  * Type command ```bundle exec jekyll serve``` to restart the server to see the new theme.
  
  **2.Use jekyll theme template**
  * Navigate to [jekyll theme template web](https://jekyllthemes.io/free) then pick up a theme template that you like.
  * Navigate to template source web to follow the installation instruction to apply to your own project.
  * Here is a [live Demo](https://willproj.github.io/chang.github.io/) by using template.

----

# 📕 More resource
1. Markdown
   * [Markdown tutorial](https://www.markdowntutorial.com/)
2. [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
3. [Set up site with jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
4. [free jekyll themes](https://rubygems.org/search?query=jekyll-theme)
----

# 💛 Acknowledgments

1. [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
2. [Jekyll Docs](https://jekyllrb.com/docs/)
3. [GitHub's Jekyll Docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
4. [jekyll theme hacker](https://github.com/pages-themes/hacker)
----

# ❓FAQ

1. I have deployed site on Github pages but still cannot see it.
   * Github may take few miniutes to set up the page.Try to wait for some minites.
   * Navigate into your project repository on Github. You will see **Action** task bar below the name of your project.Click it you will see the running deployment and history deployment records.
   * Try to test localhost by your local repository. Make sure it runs well by localhost.
   * When update the Github repository by push local repository. Make sure use the right command which push content to **gh-pages** not **main**. Use ```git push origin gh-pages``` not ```git push origin main``` 
    
2. Why use command lines to keep local repository in sync with Github?
   * Github does have drag-drop feature to maintain the project while use git commands will be more easy to keep it in sync.
   * Use git commands can make sure each file in local repository be in sync with Github. While use drag-drop feature may cause miss of some files.


