{% include "../includes/header.md" %}

<!-- @TODO ATTENTION: DEVELOPER, You'll see this large chunk of comments as you develop, use them to guide you're work. A few short-cuts that will make your time move faster. Each section looks the same:

1) "Overview", "Read It", "See It", "Practice It", "Know Your Docs" if you use find/replace you can change Subject1 to the first concept and Subject2 to the next concept. You're not limited to only 2 subject so if needed, add a 3rd section.  

2) Videos in "See It" Sections should be embedded and linked to the title use find/replace to change out urls for LINKtoVIDEO1 and LINKtoVIDEO2 

3) Same for "Practice It" Sections, find/replace URLtoEXAMPLE1 or URLtoEXAMPLE2 

4) If you're linking to a blog or article please make the hyperlink descriptive not just say "for more information click [here](url)". Instead it should be, "if you want to know more about [Angular's Architecture read this article](url)."

5) In-line files and code should be marked with back-ticks `var code = "sample"`, `src/myFile.js`

6) To show large chunks of code put it inside code fences, triple back-tics with the language specified on the top line.
  csharp, typescript, css, html, javascript, ....

  ```javascript
    // use code fencing to write out code
  ```

7) If you need to create a repo for the student to clone:
  * Create the repo in the AustinCodingAcademy gitHub account and,
  * use the naming " NG421_W7D1_QuizAPI "

Happy Code Teaching!
-->

# Pre-Homework - Angular Components

*InspirationalQuote*

## Review and Recap
<!-- @TODO ATTENTION: DEVELOPER, Quickly cover the last prep work and how it bring the student to these new topics. Remember to guide their learning experience and move them through fluidly. The student is our customer and we must create a wonderful user experience for them.  -->

We have built our Angular project from the cli tool. Now we have to actually make something for ourselves.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

## Component Overview

### The Problem
An industry standard approach to building web apps with all UI tools such as Rectjs, Vue and Angular is to organize code into components. Component is a term for a custom html element. We want to build our own custom elements such as `<my-element>`. You cannot do this without a tool like Angular.
### The Solution
We need to learn how to build components in Angular.


******

### See It - [Understanding components](LINKtoVIDEO1)

<!-- @TODO ATTENTION: DEVELOPER, 
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/1sQj3RKwGQyoHzbHGZ9ix7oY3Qx4n4sAV/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******
### See It - [Making a Basic Component](LINKtoVIDEO1)

<!-- @TODO ATTENTION: DEVELOPER, 
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/1jIuugvlSyYGqO4_Zw6bTFbP9CXNFls4J/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******


### Practice It - [Make a Component](https://stackblitz.com/edit/angular-starter-421-day1-makeacomponent)

