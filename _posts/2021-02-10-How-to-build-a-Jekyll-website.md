---
layout: page
sidebar: right
title: "How to for dummies: creating a static website with Jekyll and GitHub Pages"
teaser: "Want to know how to get started with a website just like this one? Follow the steps described here!"
meta_description: "Guide to build a Jekyll website with GitHub Pages for total beginners."
breadcrumb: true
tags:
  - html
  - website
  - git
  - jekyll
  - github
  - guide
comments: false
show_meta: true
header: no
---


Prerequisites:

- A bit of knowledge on git
- A bit of knowledge on [Markdown](https://www.markdownguide.org/getting-started/) (HTML is useful but not necessary)
- Time

There are different ways to create a static website with Jekyll, probably a lot that I don’t know about! Here are the steps I followed myself, a bit more fine-grained than on the Jekyll website itself. I hope they’re useful! If not, then I’ve made some documentation for my future self 😊 

## Step 1: Install Ruby, RubyGems and Jekyll

Note: if you are using Windows (like me ☹), consider downloading the Ubuntu app from the Windows store (i.e., using the Linux Subsystem for Windows). Then follow the steps from [this instruction video](https://www.youtube.com/watch?v=LfP7Y9Ja6Qc&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=3). 

 

Use a command prompt or the Ubuntu app for the commands listed.



We need to install:

1. Ruby, a programming language that can run Jekyll
   1. Check your version: `ruby -v` (preferably version 2.1 or higher)
   2. Download it for Windows [here](https://rubyinstaller.org/downloads/) (Mac already has it installed)

2. RubyGems: a package manager for Ruby that can install, update and maintain Ruby programs. We later use it to install Jekyll
   1. Check your version: `gem -v`

3. Jekyll through using RubyGems: `gem install Jekyll bundler`
   1. Check your version: `jekyll -v`

 

## Step 2: Create a Jekyll site in a git repository

If you haven’t already, install [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and make a [GitHub account](https://github.com/join)

 

Now, you can go two ways: either A) create a Jekyll website from scratch, without any prespecified formatting *or* B) copy a repository using a specific theme and personalize it.

### A) Create a Jekyll website from scratch

1. Move to the local folder where you want to store your local site files: `cd /my/folder/`
   1. **Note**: if using Ubuntu on Windows, it took me some time to figure out how to move through folders. My C drive was for example reachable through `cd /mnt/c/Users/dorie/`
   2. **Note 2**: Use the `TAB` key to autofill commands!

2. Create a new Jekyll site: `jekyll new [nameofsite]`
   1. Note: aptly name the project!
   2. If you want to use GitHub Pages to host your website, the easiest way is to create a project named `githubusername.github.io`

3. Version control the Jekyll folder by typing: `git init`. The folder is now a git repository: all contents are now tracked by git (except what is listed in the .gitignore file)

4. You can now either create completely new layouts, or install a Jekyll theme. They are available via multiple websites, read all about themes [here](https://jekyllrb.com/docs/themes/). For example, for the theme minimal mistakes, see the installation steps [here](https://github.com/mmistakes/minimal-mistakes#installation) and a preview [here](https://mmistakes.github.io/minimal-mistakes/)

5. Edit your files, see Step 3

6. `add` (stage) and `commit` your changes ([basic instructions here](https://rubygarage.org/blog/most-basic-git-commands-with-examples)) 

7. Finally, `push` your changes to GitHub ([instructions](https://docs.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line))



### B) Copy a repository of an existing theme to your GitHub account

2. Choose a theme for your Jekyll website. They are available via multiple websites, read all about themes [here](https://jekyllrb.com/docs/themes/).

3. Once you have chosen a theme, `fork` (i.e., copy) the repository belonging to that theme to your personal GitHub account. 

4. In the repository settings, change the repository name to `githubusername.github.io`

5. Now in order to work on your website on your local PC, `clone` the repository to your PC

   1. Move to the folder location where you want to clone your repository to: `cd /my/folder`
      1. **Note**: if you use Ubuntu on Windows, it took me some time to figure out how to move through folders. My C drive was for example reachable through ` cd /mnt/c/Users/dorie/`
      2. **Note 2**: Use the `TAB` key to autofill commands!

   2. Clone the repository to that location: `git clone https://github.com/username/username.github.io.git`



## Step 3: Customizing your website

It will probably take some time to get used to the way a Jekyll website is built, especially if you want to change more structural parts of it. In the latter case, some html knowledge would be useful, but I can assure you that Google is your best friend in this case (as it was for me)!

 

Standard folders in a Jekyll website can be found [here](https://jekyllrb.com/docs/structure/). Here’s some introductory tips how to personalize your website. 



### General steps during customization

1. Make sure to move into the folder of the repository: `cd githubusername.github.io`

2. Make sure you are working on the correct branch: `git checkout [branchname]` (e.g., `master`)

3. To see your changes locally, run `bundle exec jekyll serve` and open the URL that Jekyll provides in a browser, probably something like `http://127.0.0.1:4000/`

4. If you are happy with your change, stage the change: `git add [filename]` or `git all -A .` (if you want to stage ALL changes made)

5. Commit your staged files: `git commit -m "Edit x"`

6. Push your changes to your fork (online repository): `git push origin [branch name]`

 

### Editing pages and blogposts

- Open the markdown (.md) files of the pages you want to edit - these may or may not be located in a `pages` folder (note that the `index.md` files is always the homepage. 

- If you want to create a blog post, create a new .md files in the `_posts` folder. Or if you don’t want to publish your post yet, in the `_drafts` folder. 

- Use Atom, Typora or any other markdown editor ([cheat sheet](https://www.markdownguide.org/cheat-sheet/)) to edit the pages

- In order for your pages and posts to display correctly, be sure to include correct `front matter` in each page file (more info [here](https://jekyllrb.com/docs/front-matter/))



### Editing the structure of the website

The structure of your website is determined largely by the following files:

-  `_config.yml` contains all your website’s configuration details. You may want to set your `title: “your website’s title”`, `slogan: “your slogan here”`, `description: “site description here` and other details

- The `_data` folder may include a `navigation.yml` file (or something similar) that defines the navigation menu on your website. It may also contain other data files that you can personalize, depending on the theme you are using. And of course you can create new ones to be used in pages through `site.data.*nameOfDatafile*`

- If you keep including the same component on several pages, you can create `includes`. These are files that can be included on multiple pages without having to edit that component multiple times. Includes are therefore a way to make your website more modular, flexible and efficient as they prevent creating enormous page files. 

**Note on `.yml` files**: `.yml` files are terribly precise and give an error if you type even an extra space. Use a yaml validator (like [this one](http://www.yamllint.com/) to check where your .yml error is!



### Editing the looks of your website

- The `_layouts` folder contains html files with layouts in which content is wrapped. If you change anything in these layouts, all pages using that layout are changed accordingly

- Layouts can also include files from the `_includes` folder, e.g., a `sidebar.html` or `footer.html`. Again, this increases the modularity and efficiency of your website, since all those components are specified separately

- If you want to change colors, fonts, etc., you should go to the `_sass` folder. This usually contains some `.scss` files (a more modern version of the `.css` file) which specify all this. 



## Step 4: Publishing your website

- If you are happy with your website, `push` all changes to the branch of your GitHub repository that you want to publish

- Go to the settings of your GitHub repository

- Scroll down to “GitHub Pages”

- Select the branch that you want published on GitHub Pages

- If you want, use a custom domain for your website (instead of `username.github.io`)

- Wait a few minutes and tadaa! Your website is published. 



**Good luck and have fun! Any questions are welcome.**