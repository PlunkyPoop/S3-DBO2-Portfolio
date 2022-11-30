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
<summary>What is the goal of the user? </summary>
</br>
In my case it's an easy way to access different streaming platforms with little information about the show or movie they are watching. It's important for the user to quickly and easily understand the purpose of the app in a single glance. 

</details>
 

 <details>
<summary>What front-end am I going to use in my project? </summary>
</br>
When looking into front-end frameworks / technologies I was hesitating between 3 options:
<ul>
<li>C#</li>
<li>React.js</li>
<li>Angular</li>
</ul>

Because I already worked with C# for most of my previous year and previous school I decided to try something new. Choosing between React and Angular was difficult because a lot of sources online seemed biased towards one or the other, so I decided to look at the <a href="https://survey.stackoverflow.co/2022/#most-loved-dreaded-and-wanted-webframe-want">Stackoverflow survey</a> to help me make a decision. Where I came along this quote: 
> "Angular.js is in its third year as the most dreaded. React.js completes its fifth year as most wanted." 

So I decided to go with React.js as my front-end to get the basic project going but when I have time I'm going look into Angular to experience "the hatred" for myself.
</details>

<details>
<summary>What backend am I going to use in my project? </summary>
</br>
I'm not going to lie, when looking into backend languages I have looked into a few but ended up choosing the same language as my group-project, which is: <b>Springboot</b>. I chose this to make my life a little easier and just to make sure I can use my knowledge in both projects.
</details>



## 2: Software quality
```
Tooling and methodology: 
Carry out, monitor and report on unit integration, regression and system tests, with attention for security and
performance aspects, as well as applying static code analysis and code reviews.
```
<br>
I have installed PVS studio to check my software quality and it succeeded without fails
<img width="321" alt="Schermafbeelding 2022-11-10 094317" src="https://user-images.githubusercontent.com/60787548/203560310-4d54a251-eb56-4a9b-b7ba-3ff5e6ddc0c1.png">
(this needs a little more work)

## 3: Agile method
```
Choose: 
You are aware of the most popular agile methods and their underlying agile principles. 
Your choice of a method is motivated and based on well-defined selection criteria and context analyses.
```

<details> 
 <summary>What are the basic Agile principles?</summary></br>
An Agile method consists of 12 basic principles, which are the following:</br></br>
<ol type="1">
  <li>Satisfying the customer</li>
  <li>Welcome requirement changes</li>
  <li>Deliver working software regularly</li>
  <li>Business and software people need to work together daily</li>
  <li>Build software around motivated people</li>
  <li>Most efficient way to convey information is face-to-face</li>
  <li>Measure progress in working software</li>
  <li>Promote sustainable development (everyone involved should be able to maintain a contant pace)</li>
  <li>Improve agility with attention to the technical and design side</li>
  <li>Simplify "the amount of work not done"</li>
  <li>The best results come from a self-orginazing team</li>
  <li>Regularly reflect with the team on the progress and behavior</li>
</ol>  

<a href="https://www.agilealliance.org/agile101/12-principles-behind-the-agile-manifesto/">The 12 Principles behind the Agile</a></br>
<a href="https://kanbanize.com/agile/project-management/principles">What Are the 12 Principles of Agile Project Management?</a></br>
</details>

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
Lean is created by Toyota, it works with 5 principles:
<ul>
<li>Value - Knowing and understanding what the customer is willing to pay for.</li>
<li>Value stream mapping - mapping the sequence the product goes through in the company.</li>
<li>Flow - Making sure the information runs smoothly without delay.</li>
<li>Pull - Replacing materials that are actually used and eleminating uneunnecessary elements.</li>
<li>Perfection - Striving the eleminate waste and to improve the value for the customer. </li>
</ul>
Lean is very customer focused, all customers wishes are defined as value. Activity that is non-value add(so not really useful for the customer) is defined as waste. And because we don't want more waste in the world we have to reduce that. 

<h3>Kanban</h3>
Kanban is a workflow management method created in Japan, the word 'Kanban' means 'visualboard' or 'sign'. This method is organised on a board and divided into columns showing the flow within the software production. Because Kanban doesn't really use timeframes (like sprints with scrum), there is a posibility that time problems will develop. Kanban is one of the easiest to use outside of an IT related project. 