<!-- @TODO ATTENTION: DEVELOPER, 
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Log into stackblitz with your github account.
1. Go to [this stackblitz project](https://stackblitz.com/edit/angular-starter-421-day1-makeacomponent) and fork it
1. Follow the exact steps as shown in the video to make your own component in Angular
1. Slow down, speed up, pause, rewind and fast forward the video as necessary 
1. When complete submit the link to the pre work homework entry for PreWork_Day1_FirstComponent

******

### Know Your Docs - Angular Components
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [Angular Components](https://angular.io/guide/architecture-components). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******
******

## Component Generator

<!-- @TODO ATTENTION: DEVELOPER, In the overview, students should see the why of what they're about to learn about. This is the place for you to use metaphors or familiar everyday objects to relate the abstract computer concept to. Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.-->

Let's learn how to use software tools to help us do repetitive tasks.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

### Read It - Component Generator

<!-- @TODO ATTENTION: DEVELOPER, Give them something to read in your words, as if you were talking to them about the topic. Within the reading you can link to a few articles: Medium, Wikipedia, Microsoft, CSS-Tricks, W3S, MozillaDev, etc... anything that can help give more perspective on the subject.  -->

At this point, we know how to make the most basic component possible. We had to make several files and import those files into other locations. I don’t know about you, but I consider that to be a lot of work we did. The thing is, I said that this is the standard operating procedure. We do this every time we want to make a component. Well, why do we have to do this? Why can’t the computer do this for us? Luckily it can. We can use the Angular CLI tool to do all this stuff for us.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

******

### See It - [ng generate](https://drive.google.com/file/d/1SeFvRAohVj3JlyeT5lXpxMsklLPpHPaN/preview)

<!-- @TODO ATTENTION: DEVELOPER,
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/1SeFvRAohVj3JlyeT5lXpxMsklLPpHPaN/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******

### Practice It - [Subject2](URLtoEXAMPLE2)

<!-- @TODO ATTENTION: DEVELOPER,
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Run the ng new command to make a project
1. Run the ng generate command to build a new component

******

### Know Your Docs - ng generate
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [Subject2](URLtoDocs2). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******






******

## Template Interpolation

<!-- @TODO ATTENTION: DEVELOPER, In the overview, students should see the why of what they're about to learn about. This is the place for you to use metaphors or familiar everyday objects to relate the abstract computer concept to. Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.-->

Let's learn how to populate our component html with dynamic data with template interpolation.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

### Read It - Template Interpolation

<!-- @TODO ATTENTION: DEVELOPER, Give them something to read in your words, as if you were talking to them about the topic. Within the reading you can link to a few articles: Medium, Wikipedia, Microsoft, CSS-Tricks, W3S, MozillaDev, etc... anything that can help give more perspective on the subject.  -->
Do you see anything wrong with the component we have made? Hopefully you noticed that our component isn't very reusable as the html is hard coded to the same thing. If you use your component in multiple places it will show the same information. We need to be able to re use the html but make the information such as first name dynamic.

<!-- @TODO ^^^ Replace Example Text ^^^ -->

******

### See It - [Template Interpolation]()

<!-- @TODO ATTENTION: DEVELOPER,
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/1_4SYliWNf6h5cTpMxVngyPHn_aAPfXuh/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******

### Practice It - [Template Interpolation](URLtoEXAMPLE2)

<!-- @TODO ATTENTION: DEVELOPER,
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Try updating your component to use a class property
1. Populate the html template with data using interpolation

******

### Know Your Docs - Subject2
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [Subject2](URLtoDocs2). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******

******

## Lifecycle Hooks

<!-- @TODO ATTENTION: DEVELOPER, In the overview, students should see the why of what they're about to learn about. This is the place for you to use metaphors or familiar everyday objects to relate the abstract computer concept to. Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.-->

Let's learn hwo to use lifecycle hooks as the appropriate place to initialize data.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

### Read It - Lifecycle Hooks

<!-- @TODO ATTENTION: DEVELOPER, Give them something to read in your words, as if you were talking to them about the topic. Within the reading you can link to a few articles: Medium, Wikipedia, Microsoft, CSS-Tricks, W3S, MozillaDev, etc... anything that can help give more perspective on the subject.  -->


<!-- @TODO ^^^ Replace Example Text ^^^ -->

******

### See It - [Lifecycle Hooks]()

<!-- @TODO ATTENTION: DEVELOPER,
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/1R0OjrtzVF5Jz23bO7fo-0urdHWV9UfmI/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******

### Practice It - [Lifecycle Hooks](URLtoEXAMPLE2)

<!-- @TODO ATTENTION: DEVELOPER,
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Try updating your component to use the OnInit lifecycle hook to initialize a class property

******

### Know Your Docs - Subject2
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [Subject2](URLtoDocs2). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******




******

## Looping in Templates

<!-- @TODO ATTENTION: DEVELOPER, In the overview, students should see the why of what they're about to learn about. This is the place for you to use metaphors or familiar everyday objects to relate the abstract computer concept to. Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.-->

Let's learn how to use dynamic data to generate multiple html elements based on that data.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

### Read It - ngForOf

<!-- @TODO ATTENTION: DEVELOPER, Give them something to read in your words, as if you were talking to them about the topic. Within the reading you can link to a few articles: Medium, Wikipedia, Microsoft, CSS-Tricks, W3S, MozillaDev, etc... anything that can help give more perspective on the subject.  -->


<!-- @TODO ^^^ Replace Example Text ^^^ -->

******

### See It - [ngForOf]()

<!-- @TODO ATTENTION: DEVELOPER,
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/12JyGMKPEi6WmnRVnyVODonv-wNG3uLNH/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******

### Practice It - [ngForOf](URLtoEXAMPLE2)

<!-- @TODO ATTENTION: DEVELOPER,
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Try updating your component to use the ngForOf

******

### Know Your Docs - Subject2
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [Subject2](URLtoDocs2). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******



******

## Conditional Rendering

<!-- @TODO ATTENTION: DEVELOPER, In the overview, students should see the why of what they're about to learn about. This is the place for you to use metaphors or familiar everyday objects to relate the abstract computer concept to. Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.-->

Let's learn how to conditionaly render html elements based on dynamic data.
<!-- @TODO ^^^ Replace Example Text ^^^ -->

### Read It - NgIf

<!-- @TODO ATTENTION: DEVELOPER, Give them something to read in your words, as if you were talking to them about the topic. Within the reading you can link to a few articles: Medium, Wikipedia, Microsoft, CSS-Tricks, W3S, MozillaDev, etc... anything that can help give more perspective on the subject.  -->


<!-- @TODO ^^^ Replace Example Text ^^^ -->

******

### See It - [NgIf]()

<!-- @TODO ATTENTION: DEVELOPER,
1) This should be a clear, high-quality, non-lame video that helps visually explain the concept at-hand. 
2) It can come from youTube as long as it doesn't advertise or come from another code school. 
3) Preferably, all video content should come from ACA. 
4) THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!!
-->

