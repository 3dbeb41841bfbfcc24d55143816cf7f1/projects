#  ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) PROJECT 3 - Requirements

## Overview

You’ve already worked in small groups to accomplish various labs and exercises, but this time **we’re going to challenge you to work on a whole project with a small team.**

Not only will you be asked to **exercise additional creativity** in designing your own project, your instructors will partner you with other classmates to architect, design, and collaboratively build a full-stack web application of your own design.

While your last project taught you how to get started with NodeJS, Express, and MongoDB, in this project you will be building a _full stack_ ___MEAN___ application.

**This is meant to push you both technically and collaboratively.** It’s a lot harder to work in a team than to work by yourself, but that's most likely what you’re going to find yourself doing in your first development job after WDI, and **it's important to learn how to work together.**

Make it work, and make it awesome.

---

## Technical Requirements

Your project must:

* **Use the MEAN Stack** to build a full-stack application
* **Have a JSON RESTful API** - routes should be defined using HTTP GET/PUT/POST/DELETE on a URL that represents the resource being accessed
* **Have an interactive front-end** using AngularJS
* **Use at least 2 related models**, one of which should be a user
* **Provide authentication and authorization** to your web application to restrict access to appropriate users
* **Craft thoughtful user stories together**
* **Have a visually impressive design** to kick your portfolio up a notch and have something to wow future clients & employers
* **Manage Source Code** via Git and GitHub
* Layout and style your front-end with **clean & well-formatted CSS**
* **Be deployed online** so it's publicly accessible

Bonuses:

