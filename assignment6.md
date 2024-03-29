# Assignment #6: Final Project Proposal

The CINS465 Final Project is your opportunity to create a website that is interesting to you and that is hosted on the cloud. In addition to using the technologies and concepts covered in class, you will practice something all web developers need to do to improve their skills -- learning something new.<br>

Review the CINS465 Final Project Overview before you complete the Project Proposal.

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
* **Uses WebSockets or WebAssembly** -- meeting this minimum complexity requirement means you've learned something beyond what is covered in class, specifically related to a modern web protocol/standard.
    * Implementing a blog, twitter, and/or forum is not enough -- you must do something beyond this type of functionality.
    * Most students meet this requirement by using [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API), usually in the form of a real time chat integrated into their project in some way.
    * [Django Channels](https://channels.readthedocs.io/en/stable/) is a good starting point. You should start by getting Channels installed and following the Channels tutorial for creating a Chat Server (parts 1-3). You will get partial credit for this requirement if you successfully complete the tutorial. To get full credit for this requirement, you will need to do something beyond what is covered in the tutorial.
    * Some examples of going beyond the tutorial include finding a way to integrate the chat system into your website (does it look like it is part of your website or something that was just tacked on?), connecting chat messages to a specific user (so it's clear who posted which message), and saving chat history (i.e. creating a model and saving the chat messages, message author, and message date in your database).
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

## Project Proposal (Part 1)

* A **description that gives a basic idea for your project**
    * This component of the proposal has some similarities to an elevator pitch -- it should be a short description that explains the concept of your project in a way such that any listener can understand it in a short period of time (explain who it is for, what it does, why it is needed).
    * Additionally, you should include some description of how the project will get done (i.e. are you using Django?) Make sure to specify how you are going to address the minimum complexity component of the final project -- for what component of your website are you using WebSockets or WebAssembly?
    * If you are completing the project as a team, the quality and complexity of the project proposed should be slightly higher than that of an individual project; however, it does not have to be twice as complex, since working successfully as a team provides its own challenges.

## Submitting Project Proposal (Part 1)

> Note: I will **not** grade your final project unless you have submitted a project proposal and gotten it approved.

* Please submit Project Proposal (Part 1) to `Assignment #6 Project Proposal (Part 1) Submission Link` in the Assignments content area on Blackboard.
* The Proposal should be submitted as a single PDF.
* Project Proposal (Part 1) is the first component of Project Proposal (Part 2). I am using separate due dates so that you can get your website idea approved before completing the rest of the proposal.

## Project Proposal (Part 2)

> Note: If you work as a group of two, you will need to break out the tasks for each member. Remember, there is a slightly higher bar and expected level of complexity for a pair project.<br>

**Your proposal needs to have all of the following**:

* A **description that gives a basic idea for your project**
    * You should include an approved version of your description that gives a basic idea for your project (see Project Proposal (Part 1) above) at the beginning of your submission for Project Proposal (Part 2).
* Basic drawings or diagrams of **what pages your website will provide for user(s)**
    * This component of the proposal is similar to a website wireframe, a visual guide that represents the skeletal framework of a website.
    * May be hand drawn or completed with the wireframing tool of your choice.
    * It is ok if this component does not look professional, but I expect you to have given some thought to how people will interact with your site (page layout, interface elements, navigation).
    * You should also make sure to diagram/discuss transitions between pages (how does everything work together?)
* A basic **database design** diagram or description
    * This component should identify the types of data you want to include in your database (entities/models), the class attributes/fields of each model, and any [relationships between the models](https://www.lucidchart.com/pages/database-diagram/database-design/#section_3) (one-to-one, many-to-one, many-to-many).
    * If creating a database design diagram, may be hand drawn or completed with a diagramming tool of your choice.
    * Your data may change as you begin building your website -- that's fine. I just want to see that you have an idea of how data is going to be used in your website.
* A **timeline** for getting aspects of your project set up, working, developed, etc.
    * For individual projects, set milestones that you want to complete by a given time (be realistic about the time you think you will need, but it's ok if you don't follow your timeline exactly)
    * For team projects, you should set milestones for each member to complete along the way.
    * For individuals and teams, make sure to include time to test each component and confirm that everything is working as expected.
    * You must set **at least 6-8 milestones** per developer. This equals out to about 1 milestone per week. Aim to make progress on your final project EVERY week for the last half of the semester. Remember that you will need to regularly submit project progress updates. Do NOT leave everything until the last week or so!
* A description of your **goals for the project**
    * This component of the proposal should be a list of deliverables/goals.
    * You can think of these as components of your web project that you hope to have working by the end of the semester.
    * You should also include **stretch goals** -- goals you have for the project if time allows or that you would possibly like to add after the semester.

## Submitting Your Project Proposal (Part 2)

> Note: I will **not** grade your final project unless you have submitted a project proposal and gotten it approved.

* Please submit your Project Proposal to `Assignment #6 Project Proposal (Part 2) Submission Link` in the Assignments content area on Blackboard.
* The Proposal should be submitted as a single PDF, with all descriptions, details, diagrams/images put into different sections of the document. Include an appropriate header for each section.
* If you cannot get everything into a single PDF for some reason, include all components of your proposal in a single Blackboard submission. Make sure each file included has a relevant name and loads correctly.
* If you submit your proposal early (at least 1 week before it is due), I will review your proposal and give you feedback if you are missing anything -- you will not lose any points if you make the necessary revisions before the due date. (I will attempt to review proposals and provide feedback for anything submitted at least 48 hours before the due date but am not making any promises).
* If there are any issues with your proposal after the due date, you will lose points, but still receive partial credit for the assignment.
* The normal late assignment policy applies to the Project Proposal. If you do not submit your project proposal by the late assignment deadline, you should still submit your project proposal so it can be approved and you can complete your final project.

## Grading

The Final Project Proposal will be graded as a component of your Final Project. Refer to [Assignment #7: CINS 465 Final Project](assignment7.md) for Final Project grading details.
