# S3-DBO2-Portfolio

![test](https://media.giphy.com/media/Dh5q0sShxgp13DwrvG/giphy.gif)

## Table of contents
[1: Web application](#1-web-application)</br>
[2: Software quality](#2-software-quality)</br>
[3: Agile method](#3-agile-method)</br>
[4: CI/CD](#4-ci-cd)</br>
[5: Cultural differences and ethics](#5-cultural-differences-and-ethics)</br>
[6: Requirements and design](#6-requirements-and-design)</br>
[7: Business processes](#7-business-processes)</br>
[8: Professional](#8-professional)</br>
 

 
 <!-- Web Application -->
<details>
  <summary>Web Application </summary>
   
Web application
 </details>
 


## 1: Web application
```
User friendly: 
You apply best practices when creating user interfaces and basic user experience testing and development techniques.

Full-stack: 
You design and build a full stack application using a commonly accepted front end Javascript framework and back end
application implementing relevant communication protocols, persistence of data by usage of ORM and addressing asynchronous 
communication issues.
```

<details>
  <summary>What are some practices in creating user interfaces? </summary>
</br>

Before I can even decide how I'm going to implement "the best practices" I need to research and understand which user interface design basics are used when making a front-end.

When researching I learned that's important to know what the goal of the user is before even designing anything. After establishing the goal it's important to keep the design simple, it's important for the user to understand the purpose of the app. Little animations in the buttons the keep the user engaged and give feedback is also important. 

So to sum it up:
+ Know the goal of the user
+ Create an easy-to-navigate interface / simple design 
+ Changes in state and helpful information by animations

There are a lot more practices in creating a good UI design but in my case I will focus on those 3 points 

[Best Practices for Designing an Interface](https://www.usability.gov/what-and-why/user-interface-design.html)</br>
[The 4 Golden Rules of UI Design](https://xd.adobe.com/ideas/process/ui-design/4-golden-rules-ui-design/)</br>
[Design Consistency Guide UI and UX Best Practices](https://www.uxpin.com/studio/blog/guide-design-consistency-best-practices-ui-ux-designers/#h-1-start-with-user-research)
</br>

 </details>
 <details>
<summary>What is the goal of the user? </summary>
</br>
In my case it's an easy way to access different streaming platforms with little information about the show or movie they are watching. It's important for the user to quickly and easily understand the purpose of the app in a single glance. 

</details>
 <details> 
 <summary>Examples of other designs</summary>
</br>
When researching I though it would be smart to first examine how the streaming services show the user where they left of before even searching for designs from other people online. </br></br>

Firsly I looked at Plex:
![image](https://user-images.githubusercontent.com/60787548/195307580-87997667-faa1-4dfb-b0b8-3fc82df30712.png)</br>
Plex uses the poster on the right with the title and a little description on the left. They show the rating and three simple buttons which get a different color when hovering over it to indicate that it will perform an action when clicking on it.</br>

Secondly I looked at Netflix:</br>
![image](https://user-images.githubusercontent.com/60787548/195308852-0e8bf976-9e67-4d30-9b6d-9814f458ca47.png)</br>
As you can see, they have almost the same design as Plex with the image on the right and a title and description on the left. With two simple buttons which change color when hovering over it to indicate it's a button with an action. </br>

To make it easier for user to understand my app I will also base my design on these two designs. </br> </br>
Now let's look at some different designs created by designers online. </br>
![image](https://user-images.githubusercontent.com/60787548/195311419-54d2c048-15e8-471e-9b68-e612d12b7909.png)
If we look at this design created by [CMARIX TechnoLabs](https://www.cmarix.com/) we can also see the title on the left but this design has the image more centered, and again the simple buttons.

![image](https://user-images.githubusercontent.com/60787548/195312662-104bfd17-f3c9-43fc-9c51-a3ffefb70660.png)
Created by: [aPurple](https://www.apurple.co/)

</details>

 <details> 
 <summary>My design</summary>
</br>
Based on the 3 practices and the other streaming service examples I can up with the following design:</br></br>
I have decided to put the image right and the title and description left, for each different streaming service it will show where they left off (if the login and api data is available)</br>
<a href='https://postimg.cc/xXyWymkg' target='_blank'><img src='https://i.postimg.cc/7Zpw4Mqv/Hub-Design-1.png' border='0' alt='Hub-Design-1'/></a>
</br>
I also have an alternative design where the colors of the background are dynamic and change with the colors of the poster</br>
<a href='https://postimg.cc/rz13LWjT' target='_blank'><img src='https://i.postimg.cc/jqmbP4JD/Hub-2.png' border='0' alt='Hub-2'/></a>
</details>





## 2: Software quality
```
Tooling and methodology: 
Carry out, monitor and report on unit integration, regression and system tests, with attention for security and
performance aspects, as well as applying static code analysis and code reviews.
```

## 3: Agile method
```
Choose: 
You are aware of the most popular agile methods and their underlying agile principles. 
Your choice of a method is motivated and based on well-defined selection criteria and context analyses.
```
<details> 
 <summary>Which different Agile methods are there?</summary>
</br>

There are 5 different mainly used Agile methods: 
+ Scrum
+ Lean
+ Kanban
+ XP (Extreme Programming)
+ Crystal

<h3>Scrum</h3>
When using scrum you work in sprints, those are cycles in the development. You start with a startup to discuss what is the plan is for the day. When using scrum it focuses more on quality resulting in less mistakes. When you get a daily assignment it's more motivating when you finish the task for a day. The disadvantage of using scrum is losing track of the whole process of the project and team members not knowing their role in the project. </br>

<h3>Lean</h3>
Lean is created by Toyota, 

[Top 5 main Agile methodologies: advantages and disadvantages](https://www.xpand-it.com/blog/top-5-agile-methodologies/)


</details>
</br>
<details> 
 <summary>What Agile method will I use and why?</summary>
 I first looked at Scrum, the way I see it it would work best in a groupsproject instead of an indivual project. 
</br>

</details>

## 4: CI-CD
```
Design and implement: 
You design a release process and implement a continuous integration and deployment solution 
(using e.g. Gitlab CI and Docker).
```

## 5: Cultural differences and ethics
```
Recognize: 
Recognition is based on theoretically substantiated awareness of cultural differences and ethical 
aspects in software engineering.

Take into account: 
Adapt your communication, working, and behavior styles to reflect project stakeholders 
from different cultures; Address one of the standard Programming Ethical Guidelines 
(e.g., ACM Code of Ethics and Professional Conduct) in your work.  
```
## 6: Requirements and design
```
Multiple types of test techniques: 
You apply user acceptance testing and stakeholder feedback to validate the quality of the requirements. 
You evaluate the quality of the design (e.g., by testing or prototyping)
taking into account the formulated quality properties like security and performance.
```
## 7: Business processes
```
Simple: 
Involving stakeholders, predominantly sequential processes with one or two alternative paths.

Related: 
Business processes during which the software that you are developing will be used (business processes that the software must
support by fully or partially automating them). Or business processes needed for the success of your software development project 
(e.g., product release, market release, financial assurance).
```

## 8: Professional
```
Professional manner: 
You develop software as a team effort according to a prescribed software methodology and following team agreements. 
You are able to track your work progress and communicate your progress with the team.

You actively ask and apply feedback from stakeholders and advise them on the most optimal technical and
design (architectural) solutions. You choose and substantiate solutions for a given problem.
```