<h3>Extreme Programming</h3>
XP, or Extreme Programming is created to improve software quality. When working with the XP method you release in short development cycles, this way you improve productivity and introduce more checkpoints to adopt new customer wishes. With XP you don't program features untill they are actually needed, expecting changes in customers requirements along the way. Code reviews are viewed as a beneficial practice and code will be reviewed continuously. 

<h3>Crystal</h3>
From these 5 Agile methods, Crystal can be seen as the most flexible methods. It is mainly used for short-term projects by a team working from the same workspace. With Crystal teams can work the way they think is most effective. By just going with the flow the team can easily adapt to requirement changes. Crystal emphasizes team collaboration and de-emphasizing documentation and reporting, this can lead to confusion in the code and less visibility  into the teams progress.
</br>
</br>
<a href="https://www.xpand-it.com/blog/top-5-agile-methodologies/">Top 5 main Agile methodologies: advantages and disadvantages</a></br>
<a href="https://leanmethods.com/resources/articles/what-is-lean/">What Is Lean?</a></br>
<a href="https://kanbanize.com/kanban-resources/getting-started/what-is-kanban">What Is Kanban?</a></br>
<a href="https://en.wikipedia.org/wiki/Extreme_programming">Extreme programming</a></br>
<a href="https://www.productplan.com/glossary/crystal-agile-framework/">Crystal Agile Framework</a></br>
</details>

<details> 
 <summary>What Agile method will I use and why?</summary></br>
 I first looked at Scrum, the way I see it it would work best in a groupsproject instead of an indivual project. So I have decided to work in the Crystal method cause that seemed like the most flexible option because I'm still figuring out what functionalities my project will consists of and because it's a short-term project. 
</br>
For my group project we use the Scrum method. We set up a Jira board with all the issues (and child issues) and split these into sprints. 
<a href='https://postimg.cc/NyZ4Rs7J' target='_blank'><img src='https://i.postimg.cc/XJYzSXZb/Schermafbeelding-2022-11-23-105130.png' border='0' alt='Schermafbeelding-2022-11-23-105130'/></a>

<img width="667" alt="image" src="https://user-images.githubusercontent.com/60787548/203517227-d3c61986-2928-478d-833d-34a4c2679fd2.png">

