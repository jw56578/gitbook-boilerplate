{% include "../includes/header.md" %}

# Pig Latin

*“Trust yourself. You know more than you think you do.” -Benjamin Spock*

## Today's Checklist

1. Daily Presentation
1. Whiteboard Training
1. Questions for Discussion
1. Ensure you have installed all dependencies/packages: `npm install`
1. Instructor covers the `package.json` and what the `scripts` and `test` are.
1. Ensure you know how to run test for each program:
    * `npm test 02Week/pigLatin.js`
1. Whiteboard a solution to building a Pig Latin program
1. Translate the broad ideas to psuedo code
1. Convert the psuedo code to real Javascript Code
1. Type into your text editor the Javascript code you've come up with one step at a time
1. Work through your bugs.
1. Achieve green checks for each of your unit tests.

******
******

## Daily Presentation

*VS Code Packages - Present to the class 3 useful and under utilized packages for VS Code.*

## Daily Whiteboard Training

Interviewing for development jobs is tough! To prepare yourself for the challenges ahead we will practice white boarding in-front of the class every day. Think of it as a warm-up for the project that awaits. The white boarding challenges should be taken seriously and practiced even outside of class. Help yourself by following these steps to attack the problem, work through the problem and collaborate with your interviewer(instructor):

  * Restate the question aloud.
  * Write the question out at the top of the whiteboard.
  * Ask any clarifying questions you need.
  * Invoke the function and write out the expected output given the sample input. If none is given, make it up.
  * Write out a code plan to the side of the whiteboard.
  * Speak aloud every thought you have. **THIS IS THE MOST IMPORTANT!**
  * Build the structure of your function(s)
  * Slowly work through your code plan building the steps you need.
  * Don't be afraid to mess up and say it aloud.
  * It's not about finding the solution. It's about collaborating and working toward a solution!
  * After you finish, take a picture and transfer it to a repl.it when you get home.

**PROMPT**
Take an array of numbers, raise them by the power of two and return the sum of the new array

## Questions for Discussion

* What is a function?
* Explain the syntax for functions.
* What are closures?
* How do you use scope when constructing functions?
* Why is it important to consider context in while you build functions?
* What are decomposition method and how do you use them?
* What are fat arrow functions?

******
******

# Pig Latin Overview

Today you'll practice building functions that take in arguments, practice passing arguments into functions and learning about scope and context as well as practicing the new and standards fat arrow syntax for a function.

```javascript
toPigLatin("Pig Latin") // => Igpay Atinlay
```

[What is Pig Latin](https://en.wikipedia.org/wiki/Pig_Latin)
> Pig Latin is a language game in which words in English are altered, usually by adding a fabricated suffix or by moving the onset or initial consonant or consonant cluster of a word to the end of the word and adding a vocalic syllable to create such a suffix.[1] For example, Wikipedia would become Ikipediaway (taking the 'W' and 'ay' to create a suffix). The objective is to conceal the words from others not familiar with the rules. The reference to Latin is a deliberate misnomer; Pig Latin is simply a form of argot or jargon unrelated to Latin, and the name is used for its English connotations as a strange and foreign-sounding language. It is most often used by young children as a fun way to confuse people unfamiliar with Pig Latin.

Today you're going to build the logic for this fun little program.

### Example

[Pig Latin Translator](https://funtranslations.com/pig-latin)

### Instructions

<!-- There should be clear step by step instruction so the material can be asyncronously consumed. This will significantly help our students learn, review and improve your teaching experience.  -->

1. Students will build the Pig Latin application.
1. Off of `master` create a new branch called: ` pigLatin `
1. Place your code in the /02week/pigLatin.js file in your javscript workbook.
1. The basic idea of Pig Latin is to take the first letters of the word up to the first vowel, move them to the back, and add 'ay' to the end of it.

  ```javascript
  pigLatin('car') //=> 'arcay'
  pigLatin('create') //=> 'eatecray'
  pigLatin('pony') //=> 'onypay'
  pigLatin('egg') //=> 'eggyay'
  ```

1. Whiteboard Pig Latin before building it.

### Follow-up Video

<!-- This video will come from ACA. It should be a place that helps them understand the material on a deeper level.  -->

<iframe width="560" height="315" src="https://www.youtube.com/embed/c-ZtRKAc3fY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Review and Further Practice

1. Compartmentalize your code into individual functions
1. Minimize redundancy: D.R.Y. up your code.
1. Write a unit test for words starting with multiple consonants: "create"
1. Build the functionality for this complexity.
1. Write a unit test for multiple words: "Pig Latin", "Jurassic Park"
1. Build the functionality for this new complexity.

<!-- ## Interview Questions (BlogPost_203)

*Every class will end with a discussion over these questions. If you have no idea about them, ask your instructor. Nevertheless, you will need to research the topics on your own and record what you learned in a blog, then link the url of the published blog into Campus Manager.*

1. Describe one thing you're learning in class today. -->
<!-- 
**¡Important!**

1. Remember, you will be graded for the completion of your blog but also this will be a place you can return to when preparing for interviews in a few months!
1. When publishing your blogs, make sure you tag "AustinCodingAcademy", "Coding", and "Web Development" in your story.  -->

******
******

# Instructor Notes

1. remind the students to merge their PRs.
1. create an assignment called " PigLatin "

## Go to [Pre-Homework >](02DayPrep.md)

{% include "../includes/footer.md" %}
