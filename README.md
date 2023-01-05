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

This semester I have two projects I've worked on, my individual project and my group project.
<p>For my individual project I decided to make an app to access different streaming platforms with little information about
the show or movie in the "resume watching". Named Hubflux.
</p>
<p>
<a href="https://github.com/PlunkyPoop/HubFlux-Backend">My backend project</a></br>
<a href="https://github.com/PlunkyPoop/HubFlux-Frontend">
My frontend Project</a></p>


<p>For my group project we made an app called "Ordinner". The idea behind our project is an app that let's you make orders from your phone (think like the MacDonalds order system but on your phone) Or like a "Thuisbezorgd" but for inside the restaurant.</p>

 <details>
<summary>What is the goal of the user? </summary>
<p>In my case it's an easy way to access different streaming platforms with little information about the show or movie they are watching. 
It's important for the user to quickly and easily understand the purpose of the app in a single glance. </p>

<p>For my group project the goal is to make the order process faster and easier by using smartphones.</p>


</details>
 

 <details>
<summary>What front-end am I going to use in my project? </summary></br>
When looking into front-end frameworks / technologies I was hesitating between 3 options:
<ul>
<li>C#</li>
<li>React.js</li>
<li>Angular</li>
</ul>

Because I already worked with C# for most of my previous year and previous school I decided to try something new. Choosing between React and Angular was difficult because a lot of sources online seemed biased towards one or the other, so I decided to look at the <a href="https://survey.stackoverflow.co/2022/#most-loved-dreaded-and-wanted-webframe-want">Stackoverflow survey</a> to help me make a decision. Where I came along this quote: 
> "Angular.js is in its third year as the most dreaded. React.js completes its fifth year as most wanted." 

So I decided to go with React.js as my front-end to get the basic project going but when I have time I'm going look into Angular to experience "the hatred" for myself.
</br> For my group project I also chose React.js because our group would want to try another coding language.
</details>

<details>
<summary>What backend am I going to use in my project? </summary>
</br>
I'm not going to lie, when looking into backend languages I have looked into a few but ended up choosing the same language as my group-project, which is: <b>Springboot</b>. I chose this to make my life a little easier and just to make sure I can use my knowledge in both projects.
</details>

<details>
<summary>User story from start to finish</summary>
<p>For my individual project I wanted to add a functionability to add your stream service credentials to see your personal watch progress.</p>
<p>I started by setting up a user story inside Github (via issues) in both the front-end and the backend</p>
<img width="718" alt="image" src="https://user-images.githubusercontent.com/60787548/209310719-61cb029c-e910-4cb0-b65f-dafa681ad545.png">
<p>And created for both the backend and the front-end a branch</p>
<img width="618" alt="image" src="https://user-images.githubusercontent.com/60787548/209311331-07ece5d4-9a52-4eb6-8cde-899fba743841.png">
<p>I already have a online database (for using Docker) so I added a new table for my project</p>
<img width="751" alt="image" src="https://user-images.githubusercontent.com/60787548/209314326-962e7da0-9427-40e5-a27f-3272fbbf654f.png">
<p>I also added my database in my backend</p>
<img width="653" alt="image" src="https://user-images.githubusercontent.com/60787548/209314728-517c7e0d-2122-4aac-81a2-5b2ee04e3daf.png">
<p> ^ This is a very big security risk (See security research)</p>

<p>For the front-end I created a new page where you will go when pressing the settings button</p>
<img width="365" alt="image" src="https://user-images.githubusercontent.com/60787548/209320740-86746887-cd45-4240-9c94-250ea7dae5d5.png">
 

<p>On that page it loads all the streaming services with image location and the imdb-code</p>
<img width="829" alt="Schermafbeelding 2022-12-28 120213" src="https://user-images.githubusercontent.com/60787548/210219215-d5ffdafd-f6ec-43f4-b06b-8c70eb2095b5.png">
 
 <p>So i created a blob storage on azure that saves all the images</p>
 <img width="1168" alt="image" src="https://user-images.githubusercontent.com/60787548/210219390-39e7c37a-2923-4346-84e6-55cd86c00795.png">

 <p>After that I made sure that after every change inside the carrousel it loads a new movie (set inside the settings menu)</p>
 <p>After removing all the warnings inside the project I pushed both projects and created a new sonarcloud for both</p>
 <img width="926" alt="Schermafbeelding 2023-01-02 111444" src="https://user-images.githubusercontent.com/60787548/210219763-0613b01f-fd68-4b09-a56c-33114222adbb.png">