* Consume a 3rd party API
* Add some dynamic UI capabilities using AngularJS based 3rd-party libraries such as:
  - [Angular UI Bootstrap](https://angular-ui.github.io/bootstrap/) - integrates Angular with Twitter Bootstrap Components
  - [Angular Data Table](http://swimlane.github.io/angular-data-table/)
  - [UI Leaflet](https://github.com/angular-ui/ui-leaflet) - embedded Maps
  - [Angular Charts](http://chinmaymk.github.io/angular-charts/) - Dynamic Charts

> NOTE: Be careful about using non-Angular UI libraries with AngularJS. Due to Angular's bi-directional data binding, non-Angular libraries need to be _wrapped_ with a custom directive to correctly interoperate with Angular's digest cycles.

---

### Necessary Deliverables

* A **working API**, hosted somewhere on the internet
* A **working front-end**, hosted somewhere on the internet
* A **link to your hosted working app** in the URL section of your Github repo
* A **git repository hosted on Github**, with a link to your hosted project, and frequent commits dating back to the very beginning of the project
* **A ``readme.md`` file** with:
    * An embedded screenshot of the app
    * Explanations of the **technologies** used
    * A couple paragraphs about the **general approach you took**
    * **Installation instructions** for any dependencies
    * Link to your **user stories** – who are your users, what do they want, and why?
    * Link to your **wireframes** – sketches of major views / interfaces in your application
    * Link to your **pitch deck** – documentation of your wireframes, user stories, and proposed architecture
    * Descriptions of any **unsolved problems** or **major hurdles** you had to overcome
    * **Future vision** for the project

---

### Suggested Ways to Get Started

* **Don’t get too caught up in too many awesome features** – simple is always better. Build something impressive that does one thing well.
* **Design first.** Planning with user stories & wireframes before writing code means you won't get distracted changing your mind – you'll know what to build, and you can spend your time wisely by just building it.
* **Don’t hesitate to write throwaway code** to solve short term problems.
* **Read the docs for whatever technologies / frameworks / API’s you use**.
* **Write your code DRY** and **build your APIs RESTful**.
* **Be consistent with your code style.** Make sure your team project looks like a unified effort.
* **Commit early, commit often.**
* **Keep user stories small and well-defined**, and remember – user stories focus on what a user needs, not what development tasks need accomplishing.
* **Write code another developer wouldn't have to ask you about**. Do your naming conventions make sense? Would another developer be able to look at your app and understand what everything is?
* **Make it all well-formatted.** Are you indenting, consistently? Can we find the start and end of every div, curly brace, etc?
* **Comment your code.** Will someone understand what is going on in each block or function? Even if it's obvious, explaining the what & why means someone else can pick it up and get it.
* **Write pseudocode before you write actual code.** Thinking through the logic of something helps.

---

## Potential Project Ideas

### Q&A App
Think of how helpful sites like Quora & StackOverflow are. Maybe there's some other niche, or some surprising twist you can add to the question-and-answer game.

### Travel Log
Keep a travel log of places you've been, activities, and ratings/reviews. Share your trip information with others. Perhaps plan a trip based on reviews from other users.

### Social Butterflies
Want to plan a social event and share it with your friends? How about an event calendar that everyone can share. Add events from the shared event calendar to your own personal event calendar.

---

### Resources

* **[HackDesign](https://hackdesign.org/lessons)** _(beginner's reference for thinking like a designer)_
* **[Visual Design Hacking](https://generalassemb.ly/online/videos/visual-design-hacking)** _(a great tips-and-tricks focused video from Front Row)_
* **[Web Design For Non-designers](https://generalassemb.ly/online/videos/web-design-for-non-designers)** _(another great design-related course for all the nerds out there)_

---

### Project Feedback + Evaluation

* __Project Workflow__: Did you complete the user stories, wireframes, task tracking, and/or ERDs, as specified above? Did you use source control as expected for the phase of the program you’re in (detailed above)?

* __Technical Requirements__: Did you deliver a project that met all the technical requirements? Given what the class has covered so far, did you build something that was reasonably complex?

* __Creativity__: Did you added a personal spin or creative element into your project submission? Did you deliver something of value to the end user (not just a login button and an index page)?

* __Code Quality__: Did you follow code style guidance and best practices covered in class, such as spacing, modularity, and semantic naming? Did you comment your code as your instructors as we have in class?

* __Problem Solving__: Are you able to defend why you implemented your solution in a certain way? Can you demonstrated that you thought through alternative implementations? _(Note that this part of your feedback evaluation will take place during your one-on-one code review with your instructors, after you've completed the project.)_

* __Total__: Your instructors will give you a total score on your project between:

    Score | Expectations
    ----- | ------------
    **0** | _Incomplete._
    **1** | _Does not meet expectations._
    **2** | _Meets expectactions, good job!_
    **3** | _Exceeds expectations, you wonderful creature, you!_

 This will serve as a helpful overall gauge of whether you met the project goals, but __the more important scores are the individual ones__ above, which can help you identify where to focus your efforts for the next project!

---

### GIT and GitHub Best Practices for Team Projects

Here are some best practices for using Git and GitHub in a one-week team project.

* **Use One GitHub Repo:**  Choose one person to create the GitHub repo. All teammates will clone from one GitHub repo. At the end of the project, teammates may fork the repo if they want to have ownership over their own fork.
* **Use Feature Branches:**  Each developer should do their work in a feature branch and coordinate with the team when to merge back into the master branch. Try to merge no less than once per day.
* **Pull Before Merging:**  Always do a pull before a merge to make sure that you are merging into the latest version of the branch.
* **Rebase Feature Branches:**  Rebasing is a good way to keep a feature branch up to date with the master. Thus you will rebase to update your feature branches and merge to update the master branch. The flow would look like this:
  - complete work on feature branch, test and commit to feature branch
  - checkout master and pull to get latest changes to master
  - if any changes were pulled into master, then
    - checkout feature branch and rebase (or merge) to include latest changes from master into feature branch
    - test feature branch again (this time with latest changes from master)
    - checkout master
  - now merge feature branch into master
  - push master to GitHub with changes from the feature branch
* **Deploy From Master Branch:**  The master branch should be used for deployments to Heroku.
I
