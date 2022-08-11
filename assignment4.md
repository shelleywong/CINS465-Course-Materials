# Assignment #4: Django Data Driven Page

For this assignment, you will practice working with the Model-View-Controller (MVC) software design pattern (Django models, templates, and views). You will need to get a simple page working with a [Django Model](https://docs.djangoproject.com/en/4.0/topics/db/models/), [Django form](https://docs.djangoproject.com/en/4.0/topics/forms/), and a [template](https://docs.djangoproject.com/en/4.0/ref/templates/language/) built from your model.

## Assignment Expectations

* You have created at least one Django model.
* You have created at least one form.
* The form should accept user input. When the form is submitted, it should send data to a server to create/update a resource (i.e. the form submission should add or change a model instance). The view/HTML template should update based on the model changes.
* You have shown some creativity.
* You submit your assignment to GitHub correctly.
* You should be able to run the development server and view the site on your local machine at http://localhost:8000/. For more information on setting up routes in Django, please see [the URL dispatcher documentation](https://docs.djangoproject.com/en/4.0/topics/http/urls/).

## Submitting Assignment 4

You should have your code set up such that, when cloned in your folder, it can be run directly via `python manage.py runserver`. Make sure to include any Python packages/libraries/dependencies in a requirements.txt file in your root directory. You can containerize your code via Docker (this is optional, but recommended). If you choose to do this, you should have a Dockerfile in your root directory and a docker-compose.yml in your root directory from which your project can be built and launched.<br>

Your code should be submitted to your CINS465 repo on a branch named `assignment4` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment4  # create branch and switch to it
git add -A  # add all
git commit -m "Assignment 4 Submission"  # Commit changes to branch
git push --set-upstream origin assignment4  # Push code up to assignment4 branch on remote
```

After you create the `assignment4` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
