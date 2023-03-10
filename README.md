# How to host a online Resume on Github

*A simple online resume guide which powered by **Jekyll** and **Github Pages***

![GIF](/asset/gifs/resumegif.gif)

[View Online Resume](https://willproj.github.io/changgeng.github.io/)

----

<div align="center">

**[Purpose](https://github.com/willproj/changgeng.github.io#-Purpose) • 
[Prerequisites](https://github.com/willproj/changgeng.github.io#%EF%B8%8F-prerequisites) • 
[Instructions](https://github.com/willproj/changgeng.github.io#%EF%B8%8F-instructions) •
[Embellishment](https://github.com/willproj/changgeng.github.io#-embellishment) • 
[More resource](https://github.com/willproj/changgeng.github.io#-more-resource) •
[Acknowledgments](https://github.com/willproj/changgeng.github.io#-acknowledgments) • 
[FAQs](https://github.com/willproj/changgeng.github.io#faq)**

</div>


# 🧐 Purpose

This project is a showcase of hosting a resume online by using Jekyll and Github pages. it is more than just an online resume site. This README file provides a simple approach to how to host an online resume in a static site by steps from the preparation of the project to building and deploying the site online. It encourages people to build their online resume to be more attractive during job hunting and also provides a guide on how to use **Jekyll** and **Github pages**.

----

# ⚠️ Prerequisites

To start to use this guide you need to prepare a resume which is written by **markdown**. If you need to know how to use markdown to write a resume here is a nice tutorial about learning markdown in [More Resource](#-more-resource).

Also, a Github account is also necessary since the resume will be hosted by Github pages. You can find steps on how to set up your GitHub account in Instruction step 2.

----

# ✍️ Instructions
## Host your own resume from scratch
**1. Installation**   
* Download [Git](https://git-scm.com/download/win)
* Download [Jekyll](https://jekyllrb.com/docs/) ( simply follow the instructions in jekyll official website)
* Download [visual studio code](https://code.visualstudio.com/download)   

**2. Set up Github account**   

* Sign up an Github account
* Navigate to your Github main page to find a **green new button**
* Create an empty repository
* Name your repository as format: **yourname.github.io**
* Then just click Button **Create repository**   
  
**3. Set up local repository**
* Find a proper folder then install the Jekyll and bundler gems by typing command in terminal:
  
  ```
  gem install jekyll bundler
  ```
* Create a jekyll site at **./yourname.github.io**.
  
  ```
  jekyll new yourname.github.io
  ```
* Drag your **README.md** file and **resume.md** to this repository
* Use visual studio code to edit your content in this repository 

**4. Push your local repository to Github**
* Use terminal in your local repository, by typing command:
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

**5.Add you resume and test your Site**
* Copy your resume content into ```index.markdown``` file.
* Open windows powershell terminal
* Navigate to your local repository
* Type command ```bundle exec jekyll serve```
* Once terminal says ```Server running... press ctrl-c to stop.``` then type url: localhost:4000 in browser.
* The page will be seen if it is correctly been set.
* To stop the server, get into the terminal by pressing ***ctrl-c***.Then type ***Y*** and ***enter*** to stop the running server.
      
**6. Update and maintainace with Github**
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
* Once you have initialized your project on GitHub then you only need to repeat commands in **step 6** to keep
  your local project in sync with your GitHub repository.If each time you would like to see the files that would be changed
  in your GitHub repository, you can simply type the command ```git status .``` to check the changing files after using the command
  ```git add .```
## Host your own resume by using this Demo
**1. Fork this project to your own Github account**
* Click **_Fork_** on the top-right position of the project repository webpage.   

**2. Installation**
* Navigate to your own copy of this project in your Github repositories section
* Open terminal in your local folder that you choose to build project and type ```git clone https://github.com/willproj/changgeng.github.io.git``` to copy the project into local folder.   

**3.Test the site**
* Type ```cd changgeng.github.io``` to step into local repository. Type ```bundle install``` to install all dependencies. Type ```bundle exec jekyll serve``` to start the server of the project. 
* Then you can go to ```localhost:4000/changgeng.github.io/``` to review the online resume.
* You can easily change the resume content by copying your own resume content into ```index.markdown```file in the local repository. Restart the server and it will show the new content that you change. 
  
**4. Update and maintainace with Github**
* You can simply follow the **step 6** from the above topic **Host your own resume from scratch**. 
----


# 🤩 Embellishment
  **1.Change jekyll theme**
  * Navigate to [jekyll theme](https://rubygems.org/search?query=jekyll-theme) web then pick up a theme that you like.
  * Find **_Gemfile_** in your local repository,copy command under **_GEMFILE_** from website to your local ```Gemfile``` file.
    also change the **theme name** in ```_config.yml``` file.
  * Open terminal in your local repository folder.
  * Type command ```gem install``` to install the theme.
  * Find the layout requirement in jekyll theme repository, change the layout in ```index.markdown``` to keep compatible with jekyll theme. You can find the layout format in folder **_layout** of theme repository
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
5. [free jekyll theme templates](https://jekyllthemes.io/free)
----
# 💛 Acknowledgments

1. [Modern Technical Writing, *By Andrew Etter*](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=kinw_myk_ro_title)
2. [Jekyll Docs](https://jekyllrb.com/docs/)
3. [GitHub's Jekyll Docs](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)
4. [jekyll theme hacker](https://github.com/pages-themes/hacker)
5. Group members: Robert Loader, Michael Akpan, Kehinde Elukanle 
----

# ❓FAQ

1. Why is my resume not showing up.
   * GitHub may take a few minutes to set up the page. Try to wait for some minutes.
   * Navigate into your project repository on GitHub. You will see **Action** task bar below the name of your project. Click it you will see the running deployment and history deployment records.
   * Try to test localhost by your local repository. Make sure it runs well by localhost.
   * When updating the GitHub repository by pushing the local repository. Make sure to use the right command which pushes content to **gh-pages** branch instead of **main** branch. Make sure you use ```git push origin gh-pages``` instead of ```git push origin main``` 
    
2. Why use command lines to keep local repository in sync with Github?
   * Github does have a drag-drop feature to maintain the project while using git commands will be easier to keep it in sync.
   * Using git commands can make sure each file in the local repository is in sync with Github. While use drag-drop feature may cause a miss of files.
  
3. Why is Markdown better than a word processor?
   * It provides an easy way to format work without finding specific formats like in word doc.
   * The formats used by markdown are clearly shown which can let people know which format is used.
   * Markdown files can be easy to be converted to other formats such as HTML etc.