<iframe width="560" height="315" src="https://drive.google.com/file/d/14FBojbJoteik-4Rir3-2QHnyHctgIwte/preview" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

******

### Practice It - [NgIf](URLtoEXAMPLE2)

<!-- @TODO ATTENTION: DEVELOPER,
1) Insert an iframe of a DotNet Fiddle, CodePen, or Repl.it with  pre-built code block(s) for the student to begin tinkering with quickly. 
2) The Code Sandbox should owned by ACA; 
3)if you don't have the credentials for the ACA account ASK!!. 
4)In the sandbox above you will do x, y, z. Give the student  instructions to get them in to the code more quickly. Remember, they're very young and you will need to guide them a little more to get them going. -->

1. Try implementing NgIf in a stackblitz project

******

### Know Your Docs - NgIf
<!-- @TODO ATTENTION: DEVELOPER, Student's often forget there is documentation to use. Give them the link so they know where it is. -->

Be sure to reference the official documentation on [NgIf](https://angular.io/api/common/NgIf). Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******





## Questions for Class Discussion
<!-- @TODO ATTENTION: DEVELOPER, Write down a few questions you'd like to ask the student by the time they've finished this pre-homework. We'll copy/paste them to the following class day. -->
Now that you've read, watched and practiced these concepts take your understanding a little deeper. Let's make sure we internalize these concepts by answer the questions below. We'll use these as a starting point for class discussion tomorrow. Don't rely on the Instructor or students to answer these question, **DO IT FOR YOURSELF NOW**. The time is now! Go *google*-up these on your own and have other questions to ask. We do not lecture in class, we discuss, collaborate and learn together.

1. ...
1. ...
1. ...

### Terminology to Know
<!-- @TODO ATTENTION: DEVELOPER, In this section, we list terms students should now and be able to discuss at this point. Be sure to list a few for the students to jot down and work with. -->
Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

1. ...
1. ...
1. ...

## Daily Puzzle Practice

In class we'll work on solving problems while communicating to a group. To get better at this, (*and you will*), you'll have to practice on you're own everyday. YES, the first few times you work on this you're going to get stuck, frustrated, and want to give up. That's okay. Just take a breathe and take some time away from it. Ten minutes later, come back to it. Then look at the answer. Understand how it was solved and try to repeat it for yourself. In this way you can learn from **REALLY** smart people. Slowly, but surely, you will pick up the patterns.

We want you to succeed! To make sure our students are doing the right practice, **everyday**, for themselves we're going to give you a problem to work on here. But if you're wanting more to work on try these sites:

* [HackerRank](https://www.hackerrank.com)
* [Geeks4Geeks](https://www.geeksforgeeks.org)
* [LeetCode](https://leetcode.com)
* [Pramp](https://www.pramp.com)

In fact, you'll want to get on [HackerRank](https://www.hackerrank.com) and [LeetCode](https://leetcode.com) sooner rather than later because they actually track your progress and your profile is searchable by hiring managers and recruiters!

Remember to follow the rules to Whiteboarding Success:

1. Restate, rewrite, and clarify the question
1. Write the expect return given an input
1. Make a code plan and speak aloud with your interviewers/team/self
1. Test and come up with edge case scenarios
1. Revise if you can for efficiency

<!-- @TODO ATTENTION: DEVELOPER, every pre-homework needs a good challenge for students to whiteboard on their own. Make sure to give them a prompt, example input and expected output -->
> Prompt Goes Here

  ```javascript
    // use code fencing to write out code
  ```

******
******

### Let's go to the [in Class Lesson >](01DayClass.md)

{% include "../includes/footer.md" %}
