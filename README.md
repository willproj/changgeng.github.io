# How to host a online Resume on Github

*A simple online resume guide which powered by **Jekyll** and **Github Pages***

![GIF](/asset/gifs/resumegif.gif)

[View Online Resume](http://localhost:4000/changgeng.github.io/)

----

<div align="center">

**[Purpose](https://github.com/willproj/changgeng.github.io#-Purpose) • 
[Prerequisites](https://github.com/willproj/changgeng.github.io#-Prerequisites) • 
[Instructions](https://github.com/willproj/changgeng.github.io#-Instructions) • 
[Acknowledgments](https://github.com/willproj/changgeng.github.io#-Acknowledgments) • 
[FAQs](https://github.com/willproj/changgeng.github.io#-FAQs)**

</div>

# 🧐 Purpose

This readme file will explain how to host an online resume in a static site. In this guide the online resume site will be powered by **Jekyll** and **Github pages**.  

# ⚠️ Prerequisites

To start to use this guide you need to prepare a resume which is written by **markdown**. If you need to know how to use markdown to write a resume here is a nice tutorial about learning markdown in [More Resource](#-more-resource).

# ✍️ Instructions

**1. Installation**   
* Download [Git](https://git-scm.com/download/win)
* Download [Jekyll](https://jekyllrb.com/docs/)
* Download [visual studio code](https://code.visualstudio.com/download)   

**2. Set up Github account**   

* Sign up an Github account
* Navigating your Github main page to find a **green new button**
* Create an empty repository
* Name your repository as format: **yourname.github.io**
* Then just click Button **Create repository**   
  
**3. Set up local repository**
* Find a proper folder then install the jekyll and bundler gems ```gem install jekyll bundler```
* Create a jekyll site at ./yourname.github.io.```jekyll new yourname.github.io```
* Drag your README file and Resume markdown file to this repository
* Use visual studio code to edit your content in this repository 


**4. Push your local repository to Github**
* use powershell in your local repository, by typing command ```git init```
* Create a github branch to deploy your site ```git checkout -b gh-pages```
* Push your repository to Github ```git remote and add https://github.com/username/yourname.github.io.git``` ```git add .``` ```git commit -m "your own comment"``` ```git push origin gh-pages```  

**5.Test your Site**
* Open windows powershell terminal
* Navigate to your local repository
* Type command ```bundle exec jekyll serve```
* Once terminal says ```Server running... press ctrl-c to stop.``` then type url: localhost:4000 in browser.
* The page will be seen if it is correctly been set.
* To stop the server, get into the terminal by pressing ***ctrl-c***.Then type ***Y*** and ***enter*** to stop the running server.
      
**6. Keep local repository in sync with Github repository**
* Open terminal and navigate into your local repository
* Type command ```git add .``` to add updated files
* Type command ```git commit -m "your own comments"``` to prepare the new push
* Type command ```git push origin gh-pages``` to push your new content into Github repository 


# 📕 More resource
1. Markdown
   * [Markdown tutorial](https://www.markdowntutorial.com/)
2. [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
3. [Set up site with jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
# 💛 Acknowledgments

1. [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
2. [Jekyll Docs](https://jekyllrb.com/docs/)
3. [GitHub's Jekyll Docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)


# ❓FAQ