<img width="429" alt="Schermafbeelding 2023-01-02 111924" src="https://user-images.githubusercontent.com/60787548/210219791-1c203683-5627-4fb4-83ff-b4f6dcd3038d.png">
 <p>They both failed</p>
 <p>Frontend:</p>
 <img width="870" alt="Schermafbeelding 2023-01-02 112314" src="https://user-images.githubusercontent.com/60787548/210219869-c563ad35-056a-4394-9e3f-e2d67fb5ea92.png">
 <p>Backend:</p>
<img width="920" alt="Schermafbeelding 2023-01-02 112347" src="https://user-images.githubusercontent.com/60787548/210219925-7d8c137a-69fd-4b75-b802-7902ff25196c.png">
 
<details>
 <summary>Examining the front-end errors</summary>
 <p>When looking at the front-end erros we will see 1 bug, when opening that bug we see that I accidentally used the height property two times in my css. This is easy to fix</p>
 <img width="769" alt="image" src="https://user-images.githubusercontent.com/60787548/210220499-837696ab-f57a-4611-a6e3-9e9edcd7cbe4.png">
 <p>There were also a few code smells present, those also consisted of using the same property being used twice</p>
 <img width="467" alt="image" src="https://user-images.githubusercontent.com/60787548/210220760-0c0d7432-628e-49ff-b447-bd7a1f2d4b24.png">
 <p>After changing that and checking the master we will see that it will pass</p>
 <img width="858" alt="image" src="https://user-images.githubusercontent.com/60787548/210222175-b674eb89-1e16-4938-b7ea-941fdcd5f5bc.png">
 <p>With a mayor security hotspot, which I will skip now and research for my security reseach</p>
 

 </details>
 
  <details>
  <summary>Examining the backend errors</summary>
   <p>When looking at the backend you will see a few security vulnerabilities, when openings these you will see that it asks to make DTO's objects of it. That would be indeed the better options but for my project now I will not do this</p>
   <img width="761" alt="image" src="https://user-images.githubusercontent.com/60787548/210229192-44f59e57-7ecf-4373-9881-d9d96cb8f17d.png">
  <p>You will also see a few code smells which consists of remaining packages, but that won't really do or the whole project will crash. So I will ignore those</p>
   <img width="884" alt="image" src="https://user-images.githubusercontent.com/60787548/210229371-6009e2e6-91c8-449a-a57f-c34a8bdea2a1.png">
   <p>When uploading the new version you will get this:</p>
   <img width="878" alt="image" src="https://user-images.githubusercontent.com/60787548/210230043-52dd07b9-80ab-41a4-80d2-9601ee24a3f7.png">
   <p>So this also passes</p>
</details>
 <p>After passing the SonarCloud test I will write a few tests to check if it actually does what it needs to do. So I installed Cypress on my front-end</p>
 <img width="722" alt="image" src="https://user-images.githubusercontent.com/60787548/210231063-c095f44f-46f9-428c-95cb-bffcb1c945ae.png">
<img width="674" alt="image" src="https://user-images.githubusercontent.com/60787548/210231125-8be370d9-b64e-4d3f-9b6d-13adc969a4a0.png">
 <p>I will set up a end-to-end test to test if the crud works</p>
 <img width="647" alt="image" src="https://user-images.githubusercontent.com/60787548/210241614-3686deac-5a6e-4b28-b0ec-cab339105d54.png">
 <p>So I created three scrips, to test if it can add something, edit something and delete something</p>
 <img width="832" alt="image" src="https://user-images.githubusercontent.com/60787548/210241715-83c2c4da-532a-484d-8109-948b441bb269.png">
