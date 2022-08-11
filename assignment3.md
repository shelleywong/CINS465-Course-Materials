# Assignment #3: Django Templates and Static Files

Simple assignment to help you start working with [Django templates](https://docs.djangoproject.com/en/4.0/topics/templates/) and [static files](https://docs.djangoproject.com/en/4.0/howto/static-files/).

## Assignment Expectations

Note: you may find the Django documentation for [Templates](https://docs.djangoproject.com/en/4.1/topics/templates/) and [How to manage static files](https://docs.djangoproject.com/en/4.1/howto/static-files/) useful for completing this assignment.<br>

* Your website needs to display "CINS465 Hello World" via **Django Template Variable**.
    * Note that this is different than the instructions for assignment 2 -- you **must** use a template variable. If the message is statically defined in an HTML template, you will not get credit.
    * A template variable outputs a value from context; thus, you should also have a view that contains `context` (a dictionary-like object for mapping keys to values)
    * To complete this step, make sure you have a `templates/` folder in your app directory and have included the name of your app in the INSTALLED_APPS in the settings file
* You need to include an example of using a **Django Template Tag** to perform programming logic (i.e. execute an if statement or a for loop)
* You must use **template inheritance**
  * You should have a base "skeleton" template (name this file base.html) that contains common elements of your site and defines blocks that child templates can override.
  * You should have at least one child template that extends base.html
* You use CSS and/or JavaScript to stylize the page.
    * I recommend using [Foundation 6](https://get.foundation/sites/docs/) or another responsive front-end framework.
* You must host at least two different types of static files (e.g. images, JavaScript, CSS) and use the static files embedded in your HTML template.
* You submit your assignment to GitHub correctly.
* You should be able to run the development server and view the site on your local machine at http://localhost:8000/. For more information on setting up routes in Django, please see [the URL dispatcher documentation](https://docs.djangoproject.com/en/4.0/topics/http/urls/).

## Submitting Assignment 3

You should have your code set up such that, when cloned in your folder, it can be run directly via `python manage.py runserver`. Make sure to include any Python packages/libraries/dependencies in a requirements.txt file in your root directory. You can containerize your code via Docker (this is optional, but recommended). If you choose to do this, you should have a Dockerfile in your root directory and a docker-compose.yml in your root directory from which your project can be built and launched.<br>

Your code should be submitted to your CINS465 repo on a branch named `assignment3` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment3  # create branch and switch to it
git add -A  # add all
git commit -m "Assignment 3 Submission"  # Commit changes to branch
git push --set-upstream origin assignment3  # Push code up to assignment3 branch on remote
```

After you create the `assignment3` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
