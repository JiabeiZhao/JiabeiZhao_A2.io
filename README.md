# Hosting and Formatting a Resume using Markdown, VS Code, GitHub Pages, and Jekyll
---
## Purpose
- The purpose of this README is to provide practical steps on how to host and
 format a resume using Markdown, VS Code, GitHub Pages, and Jekyll.
 It includes instructions, animated gifs, and resources for a comprehensive
  guide.
---
## Prerequisites
##### Before proceeding with the steps, you need to have a resume formatted in Markdown. If you need help with Markdown, check out this [Markdown tutorial](https://www.markdowntutorial.com/lesson/1/).
-  Remember to follow the  principles outlined in ["Modern Technical Writing"](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
 -  clear
 -  concise
 -  user-focused
---
## Instructions
Follow the steps below to host and format your resume using **Markdown, VS Code, GitHub Pages, and Jekyll**.

---

#### To begin with, you should have a resuem.md file and jekyll

-  Install Jekyll: If you haven't already, you'll need to install Jekyll on your local machine.
You can do this by following the instructions on the [Jekyll website](https://jekyllrb.com/docs/installation/). Or you can refer to the following abbreviated steps(for Windows).

---
  - Install **Ruby** version 2.5.0 or higher
  - Download and install a **_Ruby+Devkit_** version from RubyInstaller Downloads. Use default options for installation.
  -Run the **_ridk install_** step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the RubyInstaller Documentation. From the options choose **_MSYS2 and MINGW development tool chain_**.
  - Open a new command prompt window from the start menu, so that changes to the **_PATH_** environment variable becomes effective. Install Jekyll and Bundler using **_gem install jekyll bundler_**
  - Check if Jekyll has been installed properly: **_jekyll -v_**
---
  Once you have installed **jekyll**
-  Create a new Jekyll site: Once you have Jekyll installed, you can create a new Jekyll site
by running the command jekyll new  *templete_site*  in your terminal. Replace *template_site* with the name of your site.
-  Add your HTML file: Move your HTML file to the root directory of your new Jekyll site.
-  Edit the _config.yml file: Open the **_config.yml** file in the root directory
of your Jekyll site and add the following line to the end of the file: include: ["*.html"]
-  Generate the site: Run the command jekyll build in your terminal to generate the site.
This will create a **_site** directory in your Jekyll site's root directory.
-  Serve the site: To view your site locally, run the command jekyll serve in your terminal.
This will start a local server and allow you to view your site by going to http://localhost:4000 in your web browser.
-  Upload to a hosting service: Once you're satisfied with your site, you can upload the
contents of the **_site** directory to a hosting service of your choice to make it available
online.

---
#### The next step is uplode our local site to [Github](https://github.com/).
- Create a new repository on GitHub for your resume.
 -  Clone the repository to your local machine.
 -  Create a new file in the repository called index.md.
 -  Open index.md in VS Code and format your resume using Markdown.
 -  Commit your changes and push them to the remote repository.
 -  Set up GitHub Pages or Codeberg Pages for your repository by going to your repository's Settings, scrolling down to the GitHub Pages or Codeberg Pages section, and selecting the source for your pages. Make sure to select the main branch and the root directory.
 -  Wait for a few minutes until your site is ready. You can access it using the link provided in the GitHub Pages or Codeberg Pages section of your repository's Settings.
Here's a visual demonstration of the above steps:

   ![Host and Format a Resume using Markdown, VS Code, GitHub Pages, and Jekyll](https://raw.githubusercontent.com/Satyam1203/resume-github/master/working.gif)

# Resources
- [ Markdown Tutorial ](https://www.markdowntutorial.com/)
- [ Modern Technical Writing by Andrew Etter ](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
- [ Jekyll Documentation ](https://jekyllrb.com/docs/)
- [ Building Websites With Jekyll and GitHub ](https://carpentries-incubator.github.io/jekyll-pages-novice/aio/index.html
)
---
## Authors and Acknowledgments
- This README template was created by and modified by Jiabei Zhao.
---
# FAQs

## Why is Markdown better than a word processor?
Markdown is better than a word processor because it is a lightweight markup language that is easy to learn, write, and read. It allows you to focus on the content of your document rather than the formatting, which makes it easier to create and edit documents quickly and efficiently.

## Why is my resume not showing up?
If your resume is not showing up, make sure that you have followed the instructions correctly and that your repository's GitHub Pages or Codeberg Pages settings are configured properly. Also, give it some time to build and deploy your site. If the issue persists, check your Markdown formatting and the file name of your resume **(index.md)**.

## Why my local site is not as same as the page made by Github?
Take a look inside you **Gemfile** file, the github might not use same format with your local site which automatically generated by **jekyll build**.