<img width="869" alt="image" src="https://user-images.githubusercontent.com/60787548/210241751-69850179-c773-42ba-a906-3f43baa25ff0.png">
<img width="845" alt="image" src="https://user-images.githubusercontent.com/60787548/210241788-04eb6a4a-99e1-4157-9e5f-771af9035874.png">
 <p>Which will (if all goes well) all pass</p>
 <p>Add:</p>
 <img width="845" alt="image" src="https://user-images.githubusercontent.com/60787548/210242100-ab5a220f-0125-4778-b6a6-d4f816f4d8ad.gif">
 
  <p>Edit:</p>
 <img width="845" alt="image" src="https://user-images.githubusercontent.com/60787548/210242356-531b87b6-5cde-4a26-bae0-3d569a6f3c27.gif">

  <p>Delete:</p>
 <img width="845" alt="image" src="https://user-images.githubusercontent.com/60787548/210242543-733b2a55-771f-4a87-8b26-7799ef9da3ae.gif">

 <p>All the tests passed on both local and in Cypress Cloud</p>
 <img width="665" alt="image" src="https://user-images.githubusercontent.com/60787548/210244036-5518a576-4e94-4e53-9236-2f10d4809740.png">
<img width="1010" alt="image" src="https://user-images.githubusercontent.com/60787548/210244073-c7282bdf-493d-47c5-90d6-85fa875c6bf4.png">
<p> When running it on github actions they all fail</p>
<img width="690" alt="image" src="https://user-images.githubusercontent.com/60787548/210246633-d0a78066-c953-431c-b30d-07a9cad67687.png">
<p>This is not really shocking as it's trying to send the data to my local backend (which he will never find) So the next thing to do is to put my backend on a live envoirment, for with we will use docker</p>
 
 <p>I started by making a new webapp on azure for my backend</p>
 <img width="709" alt="image" src="https://user-images.githubusercontent.com/60787548/210324845-8113d653-d364-4683-953b-51674de9129a.png">
<p>And in my settings I set my public docker image</p>
<img width="922" alt="image" src="https://user-images.githubusercontent.com/60787548/210341355-b381e3eb-2103-455d-8de8-faa7d607da6d.png">
<p>And when I started my app it immediately crashed, after some research I found that Azure webapp runs on port :80 or :8080, but my app runs on port :8090 (due to it also running on my server which already has something assigned on that port), so I had to change the azure port. You can easily do this by going to the app settings</p>
<img width="847" alt="image" src="https://user-images.githubusercontent.com/60787548/210341893-ca7803a0-5544-4709-bd8c-73922ed317cb.png">
<p>And when running the app again you will see that it shows my data</p>
<img width="685" alt="image" src="https://user-images.githubusercontent.com/60787548/210342091-5872df92-8810-4b7b-92ce-9da9acffc819.png">
<p>So now we can change the front-end to get the data from the azure webapp (so the github tests will not fail)</p>
<img width="641" alt="image" src="https://user-images.githubusercontent.com/60787548/210342596-07650016-ad70-4f73-8455-ae50aa2bb1ec.png">
<p>And they indeed passed the tests</p>
<img width="641" alt="image" src="https://user-images.githubusercontent.com/60787548/210346868-3790dd4e-989f-4992-b384-7e7d4b156588.gif">

</details>


## 2: Software quality
```
Tooling and methodology: 
Carry out, monitor and report on unit integration, regression and system tests, with attention for security and
performance aspects, as well as applying static code analysis and code reviews.
```
<h3>SonarQube</h3>
First I started of by installing <a href="https://www.sonarqube.org/downloads/">SonarQube</a> locally , this however did not work for my system because when trying to opening it it just crashed.</br></br>

So my second attempt was by trying to run it in a Docker container. I followed the instructions on the website. </br> Opened a port and I was ready to go, atleast I thought...</br></br>
<img width="776" alt="image" src="https://user-images.githubusercontent.com/60787548/206403511-1ef089c3-5466-4a30-9ebf-7304e360e781.png"></br>
Inside SonarQube, I chose the "manually" option </br>
<img width="653" alt="Schermafbeelding 2022-12-01 100351" src="https://user-images.githubusercontent.com/60787548/206408101-d7bdea7f-f04e-41fe-a77b-5f0f16de3fe3.png"></br></br>
And chose to set it up as github actions for the continuous integrations. 
<img width="931" alt="Schermafbeelding 2022-12-01 100457" src="https://user-images.githubusercontent.com/60787548/206408821-861a4db6-7b13-4745-b84d-524ee74ec3ee.png">
</br></br>