![ezgif com-gif-maker](https://user-images.githubusercontent.com/60787548/203518142-789e6e5f-3f66-4446-9597-a34b5af2a66f.gif)


</br>
And we also use a time table to easily calculate how long we think we need to finish a issue:
<img width="1217" alt="image" src="https://user-images.githubusercontent.com/60787548/203518435-c886ea2c-9523-427d-8396-0078b0c331e9.png">
</br>
After we finish a sprint we reflect on it by using <a href="https://metroretro.io/">Metro retro</a></br>

<img width="1215" alt="image" src="https://user-images.githubusercontent.com/60787548/203520259-8b7468e8-3f88-48eb-b158-14dea8c21b04.png">





</details>

## 4: CI-CD
```
Design and implement: 
You design a release process and implement a continuous integration and deployment solution 
(using e.g. Gitlab CI and Docker).
```
<details> 
 <summary>Research question: How does using docker affect my performance</summary>
 </br>
 For my project I want use Docker to run my project on. When looking into alternative options I thought kept thinking if using docker could have a negative of positive impact on the performance. But before I can make a conclusion I need to first understand what Docker even is and why people use it.
</br>
<h3> What is Docker </h3>
<h6>DOT: literature study</h6>
<hr>
<p>Here is a quote from dockers own website:</p>
<blockquote cite="https://docs.docker.com/get-started/overview/">
"Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running it in production."
</blockquote>

Docker claims to be lighter weight than VM's because they don't have to carry the whole OS, so it could run more copies of the application on the same hardware in comparison to a virtual machine. 

Docker uses containers, each container contains a packaged version of the application with all the necessary parts to operate. That way Docker makes your application portable.

Docker was created to work on Linux but has extended support for non-Linux operating systems like Windows and Apple OS.

![image](https://user-images.githubusercontent.com/60787548/203562860-59f3eaf0-53ad-4c7a-a7d8-6bcf2412ee30.png)
Source: [Ameya Shanbhag](https://avs431.medium.com/explain-it-to-me-like-i-am-a-5-year-old-what-are-docker-image-and-containers-b18db4863cb1)



<a href="https://www.techtarget.com/searchitoperations/definition/Docker">How Docker works</a></br>
<a href="https://docs.docker.com/get-started/overview/">Docker overview</a></br>
<a href="https://www.ibm.com/nl-en/cloud/learn/docker">What is Docker?</a></br>

<h3> Why do people use Docker </h3>
<h6>DOT: Community research</h6>
<hr>

<h3> Which Docker alternatives are there <h3>
<h6>DOT: literature research?</h6>
<hr>

<h3> Docker vs alternative option <h3>
<h6>DOT: System test?</h6>
<hr>

<h3>Conclusion<h3>
<hr>

 </details>




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
</br>
<details> 
 <summary>Which cultural differences are there?</summary>
</br>
 

There are a few different cultural differences according to <a href="https://www.hofstede-insights.com/models/national-culture/">the Hofstede's Cultural Dimensions</a></br>
<ul>
 <li>Power Distance</li>
 <li>Uncertainty Avoidance</li>
 <li>Indulgence / Restraint</li>
 <li>Individualism / Collectivism</li>
 <li>Masculinity / Femininity</li>
 <li>Long-Term Orientation</li>
</ul>
</br>

 <h2>Power distance</h2>
 Here is a quote from <a href="https://www.hofstede-insights.com/country-comparison/the-usa/#:~:text=Power%20distance%20is%20defined%20as,much%20as%20by%20the%20leaders">Hofstede Insight</a> </br>
 
 <blockquote cite="https://www.hofstede-insights.com/country-comparison/the-usa/#:~:text=Power%20distance%20is%20defined%20as,much%20as%20by%20the%20leaders.">
"Power distance is defined as the extent to which the less powerful members of institutions and organisations within a country expect and accept that power is distributed unequally. It has to do with the fact that a society’s inequality is endorsed by the followers as much as by the leaders."
</blockquote>
For example, in a high power distance organization you have desicion making is a result of a rigid hierachy, leaders have more power than the general workforce. People in power have special treatment and employeed depend on those in power for their work assignments.
</br>
</br>
When looking at lower power distance organizations we see that the organizational structure is flat and status isn't as important as in high power distance organizations. Employees have more independce and managers have an "open-door" policy where employees can easily acces leadership when necessary.
</br></br>
If we look at the power distance in the Netherlands we have a score of "38", if we compare that too the countries seen as having a high power distance (like Malaysia and China) and a country that has a lower power distance (like Austria) we will see that the Netherlands is just below the middle.
<a href="https://clearlycultural.com/geert-hofstede-cultural-dimensions/power-distance-index/">(Source for countries)</a>
</br></br>
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204772235-4b69d68e-ea4e-4b3b-a33a-3f36c4b7e0c6.png"></br>

<a href="https://www.hofstede-insights.com/country-comparison/austria,china,malaysia,the-netherlands/">Source</a>
</br>
<h2>Uncertainty Avoidance</h2>
<blockquote cite="https://www.sciencedirect.com/topics/computer-science/uncertainty-avoidance#:~:text=Uncertainty%20avoidance%2C%20or%20the%20degree,relatively%20flexible%20to%20extremely%20rigid).">
"Uncertainty avoidance, or the degree to which people in a country prefer structured over unstructured situations and their tolerance for uncertainty, ambiguity, and diversity of approach (from relatively flexible to extremely rigid)."
</blockquote>
<a href="https://www.hofstede-insights.com/country-comparison/the-usa/#:~:text=Power%20distance%20is%20defined%20as,much%20as%20by%20the%20leaders">Hofstede Insight</a></br></br>
</br>
There are a few difference between high uncertainty avoidance and low uncertainity avoidance:
<h3>Social normal</h3>
<table>
 <tr>
    <th>High Uncertainty Avoidance</th>
    <th>Low Uncertainty Avoidance</th>
  </tr>
  <tr>
    <td>Preserve traditional social institutions and practice</td>
    <td>Openness to change, innovation</td>
  </tr>
   <tr>
    <td>Relating to or exhibiting fear or hatred of foreigners or strangers</td>
    <td>Tolerance of diversity</td>
  </tr>
  <tr>
    <td>Express emotions</td>
    <td>Supress emotions</td>
  </tr>
</table>
</br>
<h3>Politics / legal system</h3>
<table>
 <tr>
    <th>High Uncertainty Avoidance</th>
    <th>Low Uncertainty Avoidance</th>
  </tr>
  <tr>
    <td>Weak interest in politics</td>
    <td>High interest in politics</td>
  </tr>
   <tr>
    <td>Citizen protest repressed</td>
    <td>Citizen protest accepted </td>
  </tr>
  <tr>
    <td>More and specific laws and regulations</td>
    <td>Fewer and general laws and regulations</td>
  </tr>
</table>
</br>
<h3>Religion</h3>
<table>
  <tr>
     <th>High Uncertainty Avoidance</th>
    <th>Low Uncertainty Avoidance</th>
  </tr>
 <tr>
    <td>Catholic, Islam, Judaism, Shintoism</td>
    <td>Protestant, Buddhism, Taoism, Hinduism</td>
  </tr>
  <tr>
    <td>Aggressive core believers</td>
    <td>Little persecution for beliefs</td>
  </tr>
   <tr>
    <td>Ritualized / ceremonial</td>
    <td>Avoid ritualization and ceremony </td>
  </tr>
</table>
</br>
<h3>School</h3>
<table>
  <tr>
     <th>High Uncertainty Avoidance</th>
    <th>Low Uncertainty Avoidance</th>
  </tr>
 <tr>
    <td>Teachers have all the answers</td>
    <td>Teachers may say "I don't know"</td>
  </tr>
  <tr>
    <td>Structured learning</td>
    <td>Open-ended learning</td>
  </tr>
</table>
</br>
<h3>Family</h3>
<table>
  <tr>
     <th>High Uncertainty Avoidance</th>
    <th>Low Uncertainty Avoidance</th>
  </tr>
 <tr>
    <td>Tradional gender roles</td>
    <td>Fewer gender roles</td>
  </tr>
  <tr>
    <td>Children taught the world is full of enemies</td>
    <td>Children taught the world is kind</td>
  </tr>
</table>
</br></br>
If we go back to the <a href="https://clearlycultural.com/geert-hofstede-cultural-dimensions/uncertainty-avoidance-index/">index</a> to compare different countries we will see that the Netherlands around the middle. With the highest uncertainty avoidance Greece and the lowest Singapore.</br></br>
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204782060-1b7a9749-1163-486b-ac86-8a7734b3c665.png">
</br>
According to the <a href="https://www.hofstede-insights.com/country-comparison/the-netherlands/">Hofstede Insight</a>:</br>
<blockquote cite="https://www.hofstede-insights.com/country-comparison/the-netherlands/">
"The Netherlands scores 53 on this dimension and thus exhibits a slight preference for avoiding uncertainty. Countries exhibiting high Uncertainty Avoidance maintain rigid codes of belief and behaviour and are intolerant of unorthodox behaviour and ideas. In these cultures there is an emotional need for rules (even if the rules never seem to work) time is money, people have an inner urge to be busy and work hard, precision and punctuality are the norm, innovation may be resisted, security is an important element in individual motivation."
</blockquote></br>

<h2>Indulgence / Restraint</h2>
<blockquote cite="https://www.jmu.edu/global/isss/resources/global-campus-toolkit/files/hofstede-indulgence.pdf">
"An indulgent society is one
which values the satisfaction of human needs and desires; a restrained society sees the value in curbing
ones' desires and withholding pleasures to align more with societal norms. "Indulgent cultures will tend
to focus more on individual happiness and well-being, leisure time is more important, and there is
greater freedom and personal control. This is in contrast with restrained cultures where positive
emotions are less freely expressed and happiness, freedom, and leisure are not given the same
importance"
</blockquote></br>
For example, China is a restrained society, according to Hofstede, the low score in Indulgance shows "cynicism and pessimism".
The Netherlands is pretty high, which means we are more indulgent.
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204786813-d224407f-3267-4836-a817-b4a8fb3b6493.png">
<blockquote cite="https://www.hofstede-insights.com/country-comparison/the-netherlands/">
"People in societies classified by a high score in Indulgence generally exhibit a willingness to realise their impulses and desires with regard to enjoying life and having fun. They possess a positive attitude and have a tendency towards optimism. In addition, they place a higher degree of importance on leisure time, act as they please and spend money as they wish."
</blockquote></br>
<a href="https://www.hofstede-insights.com/country-comparison/the-netherlands/">Hofstede Insight</a>
</br>

<h2> Individualism / Collectivism</h2>

<blockquote cite="https://www.verywellmind.com/what-are-collectivistic-cultures-2794962#:~:text=Collectivism%20stresses%20the%20importance%20of,are%20promoted%20in%20individualistic%20cultures.">
"Collectivism stresses the importance of the community, while individualism is focused on the rights and concerns of each person. Where unity and selflessness or altruism are valued traits in collectivist cultures, independence and personal identity are promoted in individualistic cultures.
Collectivism stresses the importance of the community, while individualism is focused on the rights and concerns of each person. Where unity and selflessness or altruism are valued traits in collectivist cultures, independence and personal identity are promoted in individualistic cultures"
</blockquote></br>
<a href="https://www.verywellmind.com/what-are-collectivistic-cultures-2794962#:~:text=Collectivism%20stresses%20the%20importance%20of,are%20promoted%20in%20individualistic%20cultures.">Source</a>
</br>

For example, workers that live in a collectivism culture strive to sacrifice their own happiness for the greater good of the group, unlike people who live in a individualism culture, they feel like their own well-being and goals carry greater weight. </br>

When it comes to the Netherlands we score pretty high with a "80", which means we like in a pretty individualism culture. This honestly doesn't come as a shock, we tend to do things on our own and on our own terms. </br>
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204789805-b6e5f64c-a257-4cf0-a159-57e498713415.png"></br>
Netherlands is in the top 5 of the world for the most individualism culture, with UK, Australia and the US just above us. </br>
<blockquote cite="https://www.hofstede-insights.com/country-comparison/the-netherlands/)">
"The Netherlands, with the very high score of 80 is an Individualist society. This means there is a high preference for a loosely-knit social framework in which individuals are expected to take care of themselves and their immediate families only. In Individualist societies offence causes guilt and a loss of self-esteem, the employer/employee relationship is a contract based on mutual advantage, hiring and promotion decisions are supposed to be based on merit only, management is the management of individuals."
</blockquote><a href="https://www.hofstede-insights.com/country-comparison/the-netherlands/)">Source</a></br>




</details>

<details> 
 <summary>What cultural ethics are there in programming?</summary>
 </br>
 
 There are a few ethics to keep in mind while programming. Here are the 8 principles:</br>
 <ul>

<li>Public - "Software engineers shall act consistently with the public interest."</li>
<li>Client and employer - "Software engineers shall act in a manner that is in the best interests of their client and employer consistent with the public interest.</li>
<li>Product - "Software engineers shall ensure that their products and related modifications meet the highest professional standards possible."</li>
<li>Judgement - "Software engineers shall maintain integrity and independence in their professional judgment."</li>
<li>Management -  "Software engineering managers and leaders shall subscribe to and promote an ethical approach to the management of software development and maintenance." </li>
<li>Profession - "Software engineers shall advance the integrity and reputation of the profession consistent with the public interest." </li>
<li>Colleagues - "Software engineers shall be fair to and supportive of their colleagues." </li>
<li>Self - "Software engineers shall participate in lifelong learning regarding the practice of their profession and shall promote an ethical approach to the practice of the profession." </li>
</ul>
 
  </br>
  </br>
 <a href="https://ethics.acm.org/code-of-ethics/software-engineering-code/">The Software Engineering Code of Ethics and Professional Practice</a></br>

</br>

</details>

## 6: Requirements and design
```
Multiple types of test techniques: 
You apply user acceptance testing and stakeholder feedback to validate the quality of the requirements. 
You evaluate the quality of the design (e.g., by testing or prototyping)
taking into account the formulated quality properties like security and performance.
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
  <summary>Wireframe</summary>
<img width="674" alt="image" src="https://user-images.githubusercontent.com/60787548/203567444-b498cb14-e493-4e77-9fcb-1f636bd29a1a.png">
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
 <details> 
  <summary>Design user test</summary>
  </br>
To test if the design idea is clear and users understand the purpose of it I created a <a href='https://app.ballparkhq.com/record/dd590819-27fc-4fbe-bca6-5b9b8485ec3f' target='_blank'>survey</a></br>

<img width="841" alt="image" src="https://user-images.githubusercontent.com/60787548/203735589-ebb3f6a0-dd8f-4eee-afa3-57943bdd7161.png">
<img width="735" alt="image" src="https://user-images.githubusercontent.com/60787548/203735643-f5ea58bd-3df4-4281-a0e2-98d411f2e0b1.png">

</details>
 
 
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


<img width="628" alt="image" src="https://user-images.githubusercontent.com/60787548/203740409-69fbedb4-76e1-4e3c-a30f-6e6e70734e83.png">
<img width="869" alt="image" src="https://user-images.githubusercontent.com/60787548/203740089-3c97157e-994f-444d-9731-531b8f6a423c.png">

