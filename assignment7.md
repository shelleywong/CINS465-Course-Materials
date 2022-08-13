# Assignment #7: CINS 465 Final Project

The CINS465 Final Project is your opportunity to create a website that is interesting to you and that is hosted on the cloud. In addition to using the technologies and concepts covered in class, you will practice something all web developers need to do to improve their skills -- learning something new.<br>

Use your project proposal (created for [Assignment #6: Final Project Proposal](assignment6.md)) to keep yourself on track as you work on your final project.

> Note: You may NOT use this project as a submission for an assignment in another class. You also may NOT submit a project from another class as your final project for CINS465. In certain cases, you may be allowed to expand on a project from another class; however, you must make clear which components were completed for which class and get approval from any instructors involved.

## CINS465 Final Project Overview

For the final project, you should have a website that does the following:

* **Uses data in some way**
    * For this requirement, you must create and use at least one [Model](https://docs.djangoproject.com/en/4.1/topics/db/models/)
    * For at least one of your models, you must get new data from the user (i.e. through a type of [form](https://docs.djangoproject.com/en/4.1/topics/forms/) submission). Additional models may get data from an alternative source.
    * You need to present this data to the user.
    * Ideally, if data presented to the user has changed, they should get an updated version without refreshing the page.
    * Reminder: Django supports several databases, but I recommend using SQLite for this class. When you create your initial Django project, SQLite is the default database.
* **Uses templates**
    * You may use [Django's template language](https://docs.djangoproject.com/en/4.1/topics/templates/) or another template system, but you need a way to render content dynamically in the views.
* **Uses WebSockets or WebAssembly** -- meeting this minimum complexity requirement means you've learned something beyond what is covered in class, specifically related to a modern web protocol/standard
    * Implementing a blog, twitter, and/or forum is not enough -- you must do something beyond this type of functionality.
    * Most students meet this requirement by using [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API), usually in the form of a real time chat integrated into their project in some way.
    * [Django Channels](https://channels.readthedocs.io/en/stable/) is a good starting point. You should start by getting Channels installed and following the Channels tutorial for creating a Chat Server (parts 1-3). You will get partial credit for this component if you successfully complete the tutorial. To get full credit for this component, you will need to do something beyond what is covered in the tutorial.
    * Some examples of going beyond the tutorial include finding a way to integrate the chat system into your website (does it look like it is part of your website or something that was just tacked on?), connecting chat messages to a specific user (so it's clear who posted which message), and saving chat history (i.e. creating a model and saving the chat messages, message author, and message date in your database)
    * This requirement could also be met by a more-than-minimal use of [WebAssembly](https://webassembly.org/). WebAssembly is a binary instruction format that provides a way to run code written in multiple languages on the web at near-native speed. If you are interested in this option, the WebAssembly [developer's guide](https://webassembly.org/getting-started/developers-guide/) is a good starting point. I have some experience compiling C/C++ and Rust to WebAssembly; however, you will need to do some research to determine WebAssembly makes sense for your use case.
* Is **interesting** or **useful**.
    * Doesn't have to be a completely original idea, but should be unique in some way.
    * If you use any tutorials (particularly anything that is not an official Django tutorial), you must include a reference (at minimum, include a link). You should also go beyond the tutorial or include changes that make sense for your website. Your final project should not match something I can find on the internet. Please refer to the academic honesty policy in the syllabus or ask me if you have questions about this.
* Is **hosted on the cloud**.
    * I will be providing you $50 of [Google Compute](https://cloud.google.com/compute) Cloud Credit for this purpose.
    * There is no requirement you host on Google's cloud, but I recommend it, as this cloud credit is no cost to you (credit card information not required).

I will only be supporting development with the technologies discussed in class:

* [Django 4+](https://www.djangoproject.com/)
* [Foundation 6](https://get.foundation/sites/docs/)

It is recommended that you complete the final project as an individual assignment. You may work in a group of two, but working in a group is not a requirement. If you choose to work as a pair, I suggest you have specific roles for each member -- for example, one member focusing on JavaScript, stylization, and front-end programming and the other focusing on data, RESTful APIs, and backend programming. The quality of project proposed be it a team or single member proposal is the same; however, the expectation of the quality and complexity of the final project for a team of two is slightly higher.

## Final Project Grading

Your CINS465 Final Project will be graded on the following:

* **Your Proposal**
    * See [Assignment 6](assignment6.md)
* **Lecture and Lab Session Attendance**
    * During class lectures, I will use PollEverywhere to ask questions, get feedback, and track attendance. Partway through the semester, class time will switch from lectures to lab help sessions.
    * To receive full credit for this component, you should plan on attending at least 80% of class lectures and lab help sessions.
    * These lab help sessions will (1) double as a midpoint check-in to confirm that you are making progress on your projects and (2) offer much needed time for you/your group to get any potential development road blocks resolved.
* **Project Progress Updates**
    * You must complete at least 6 Project Progress Update forms
    * The form will ask about what tasks you've completed and any challenges you ran into since the last update, as well as what you plan on working on next.
    * The more detail you include in these forms, the more it will help you for your presentation and the final project feedback form. Note that this web project could be something you want to include on a resume, and it will be beneficial to you if you are able to describe what you accomplished and learned while working on this project.
* **Your Project Presentation**
    * During the last few weeks of the semester and on the day scheduled for the CINS465 final, we will have project presentations.
    * Presentation content may vary depending on the project but should include:
        * An introduction to your project (basic idea of the project)
        * A walk-through of how users could use your website/project,
        * An overview of the goals you had for the project (what you have working at the time of the presentation and what still needs work), and
        * A discussion of any technical problems you have run into along the way.
* **Student Presentation Feedback**
    * For the days that students are presenting their projects, you should plan on attending class in-person (for all presentations!) and filling out feedback forms for the presentations. You must complete at least 75% of the presentation feedback forms in order to receive full credit for this component of the final project.
* **The Final Project Submission**
    * Your project will be graded on the following:
        * If it meets your goals
        * How easy it is for me to use
        * How much I feel you learned along the way (this is partly based on your submission for the Final Project Feedback survey described below) -- make sure to put particular effort into answering the question about what you learned this semester and while working on this project.
        * If it meets the requirements of the project
        * For pair projects, there will be team member feedback, but I will also consider the git commit history for your project submission -- if you aren't contributing, it will show up in the git history.
        * If your final project submission is hosted and submitted on time. I will give information in class about what days I will be grading, so make sure to have your website up and running during this time. If your project is not hosted when I start grading your project, I will give you an opportunity to get your project up and running before I submit final grades.
* **Your Final Project Feedback**
    * You will get access to a Google Survey after the semester ends that you will need to fill out. This will include team member feedback if you worked in a group of two. It will also ask for feedback on the project and the class, things you think should be clarified or improved for future semesters, etc.
    * Pay special attention to the question that asks you about what you learned along the way while completing your project. If your response is too general or does not give much detail, what you learned will not be clear to me.

## Submitting Your Final Project

* Submit your project through a **GitHub repo** (or GitLab, BitBucket, etc) -- either the CSUChico-CINS465 repo created for you OR a personal repo. If you are using a repo that I did not create for you, make sure I can see your project (i.e. if it is private, add me as a collaborator).
* Submit the **Final Project Feedback form** (Google Survey, link in the assignments content area of Blackboard) for your project.
* Submit a link to your Final Project on GitHub (or another source code management service) to `Assignment #7 Final Project Submission Link` in the Assignments content area on Blackboard, so that I have a place to post your final project grade and overall grade for the semester.

**Reminder**: Your final project may be public, but your other CINS465 assignments need to be kept private.

## Grading Caveat

If you have gone above and beyond these requirements or using technology far outside the scope of what I've covered in the semester, but you've come up short on your project goals in the end, you may still receive a good grade in this class. I weigh ambition and self interest in learning new things for this course heavily, even if it means all your goals are not met.
