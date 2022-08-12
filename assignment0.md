# Assignment 0 Hello Web

The goal of this assignment is to make sure you have set up your CINS465 GitHub repo and give you some experience with basic web (HTML, CSS, and JavaScript).

**Assignment Expectations:**
* You have generated a CINS465 GitHub repo (Part 1)
* You have created a basic website and practiced using HTML and CSS (Part 2)

## Part 1: Generate your CINS465 GitHub repo

To Generate Your CINS465 Repo, see instructions on Blackboard in the **Assignments** content area.<br>

After you have created any remote git repository, I recommend completing all actions through the command line. There are ways to work with git through a graphical user interface (GUI); however, although this may seem easier at first, it can lead to problems and make your life more difficult if you are not careful. Most experienced programmers and recruiters use the command line for git operations and may expect you to do so as well. Once you've learned the commands, it can make your day-to-day workflow smoother and easier!<br>

You may find the following git cheat sheets useful for completing common git operations:
* [GitHub's git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)
* [GitLab's git cheat sheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)<br>

Before completing the next steps, make sure you have set up a way to [authenticate to GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github). My preferred way to connect to GitHub is to [Connect with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh), an option that is both secure and easy to use:
* [Check for existing SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys)
* If you do not have an existing SSH key, follow the steps for [Generating a new SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
  * Note: you may want to create an RSA key (for later in the semester, if you host your website with Google Cloud) -- the [Google Cloud guide for choosing a key algorithm](https://cloud.google.com/certificate-authority-service/docs/choosing-key-algorithm) mentions that its certificate authority does not support Ed25519 algorithms.
  * I use the following command to create a key that is larger (and more secure) than the default: `ssh-keygen -t rsa -b 8192`
  * If you want to see this in action, I recommend watching Dr. Bryan Dixon's [Git Basics Video](https://www.youtube.com/watch?v=0JgyAJMvZlY)
* Then follow the instructions for [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

Once you have generated your repository and confirmed that it contains the expected starter code, you will need to clone the repo. In a terminal, navigate to the directory where you would like to put your repo. For example, I have created a directory called `repos` in my home directory to hold all my git repos:
```
$ cd ~/repos
```

You will want to run the `git clone` command from this directory. On GitHub, find the green 'Code' button and copy the URL -- if you have set up an SSH key, you can use the SSH URL; otherwise, you'll need to use the HTTPS URL. Then go back to your local directory and clone the repo (replace with your project's URL, no brackets):
```
$ git clone [project url]
```

Then move into the directory that you've just created and confirm that it contains the expected starter code files (should look similar to the following):
```
~/repos $ cd CINS465-F22-Shelley-Wong
~/repos/CINS465-F22-Shelley-Wong $ ls -al
total 64
drwxr-xr-x  11 shelleywong  staff   352 Aug 10 09:26 .
drwxr-xr-x  19 shelleywong  staff   608 Aug 10 09:26 ..
-rw-r--r--   1 shelleywong  staff   547 Aug 10 09:26 .coveragerc
drwxr-xr-x  12 shelleywong  staff   384 Aug 10 09:26 .git
-rw-r--r--   1 shelleywong  staff  2802 Aug 10 09:26 .gitignore
-rw-r--r--   1 shelleywong  staff  1384 Aug 10 09:26 .gitlab-ci.yml
-rw-r--r--   1 shelleywong  staff   114 Aug 10 09:26 Dockerfile
-rw-r--r--   1 shelleywong  staff  1073 Aug 10 09:26 LICENSE
-rw-r--r--   1 shelleywong  staff   859 Aug 10 09:26 README.md
-rw-r--r--   1 shelleywong  staff   216 Aug 10 09:26 docker-compose.yml
-rw-r--r--   1 shelleywong  staff     1 Aug 10 09:26 requirements.txt
```
> Note: Files and directories that begin with '.' are hidden -- if you simply use `ls` to see what's in this directory, you will not see the hidden files.

Confirm that you are on the `main` branch:
```
$ git branch
```
> Note: If a git command is not working, make sure that you are working in a directory that contains a .git subdirectory

You should see something like this (type `q` to exit) -- the `*` indicates which branch you are currently on:
```
* main
(END)
```

You can figure out how to work with git in a way that works for you; however, the following commands describe my preferred workflow:
* From the `main` branch, create a new branch and switch your working directory to this branch (for a specific task or assignment, e.g. `assignment0`):
```
(main) $ git checkout -b assignment0
Switched to a new branch 'assignment0'
(assignment0) $
```
* Complete work for this task, e.g. adding and editing files/directories. Then, you can add, commit, and push changes to the current branch -- you may do these steps once or as many times as makes sense for your task (note that these are the steps shown for submitting your CINS465 assignments):
```
(assignment0) $ git add -A  # add all
(assignment0) $ git commit -m "Assignment 0 Submission"  # Commit changes to this branch
(assignment0) $ git push --set-upstream origin assignment0  # Push code up to assignment0 branch on remote
```
  * Note: You only need to include `--set-upstream origin assignment0` once per branch. After doing this once, you can simply use: `git push`
  * Before I add, commit, and push changes, I like to use the `git status` and `git diff` commands to confirm the changes I have made -- these steps are optional, but they help me know what to write in my commit message and be sure that I am only saving changes that I want to be saved.
* When done with this task/assignment, return to the main branch, merge the task branch history into the main branch, and push changes to the main branch.
```
(assignment0) $ git checkout main
(main) $ git merge assignment0
(main) $ git push origin main
```
* When ready to start a new task, repeat the steps listed above with a new branch. The task/assignment branches will act as a snapshot of your code at a given point in time. New branches will contain the code from the previously created branches. It is not necessary that you merge all changes back into the main branch; however, I find that this helps ensure that the history of the repo remains consistent.

## Part 2: Practice HTML, CSS, and JavaScript

To be prepared for this class, you will want to familiarize yourself with HTML5, CSS/CSS3, and Javascript/JS. At one point, this material was effectively its own course (CINS110, a prerequisite to CINS465); however, CINS110 has been removed as a prerequisite, so you are responsible for learning HTML5, CSS, and JS mostly on your own. HTML is the language for building web pages, CSS is the language for styling web pages, and JavaScript is the most widely used client-side scripting language. Most modern websites use libraries or frameworks built on top of these languages, and the focus in this class will be applying these tools in relation to a web framework.

### Create an intro website to practice HTML and CSS

For this assignment, you will need to create a simple website that serves as a brief introduction to you or something that interests you. Be creative, just make sure you include the requirements listed below. For this assignment, focus on HTML and CSS (JavaScript is optional right now -- later in the semester, for Assignment 5, you will be required to use JavaScript) <br>

For this assignment, your website will basically live on your local computer. Put everything related to this website in a directory called `assignment0`. Within this folder, you will have one .html file (at minimum). Optionally, you may have some subdirectories to hold `scripts` (.js files), `styles` (.css files), and/or `images` (e.g. jpeg, png). You will be able to view the html file in the browser. It will probably look like it was made in the 90s.<br>

**To view your website (local html file) in a browser:**<br>
Figure out the path to your assignment0 directory:
```
$ pwd
/Users/shelleywong/repos/CINS465-test-repo-f22/assignment0
```
Copy the entire path and paste it in the browser address bar. Add a backslash and the name of your html file at the end of the path, e.g. `/Users/shelleywong/repos/CINS465-test-repo-f22/assignment0/web-basics.html`<br>

As you make updates to your website, it may help to regularly reload the page in your browser and confirm that your changes are showing up as expected.<br>

**Assignment 0 Website Requirements:**
* Includes basic HTML (use at least one example of each of the following in a way that makes sense for your website)
  * A \<head\> element
  * A \<body\> element
  * A \<div\> element
  * A \<title\> element
  * A heading element
  * A paragraph element
  * An HTML comment
  * metadata
  * A list (ordered or unordered, with at least 3 list items)
  * A link (an anchor with a hypertext reference to a web address)
  * An image (make sure to include alt text)
* Basic CSS (can be inline, internal, or an external stylesheet)
  * CSS comment
  * Set text color (to something other than the default)
  * Set background color (to something other than the default)
  * Update the font (e.g. change the font family or font size to something other than the default)
  * use padding in some way (other than 0)
  * use a margin in some way (other than 0)
  * add style to an HTML element (impacts all elements of this type)
  * add style to a class (impacts all elements with a specific class attribute)
  * add style to an element with a given id

### Reference: Mozilla's MDN web docs

The Mozilla [MDN web docs](https://developer.mozilla.org/en-US/) are a good resource for web developers. To complete this assignment you can follow their beginners guides that walk through the creation of a "Mozilla is cool" website. Your website can look similar, except it should introduce me to you or something you are interested in:

* [HTML basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
* [CSS basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
* [JavaScript basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

### Reference: W3schools Tutorials

[W3Schools](https://www.w3schools.com/) is an excellent educational website for learning basics of web development. Spend as much time as you need reviewing the HTML5, CSS, and JavaScript tutorials. These tutorials are great resources that you can refer back to throughout the semester, or any time you have questions about these subjects.

* [HTML](https://www.w3schools.com/html/)
* [CSS](https://www.w3schools.com/css/)
* [JavaScript](https://www.w3schools.com/js/)

## Submitting Assignment 0

Make sure you have [created your CINS465 GitHub repo](https://www.bryancdixon.com/fall/2022/cins/465/repo/), you'll need the GitHub Token given out in lecture to do so.

Your code should be submitted to your CINS465 repo on a git branch named `assignment0` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment0  # create branch named 'assignment0' and switch to it
git add -A  # add all
git commit -m "Assignment 0 Submission"  # Commit changes to this branch
git push --set-upstream origin assignment0  # Push code up to assignment0 branch on remote
```

After you create the `assignment0` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
