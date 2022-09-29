# Assignment #5: Client Side Programming

For this assignment, you need to use JavaScript to program the behavior of a web page and add some dynamic functionality (something interesting that happens on the front-end, so your website is not all static).

## Assignment Expectations

* Uses JavaScript (JS) in a way that demonstrates the usefulness of JavaScript.
  * For users visiting your website (or me grading your website), make sure it is clear what your JavaScript does and why it's useful. That is, when I load your index/homepage, I shouldn't have to search for the JavaScript -- it should be clear how I can use your website.
  * May use an internal script, but must include at least one external JS script
  * Includes a JavaScript comment
  * Writes to an HTML element
    * e.g. by using querySelector() and textContext or by using getElementById() and innerHTML
  * Declares and uses at least two variables of different types
  * Uses at least one conditional (i.e. if-else statement) or loop (i.e. while or for loop)
  * Creates and uses an Event Handler
    * Create at least one function that will run based on activity in the browser (e.g. when a user clicks an HTML element, pushes a keyboard key, or moves the mouse over an element)
    * Hint: you may want to use addEventListener() or an onclick event
  * Live updates data from your back-end without the user having to refresh the page.
    * One way to complete this component is to create a JSON version of the data from a model and use [vue.js](https://vuejs.org/) and [Axios](https://axios-http.com/docs/intro) to get the data and update our website.
* You have shown some creativity.
* You submit your assignment to GitHub correctly.
* You should be able to run the development server and view the site on your local machine at http://localhost:8000/. For more information on setting up routes in Django, please see [the URL dispatcher documentation](https://docs.djangoproject.com/en/4.0/topics/http/urls/).

# Submitting Assignment 5

You should have your code set up such that, when cloned in your folder, it can be run directly via `python manage.py runserver`. Make sure to include any Python packages/libraries/dependencies in a requirements.txt file in your root directory. You can containerize your code via Docker (this is optional, but recommended). If you choose to do this, you should have a Dockerfile in your root directory and a docker-compose.yml in your root directory from which your project can be built and launched.<br>

Your code should be submitted to your CINS465 repo on a branch named `assignment5` -- make sure your case is **identical** for your branch name, or I may not find/grade your submission. To do this, you can complete the following in your CINS465 repo directory (it assumes you want to add all the code in the directory):

```
git checkout -b assignment5  # create branch and switch to it
git add -A  # add all
git commit -m "Assignment 5 Submission"  # Commit changes to branch
git push --set-upstream origin assignment5  # Push code up to assignment5 branch on remote
```

After you create the `assignment5` branch and add, commit, and push updates to this branch, you may want to merge the changes with the `main` branch and start any future branches from the latest version of your code. This can help ensure that the history of your git repo remains consistent.
