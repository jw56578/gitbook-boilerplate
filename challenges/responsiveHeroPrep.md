{% include "../includes/header.md" %}

# Day 2 Pre-Homework - Media Queries

## Purpose

<!-- Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.  -->
People viw the web on many different devices from desktops to iPhones, Androids, Alexas, iPads, Kindles, smartWatches, smartTVs, etc. With so many ways to view, we as developers must know how to design for each and ensure our content is properly rendered on each of these devices. To do this, we use what's called a Media Query. It does exactly what it says, it queries the device requesting our page and returns back the proper CSS file according to the type of device.

## Prep For Your Career

### Code Everyday

<!-- This is where we give them a background to the history or common practice in the industry. We must remember they have no idea how the tech world works. Give them the why behind the ACTION ITEM -->
Nothing is worse than cold code. Cold code doesn't feel good. It doesn't make a lot of sense, and it doesn't inspire one to code more. Therefore, you must code everyday!

Realize now, you are planning to work as a developer. You choose this school to learn this skill because you want a new career in development as a coder. If this is true you must learn to love to code everyday. If you do, you will become infinitely better each day you commit to coding.

This doesn’t mean you have to come up with new projects every day. But it does mean practicing consistently.

And while you’re at it, take the time to learn the [ins and outs](https://code.visualstudio.com/docs/introvideos/basics) of your code editor. Learn the shortcuts and try using it without relying on your mouse or your track pad. You’ll be amazed at how much more productive you’ll be once you actually know all the features your main tool has.

### Action Item

<!-- This is a specific task they can do. It needs to be small and make them feel they are actually contributing to the their career, LinkedIn profile update, follow people on medium, youTube, GitHub, Reddit, Hackernews, etc... -->
**Make your schedule and present it to the class tomorrow.**
Create a schedule for yourself to code on a regular basis. Even on the weekends! Once you've created a schedule you need to follow it. Once you've followed it for just *two weeks* you have created a habit. Once you have a habit, you will be hard-pressed to break it. And when you do, you'll want to come back to it as soon as possible.

*Absence makes the heart grow fonder.*

**Use the example below as a guide.**

Day|Time
-|-
Monday|06:00 - 08:00
Tuesday|18:00 - 21:30
Wednesday|06:00 - 08:00
Thursday|18:00 - 21:30
Friday|06:00 - 08:00
Saturday|08:00 - 12:00  14:00 - 15:30
Sunday|18:30 - 19:30

<!-- ### Q&A - Topic
**Question: The question?** -->
<!-- Should include a short video clip of a grad asking a question about the topic. This will bring them context to the what their doing and why its important. Again, always instilling confidence!! -->
<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/XQu8TTBmGhA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> -->

## Responsive Web Design

<!-- This is how each subject should be introduced. Give the students structure so they know they can start trusting the process sooner!  -->
As it says in the name, it is a web design that responds to what ever device is requesting. Our job as developers is to build multiple views, one for each device we expect our web app to be viewed on and provide the appropriate view to each one. In the lesson were going to focus on just three: mobile, desktop and tablet.

### Read It - Why is Responsive Web Design Important

<!-- Give them our writing of the subject then link to a few articles: Medium, Wikipedia, CSS-Tricks, W3S, MozillaDev, etc... that help give more perspective on the subject  -->
[About](https://marketingland.com/mobile-top-sites-165725) 56% of all web traffic is mobile. This is a huge portion of traffic and you need to be a part of it! Take any website you're fond of, say [SmashingMagazine](https://www.smashingmagazine.com/2013/05/the-state-of-responsive-web-design/). Navigate there, be sure you're out of full-screen mode and grab the edge of the window and shrink it to the width of a phone. What happens?

This is reponsive web design. Most web pages have this functionality built in and were going to learn to do it ourselves!!

### See It - Media Queries in Action

<!-- Can be a video on youTube as long as it doesn't go to another code school. Eventually all video content should come from ACA. -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/h3IdEqpjMvQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

### Practice It - Media Queries

<!-- Section for Code Pen -->

#### CodePen Instructions

* Open up the CodePen in a new tab.
* Be sure you're not in full-screen mode .
* Grab the edge of the window and shrink it to the width of a phone.
* Watch the navigation button on the left side.
* Cool right?

<p data-height="265" data-theme-id="0" data-slug-hash="MPQBje" data-default-tab="css,result" data-user="hipperger" data-pen-title="Responsive CSS3 Side Navigation Menu" class="codepen">See the Pen <a href="https://codepen.io/hipperger/pen/MPQBje/">Responsive CSS3 Side Navigation Menu</a> by Clayton Berger (<a href="https://codepen.io/hipperger">@hipperger</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

## How to Apply Media Queries

<!-- This is how each subject should be introduced. Give the students structure so they know they can start trusting the process sooner!  -->
Above we've been focusing on Method 2: applying it in your CSS file. But let's explore both methods a little more broadly.

### Read It - Different Ways to Do Media Queries

A *media query* is a [CSS3 module](https://css-tricks.com/css-modules-part-1-need/) that allows content to adapt to conditions such as screen resolution (e.g. smartphone screen vs. computer screen). It is a cornerstone technology of responsive web design.

> As is the case with all the technical jargon you'll encounter at ACA (and beyond), it is hugely beneficial to pause for a moment and try break down what these words mean, and describe the concept to yourself in your own words.

> The technical term here - ***'media query'*** - can be broken into two disparate terms, which are quite simple to reason with:
> - 'media' - in the context of web development, you'd be right to assume that we're referring to devices such as laptops, tablets and smartphones which are used to access web content.
> - 'query' - a **question**, usually expressed in a formal or otherwise structured way.

> Putting it all back together, we can infer that a **media query** is an instance of *querying* for some particular aspect of a particular *media type* - that aspect being, in this case, a dimensional attribute such as `width` or `height`.

#### Method 1: as a `media` attribute

A media type can be declared in the `head` of an HTML document using the `media` attribute on a `<link />` element.

```html
<!-- CSS media query on a link element -->
<head>
  <link rel="stylesheet" media="(max-width: 400px)" href="my400wide-style.css" />
  <link rel="stylesheet" media="(max-width: 800px)" href="my800wide-style.css" />
</head>
```

#### Method 2: in your CSS

An alternative method of implementing media queries (and the one we'll using the most) is to specify them directly within your CSS:

```css
/* CSS media query within a stylesheet */

@media (min-width: 600px) {
  .column {
    color: blue;
  }
}
```

### Enabling Media Queries On Mobile Devices

To enable media queries on mobile devices, you can simply add this line to your `<head>` section.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

This line is to be added to the `<head>` section of every page that you write...forever until the end of time.

Additional options can be found here: https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag

### Popular Media Queries

To have your CSS respond to different screen sizes, you can simply ask, or "query", the screen size and apply special CSS rules. A media queries can very quickly get out of hand, so here is a cheatsheet for pretty much all the media queries you'll ever need!

```css
/* Extra Small and up (Portrait Phones) */

/* Small and up (Landscape Phones) */
@media (min-width: 576px) {

}

/* Medium and up (Tablets) */
@media (min-width: 768px) {

}

/* Large and up (Desktops) */
@media (min-width: 992px) {

}

/* Extra Large and up (Wide Screen Desktops) */
@media (min-width: 1200px) {

}
```

### See It - CSS Media Queries

<!-- Can be a video on youTube as long as it doesn't go to another code school. Eventually all video content should come from ACA. -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2KL-z9A56SQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Key Questions

* Environment
  * What is Visual Studio Code?
  * What is the Command Line Interface (CLI)?
  * Why is it used so much?
  * What benefits do you think it offers?
* Git
  * What is Git? Why do we use it?
  * List the key git terminal commands you will use in this class.
  * Explain how local repositories interact with the cloud repository on github.com.
  * What is the difference between git and github?
  * How do you think professional web developers use git in their jobs?
  * How do you host a website on github pages?
  * Be sure to look at the common git commands in your textbook's [home file](home.md)
  * Review the [DevTips GitHub For Noobs](https://www.youtube.com/watch?v=1h9_cB9mPT8&list=PLqGj3iMvMa4LFz8DZ0t-89twnelpT4Ilw) series.
* CSS Selectors
  * What's the difference between class and id? How to you reference them in your css file?
  * What is Inheritance as it relates to CSS?
  * What does !important do in CSS.
  * What is are pseudo-elements and pseudo-classes.

## Go to [Week 2 Day 2 Classwork >](02DayClass.md)

{% include "../includes/footer.md" %}
