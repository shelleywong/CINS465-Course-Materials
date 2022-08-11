# Assignment #2: Django Hello World

For this assignment, you will get started with making a simple standalone Django web project. The goals for this assignment are for you to get Django installed and running and to create a simple website that you can view on your local machine.

## Assignment Expectations:

* You are able to create and use a [Python virtual environment](https://docs.python.org/3/tutorial/venv.html) and/or a [Docker container](https://docs.docker.com/)
* You have downloaded and installed [Django](https://www.djangoproject.com/)
    * Use the latest release
* You have created a basic Django project
    * You may find it helpful to start with the Django documentation for [writing your first Django app](https://docs.djangoproject.com/en/4.0/intro/tutorial01/)
* Your website displays the message: "CINS465 Hello World"
* You are able to submit your assignment to GitHub correctly
    * Containerized is optional
    * Must be submitted to the correct branch
* You should be able to run the development server and view the site on your local machine at http://localhost:8000/. For more information on setting up routes in Django, please see [the URL dispatcher documentation](https://docs.djangoproject.com/en/4.0/topics/http/urls/).

## Submitting Assignment 2

If you haven't already [created your CINS465 GitHub repo](https://www.bryancdixon.com/fall/2022/cins/465/repo/), you'll need the GitHub Token given out in lecture to do so.<br>

You should have your code set up such that, when cloned in your folder, it can be run directly via `python manage.py runserver`. Make sure to include any Python packages/libraries/dependencies in a requirements.txt file in your root directory. You can containerize your code via Docker (this is optional, but recommended). If you choose to do this, you should have a Dockerfile in your root directory and a docker-compose.yml in your root directory from which your project can be built and launched.<br>

Your code should be submitted to your CINS465 repo on a branch named `assignment2` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment2  # create branch and switch to it
git add -A  # add all
git commit -m "Assignment 2 Submission"  # Commit changes to branch
git push --set-upstream origin assignment2  # Push code up to assignment2 branch on remote
```

After you create the `assignment2` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