After that it was time to setup my secrets in Github.</br>
<img width="623" alt="Schermafbeelding 2022-12-01 102031" src="https://user-images.githubusercontent.com/60787548/206406429-3f1c506b-2680-4778-9e86-5bdce78852a1.png"></br>
Build.yaml was all setup and ready to go, So I made the commit, and...</br>
<img width="986" alt="Schermafbeelding 2022-12-01 104715" src="https://user-images.githubusercontent.com/60787548/206406731-05addc8f-08c5-44ce-84c0-f8648332f252.png">
</br>
The first error code. After some searching around on the internet I figured out that my maven was not setup correctly. </br>
<img width="669" alt="Schermafbeelding 2022-12-01 111610" src="https://user-images.githubusercontent.com/60787548/206407037-752993c8-f476-4348-a6a6-b220057909b2.png"></br></br>
With new hope (after he succeeded where he first got the error message) I was ready for my code quality results. And when he was almost there...</br>
<img width="974" alt="Schermafbeelding 2022-12-01 113352" src="https://user-images.githubusercontent.com/60787548/206407489-e32f4ef3-4013-4451-903d-9f93afabb5d0.png"></br>
Another error message. When what the error message exactly said it hit me. This was never going to work. The Github actions was trying to push it to my local docker container, he was never going to find it. So it was time for another option.
</br></br>
<h3>SonarCloud</h3>
Using SonarCloud was an easier experience. You login with your Github and choose a (public) repository. </br>
<img width="899" alt="Schermafbeelding 2022-12-01 113543" src="https://user-images.githubusercontent.com/60787548/206411163-322cf473-c1fe-44f2-a1da-605f4b92581e.png"></br></br>
After following the instructions given by SonarQube (adding tokens etc.) He just runs the code and it works. </br>
<img width="1036" alt="Schermafbeelding 2022-12-01 114225" src="https://user-images.githubusercontent.com/60787548/206411631-e9c1d6a4-9838-4e19-bf9e-cfa6306fe094.png"></br>
<img width="895" alt="Schermafbeelding 2022-12-01 113743" src="https://user-images.githubusercontent.com/60787548/206411863-533e9d40-aa45-4b71-8edd-cfe9ede39c0f.png">
My code clearly needs some working on. </br>


<details> 
 <summary>What are the problems and how would you fix them?</summary></br>
 
 <h2>Code smells</h2>
 When looking at my code smells I saw mostly things like: "Remove this comment", and a few issues in a class that I didn't even use. So those were easily removed. There are some issues which were harder to fix. 
 </br> I got this error:</br>
 <img width="480" alt="image" src="https://user-images.githubusercontent.com/60787548/206417570-641a3c97-9b00-465e-bb94-0317d6805686.png">
 So in my project I have a class with public properties.
 </br><img width="326" alt="image" src="https://user-images.githubusercontent.com/60787548/206418174-1e2c838d-864a-410a-9a18-7bd30823415c.png">


 </details>




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
 I first looked at Scrum, the way I see it, it would work best in a groups project instead of an indivual project. So I have decided to work in the Crystal method cause that seemed like the most flexible option because I'm still figuring out what functionalities my project will consist of and because it's a short-term project.</br>
For my group project we use the Scrum method. We set up a Jira board with all the issues (and child issues) and split these into sprints. 
<a href='https://postimg.cc/NyZ4Rs7J' target='_blank'><img src='https://i.postimg.cc/XJYzSXZb/Schermafbeelding-2022-11-23-105130.png' border='0' alt='Schermafbeelding-2022-11-23-105130'/></a>

<img width="667" alt="image" src="https://user-images.githubusercontent.com/60787548/203517227-d3c61986-2928-478d-833d-34a4c2679fd2.png">
<img width="667" alt="image" src="https://user-images.githubusercontent.com/60787548/203518142-789e6e5f-3f66-4446-9597-a34b5af2a66f.gif"></br>
And we also use a time table to easily calculate how long we think we need to finish an issue:
<img width="1217" alt="image" src="https://user-images.githubusercontent.com/60787548/203518435-c886ea2c-9523-427d-8396-0078b0c331e9.png"></br>
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
 <summary>Research question: How does using docker containers positivly impact deploying my application</summary>
 </br>
 For my project I want use Docker to run my project on. When looking into alternative options I thought kept thinking if using docker could have a negative of positive impact on the performance. But before I can make a conclusion I need to first understand what Docker even is and why people use it.</br>
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
<p>
Docker is well known in the IT space, from software development to running minecraft servers, a lot of people use it to do 
different things with it, but why is Docker so loved? </p>
<h5>Scalability & Flexibility</h5>
<p>Docker uses containers which each contain their own set of configurations and dependencies, that way it's easier to run multiple instances of the same container at the same time. This means that it's simple to deploy multiple docker images on multiple servers. Changes within the project is also easy, you just change the thing you want to change, test it and deploy it. The developer can optimize and test the project without having any downtime. </p>
<h5>Fast Deployment</h5>
<p>By using Docker you can save a lot of time, the deployment is very fast because the docker images
are easy to handle. Docker is mostly used in a CI/CD workflow.</p>
<h5>Platform-independent apps</h5>
<p>When using Docker your apps will become OS independent. Which means you can run it on any platform 
(Linux, macOS, Windows etc.) A lot of developers like that about Docker. </p>
<h5>Less security issues</h5>
<p>Docker containers are way more secure than any normal app, Why? A container cannot access data from 
another container without having the proper authorization, it's even possible to add multiple security layers. </p>
<a href="https://www.jobsity.com/blog/8-reasons-why-docker-matter-for-devs">Why Docker matters for devs</a></br>


