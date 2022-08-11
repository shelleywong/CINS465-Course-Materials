# Assignment #1: Learning Python 3

For this assignment, you will work through [HackerRank's](https://www.hackerrank.com/) Python Language Proficiency set of challenges. The goal is for you to work through solving a variety of problems, learn Python3 language features, gain some proficiency in programming with Python3, and validate your success.

## Your Task

Your task is to get the 3 star silver Python language proficiency badge on HackerRank. There are a number of decent problems to give you hands on practice with a multitude of Python language features. Gaining some proficiency with Python will be helpful as we move forward -- you will use Python to interact with web technologies in this class, and you may continue to use Python beyond this class in other applications.

## Instructions

1. Create an Account or Login to [HackerRank](https://www.hackerrank.com/) -- make sure your csuchico email is one of the email addresses attached to your account (add another email if you've already created an account with a different email address)
2. From the Dashboard, select Python (Skills Available for Practice)
3. Complete enough challenges to earn a Python Badge. You may choose to work on any Skills or Subdomains, at any Difficulty level. To get the most benefit for this class, make sure you select Python 3 as the language you'll use to complete each challenge (there are several versions of Python available).
4. Submit Proof (see details below)

## Grading

You may earn partial credit if you complete some challenges but do not get to the 3 start silver. You may earn extra credit for additional badges you earn beyond the 3 star silver.

* 1 Star - Bronze (35 points needed) - 30%
* 2 Star - Bronze (70 points needed) - 70%
* 3 Star - Silver (110 points needed) - 100%
* 4 Star - Silver (220 points needed) - 110%
* 5 Star - Gold (400 points needed) - 120%

Hackerrank's [Scoring Documentation](https://www.hackerrank.com/scoring)

## Submitting Proof

If you haven't already [created your CINS465 GitHub repo](https://www.bryancdixon.com/fall/2022/cins/465/repo/), you'll need the GitHub Token given out in lecture to do so.

## Proofs

I'll need three things to be submitted for you to get credit for this assignment -- you will put all three things into your CINS465 repo. If it makes things easier, you can put everything for assignment 1 into an `assigment1` folder:

1. Include a screenshot of your HackerRank account settings with your username and school email in the screenshot (should look like the image below):

![Screenshot of HackerRank Account Settings](/assets/images/hackerrank_accountdetails.png)

2. Include a screenshot of your Hackerrank profile with your username and the badge to confirm you earned the badge. Make sure your username and badge are both captured as in the image below:

![Screenshot of HackerRank Profile and Python Badge](/assets/images/hackerrank_badgeproof.png)

3. Lastly, include a README.md file with the above screenshots and a list of the hackerrank challenges you solved to earn the badge. Use markdown to create a list of the names of the challenges, or as a list of links to the challenges. This is to help provide me with some insight into what challenges you solved. Here is the [GitHub Flavored Markdown guide for basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). In this README.md file, I expect you to use at least one [markdown heading](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings) and one [markdown list](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#lists) (ordered or unordered).

## Putting Proof on GitHub

The three proficiency proofs should be submitted to your CINS465 repo on a **branch** named `assignment1` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment1  #create branch and switch to it
git add -A  #add all -- this should include the 2 screenshots and README.md file listed above
git commit -m "Assignment 1 Submission"  #Commit changes to branch
git push origin assignment1  #Push code up to assignment1 branch on remote
```

> Note: I recommend putting assignments 0 and 1 in directories named assignment0 and assignment1, respectively. Starting with assignment 2, you will begin creating a Django web app. You do not need to create separate folders for assignments 2 through 5 -- these assignments build on each other, and there is no need to start from scratch with a new project/directory for each assignment.

After you create the `assignment1` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