<h3> Which deploy alternatives are there? <h3>
<h6>DOT: literature research</h6>
<hr>
<p>Before Docker, people used other methods to deploy their application.</p>

<h4>Virtual machine</h4>
<p>You can run a virtual machine and run the app inside it. I do think (because you have to run a whole instants
of a Windows server inside it that it will not be very fast.</p>

<h3> Docker vs alternative option<h3>
<h6>DOT: System test?</h6>
<hr>
<p>To see if Docker is really the easier option from the start to finish I will set up a Virtual Machine (running Windows server) and a Docker container and see if deploying it by Docker is a more positive experience. </p>

<p>I will start by deploying my container app on my server, luckily this is very easy, I will just search for my app inside Unraid</p>
<img width="862" alt="image" src="https://user-images.githubusercontent.com/60787548/210553800-c324d685-7bbf-4cec-82b3-1402f65a704d.png">

<p>After that I set the port number to the same one my app uses (which is 8090)</p>
<img width="909" alt="image" src="https://user-images.githubusercontent.com/60787548/210554175-8d08aca2-3dc1-428b-84b4-c026c0ebb8f5.png">
<p>We will see that my app runs on port :8090</p>
<img width="651" alt="image" src="https://user-images.githubusercontent.com/60787548/210554422-a7fdad9e-93c2-464d-b095-d048cca71074.png">
<p>So now I can access my app when I go to that ip adress with that port</p>
<img width="599" alt="image" src="https://user-images.githubusercontent.com/60787548/210554929-d777198c-b60d-443f-adba-0cd1e85a0798.png">
<hr>
<p>For the windows server I started by adding the Roles and Features inside the Server Manager</p>
<img width="628" alt="image" src="https://user-images.githubusercontent.com/60787548/210555697-439f6a10-fea2-4eaa-84d8-ec842beec4c1.png">
 <img width="628" alt="image" src="https://user-images.githubusercontent.com/60787548/210556274-18b70133-61b5-4b52-9bee-f8c35a13baac.gif">


 <p>After that we see that the server is running on 10.0.15.55, and if we go to that address we see the simple windows server page</p>
 <img width="623" alt="image" src="https://user-images.githubusercontent.com/60787548/210556629-52f56e8b-fee8-43d9-827c-2600020d069e.png">
 <p>Next step is to get the backend of Hubflux running on it, for that I added FTP to be able to transfer the files to the server</p>
 <img width="504" alt="image" src="https://user-images.githubusercontent.com/60787548/210558121-6c09af25-ff63-4730-ab70-1001b1a10de5.png">
<img width="610" alt="image" src="https://user-images.githubusercontent.com/60787548/210558994-bd03354b-248a-4897-b419-81706419fb25.png">
 <img width="585" alt="image" src="https://user-images.githubusercontent.com/60787548/210559073-0c83f840-8071-4e96-9c93-0f1a3fb81001.png">
 <p>this was a fun attempt but that didn't really work in the end</p>
 
 <p>I downloaded FileZilla on my server and checked the ip-adress</p>
 <img width="435" alt="image" src="https://user-images.githubusercontent.com/60787548/210562573-110b29fb-4747-41f9-ae78-64d7050d2c46.png">

 <p>I tried pinging it with my own PC, but that didnt work</p>
 <img width="403" alt="image" src="https://user-images.githubusercontent.com/60787548/210562771-fcfae411-8f23-412c-b4f8-1b740984e0ed.png">

 <p>So I turned off the firewall and after that it did work</p>
 <img width="558" alt="image" src="https://user-images.githubusercontent.com/60787548/210563345-7cda5a39-1bd3-4b8b-bbf3-61a06e05f730.png">
<img width="560" alt="image" src="https://user-images.githubusercontent.com/60787548/210563494-89d38d3a-6489-4d99-8e02-d5a59384e99e.png">
 <p>Added a inbound rule for the local ip adress and turned the firewall back on </p>
 <img width="530" alt="image" src="https://user-images.githubusercontent.com/60787548/210564307-27918da3-4c24-46c0-8161-4f2e2f75be07.png">
<p>After a lot of trial and error I found out that an IIS windows server doens't really like sharing by FTP, and people recommended sharing the folder, so I did that</p>
 <img width="730" alt="image" src="https://user-images.githubusercontent.com/60787548/210566026-d46769ab-5efd-4b16-b0ed-f0e49d48f804.png">
 <p>That way I could acces the folder from outside the virtual machine</p>
  <img width="730" alt="image" src="https://user-images.githubusercontent.com/60787548/210566755-961802ba-41e9-4e5b-ba3e-6984136acf21.gif">

 <p>Clearly I didn't do my research correctly cause running a java based app on a IIS web service is not really recommended, and they recommend using docker to run it.</p>
 <img width="566" alt="image" src="https://user-images.githubusercontent.com/60787548/210733287-467b4cf2-d25e-404c-b352-576311771d45.png">
<p>So I decided to follow <a href="https://www.youtube.com/watch?v=OOVE_g6F8mQ&ab_channel=DanGeabunea%28RomanianCoder%29">this</a> video to run it as a service</p>

<p>Starting by downloading this from github on my server</p>
<img width="623" alt="image" src="https://user-images.githubusercontent.com/60787548/210735307-e92de065-dc1b-401c-93e9-a1612e75f45f.png">
<img width="508" alt="image" src="https://user-images.githubusercontent.com/60787548/210736260-c84b74b2-c60a-4f1c-81d7-0d4ab6bec5cc.png">
<img width="484" alt="image" src="https://user-images.githubusercontent.com/60787548/210737546-a3f8e68e-2f51-4396-96ce-a10c6baaf52f.png">
<img width="596" alt="image" src="https://user-images.githubusercontent.com/60787548/210738879-3f894d02-ed4d-4cb4-8622-a5bedb127714.png">
<img width="577" alt="image" src="https://user-images.githubusercontent.com/60787548/210739209-18a6a0bb-10d4-4bd2-a03b-75391e626bf6.png">
<p>This game me an error aswell, so it was time for plan B.</p>
<img width="1124" alt="image" src="https://user-images.githubusercontent.com/60787548/210740489-f4aebe5f-67cd-4a4b-8643-c9448f6fe73b.png">
<p>It's time for a linux server with apache</p>
<img width="664" alt="image" src="https://user-images.githubusercontent.com/60787548/210741700-e33aa19f-3d68-49ac-984b-5064a7d5fbc7.png">



 




<h3>Conclusion<h3>
<hr>

<p>No conclusion yet</p>

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

<h2>Masculinity / Femininity</h2>
<blockquote cite="https://www.andrews.edu/~tidwell/bsad560/HofstedeMasculinity.html">
"Masculinity is seen to be the trait which emphasizes ambition, acquisition of wealth, and differentiated gender roles.  Femininity is seen to be the trait which stress caring and nurturing behaviors, sexuality equality, environmental awareness, and more fluid gender roles."
</blockquote>
<a href="https://www.andrews.edu/~tidwell/bsad560/HofstedeMasculinity.html.">Source</a>
</br>
There are a few differences between Masculinity and Femininity, here are they summed up:</br>
<h3>Social Norms</h3>
<table>
  <tr>
     <th>High Masculinity</th>
    <th>Low Masculininity (Femininity)</th>
  </tr>
 <tr>
    <td>Ego oriented</td>
    <td>Relationship oriented</td>
  </tr>
  <tr>
    <td>Money and things are important</td>
    <td>Quality of life and people are important</td>
  </tr>
 <tr>
    <td>Live in order to work</td>
    <td>Work in order to live</td>
  </tr>
</table>
</br>
<h3>Politics and economics</h3>
<table>
  <tr>
     <th>High Masculinity</th>
    <th>Low Masculininity (Femininity)</th>
  </tr>
 <tr>
    <td>Economic growth is high priority</td>
    <td>Envirioment protection is high priority</td>
  </tr>
  <tr>
    <td>Conflict solved through force</td>
    <td>Conflict solved through negotiation</td>
  </tr>
</table>
</br>
<h3>Religion</h3>
<table>
  <tr>
     <th>High Masculinity</th>
    <th>Low Masculininity (Femininity)</th>
  </tr>
 <tr>
    <td>Most important in life</td>
    <td>Less important in life</td>
  </tr>
  <tr>
    <td>Only men can be priests</td>
    <td>Both men and women as priests</td>
  </tr>
</table>

</br>
<h3>Work</h3>
<table>
  <tr>
     <th>High Masculinity</th>
    <th>Low Masculininity (Femininity)</th>
  </tr>
 <tr>
    <td>Larger gender wage gap</td>
    <td>Smaller wage gap</td>
  </tr>
  <tr>
    <td>Fewer woman in management</td>
    <td>More woman in management</td>
  </tr>
   <tr>
    <td>Preference for higher pay</td>
    <td>Preference for fewer working hours</td>
  </tr>
</table>

</br>
<h3>Family and school</h3>
<table>
  <tr>
     <th>High Masculinity</th>
    <th>Low Masculininity (Femininity)</th>
  </tr>
 <tr>
    <td>Traditional family structure</td>
    <td>Flexible family structure</td>
  </tr>
  <tr>
    <td>girls cry, bots don't, boys fight, girl's don't</td>
    <td>Both boys and girls cry; neither fight</td>
  </tr>
   <tr>
    <td>Failing is a disaster</td>
    <td>Failing is a minor accident</td>
  </tr>
</table>
</br>
When looking at the Netherlands we score a "14", which means we score in the low masculinity (also known as femininity) category. When looking at the <a href="http://clearlycultural.com/geert-hofstede-cultural-dimensions/masculinity/">index</a> we see that a few high scoring countries are Japan, Hungary and Austria. With a few of the lowest being Sweden, Norway and the Netherlands.</br>
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204794021-1d6c46a2-51f1-4b18-9754-b69becc1d886.png"></br>
</br>


<h2>Long-Term Orientation</h2>
<blockquote cite="https://www.cqfluency.com/cqpedia/long-term-orientation-vs-short-term-orientation-lto/#:~:text=Long%2Dterm%20orientation%20focuses%20on,persistence%2C%20perseverance%2C%20and%20adaptability.">
"Long-term orientation focuses on the future. Long-term oriented individuals may put off short-term affairs in preparation for the future. Long-term oriented cultures place emphasis and value on persistence, perseverance, and adaptability."
</blockquote>
<a href="https://www.cqfluency.com/cqpedia/long-term-orientation-vs-short-term-orientation-lto/#:~:text=Long%2Dterm%20orientation%20focuses%20on,persistence%2C%20perseverance%2C%20and%20adaptability.">Source</a>
</br>
Long term cultures tend to be more collective, they are more likely to think in "we" rather then "I", a few cultures that have a long term culture are countries like China, Japan and South Korea.</br></br>
Netherlands scores a '67', which means it has a pragmatic nature. In pragmatic societies people believe the truth depends on the situation, context and time. But have the ability to easily adapts to change conditions.</br></br>
Compare that to Ireland which scores a '24', they have a strong concern with establishing the truth. They show great respect for traditions and focus on achieving quick results. </br>
<img width="591" alt="image" src="https://user-images.githubusercontent.com/60787548/204796519-9d3faf81-4889-4183-867e-4a07a3067ab9.png"></br>



</details>
<details> 
 <summary>Real life example with a cultural difference</summary>
<p>When I needed help with my computer (at work) I was send to the help desk which
consisted of a few indian it people. </p>

<p>When I explained my problem they were convinced they could help me with my problem, 
but after a two-hour teamviewer call, a lot of digging through my computer
and a lot of back and forth between different colleagues the problem still wasn't fixed.
</p>

<p>When looking at the cultural differences between India and
Netherlands we see that India has a higher masculinity score than
the Netherlands, for indians to say "no sorry, I don't know the anwser" 
is not an option, even when they don't know the answer they will still help you</p>
<img width="536" alt="Schermafbeelding 2022-12-14 145935" src="https://user-images.githubusercontent.com/60787548/207626365-8466d8b4-7a4b-47c3-b5b0-0d9b27c58794.png">

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
 <a href="https://ethics.acm.org/code-of-ethics/software-engineering-code/">The Software Engineering Code of Ethics and Professional Practice</a>
<p>If you look at the ethics of my group project you will get the following:</p>
<img width="800" alt="Schermafbeelding 2022-12-14 145935" src="https://user-images.githubusercontent.com/60787548/207626234-e2695b2b-6055-413b-8cd1-dbafcecaed48.png">

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
 <details> 
  <summary>Individual project requirements</summary>
<p>For my individual project I have a few requirements:</p>
<ul>
 <li>Add login feature</li>
 <li>Show a notification when a new episode is available</li>
 <li>Have a homepage to show the streaming services and watch progress</li>
</ul>
</details>
 <details> 
  <summary>Group project requirements</summary>
<p>My group project is a big team consisting of 5 members, together we 
made Ordinner with the following requirements:</p>
<h3>Homepage/customer page</h3>
<ul>
 <li>Functionality to place order</li>
 <li>Able to change languages</li>
</ul>
<h3>Bar</h3>
<ul>
 <li>Show orders (load immediately automatically)</li>
 <li>Cash register system to pay for orders</li>
 <li>Able to make order for table</li>
 <li>Able to delete items from a order</li>
 <li>Switch table number from orders</li>
 <li>Able to change languages</li>
</ul>
<h3>Kitchen</h3>
<ul>
 <li>Show food from orders (load immediately automatically)</li>
 <li>Able to change languages</li>
 <li>Change order status</li>
</ul>
<h3>Management</h3>
<ul>
<li>Able to change languages</li>
<li>Show all orders from specific period of time (with statistics?)</li>
<li>Show stock</li>
<li>Run accounting feature</li>
<li>Show history from all actions</li>
</ul>
<p>All these requirements are made into issues that are divided into sprints on our Jira board. </p>
<img width="1064" alt="image" src="https://user-images.githubusercontent.com/60787548/207646346-702e4d24-6af0-4192-a3f5-e8332d21b389.png">

</details>
 <details> 
  <summary>Project software designs</summary>
 <p>For my individual project I made a Container Diagram:</p>
 <img width="700" alt="image" src="https://user-images.githubusercontent.com/60787548/207838290-3660a1f0-6e8e-464b-b1d0-ef1c7eefdfc3.png">
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
<p>
For our business process I decided to zoom into the "taking orders" within 
our app, because our base design 
(<a href='https://github.com/brittbrink/S3-DB02-Portfolio#leeruitkomst-7-business-processen'>made my Britt</a>) was very global, and our app is a little more complicated than was shown in the base design
</p>

<p>
I made a design to show the process with and without our app.
</p>
<img width="1644" alt="Swimming Lane detailed without app" src="https://user-images.githubusercontent.com/60787548/208436216-c97b3ab5-1638-413b-a0f4-3cbd71238d4f.png">
<img width="1497" alt="Swimming Lane" src="https://user-images.githubusercontent.com/60787548/208436230-9cd402fc-d5a6-45bd-9e70-6072055f6a9c.png">
<p>
When looking at the two design, you will see that our app will replace a lot of the
tasks that the bar personal would normally do. A lot of Bar personal won't really be needed when restaurants will use our app so I think a few people might lose their job.
</p>

## 8: Professional
```
Professional manner: 
You develop software as a team effort according to a prescribed software methodology and following team agreements. 
You are able to track your work progress and communicate your progress with the team.

You actively ask and apply feedback from stakeholders and advise them on the most optimal technical and
design (architectural) solutions. You choose and substantiate solutions for a given problem.
```

<p>For our group project I was responsible (with Britt) for the comminication between our group and the stakeholders. That meant that we 
had to write a lot of emails, like this one for example:</p>
<img width="869" alt="image" src="https://user-images.githubusercontent.com/60787548/203740089-3c97157e-994f-444d-9731-531b8f6a423c.png">
<p>To keep track of my progress I had a few progress/feedback conversations with my teachers.</p>
<img width="628" alt="image" src="https://user-images.githubusercontent.com/60787548/203740409-69fbedb4-76e1-4e3c-a30f-6e6e70734e83.png">
<p>At our third spint review we had to give a presentation, but because our group wasn't that well prepared at the time I decided to lead the presentation</p>



