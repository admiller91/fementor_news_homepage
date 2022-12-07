# Frontend Mentor - News homepage solution

This is a solution to the [News homepage challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://github.com/admiller91/fementor_news_homepage)

## My process

### Built with

- HTML5
- CSS
- Flexbox


### What I learned

I learned that even though I thought I was good at building a responsive site from just a design, I need more hands on work to get more comfortable.

I knew about the box-sizing issue but this was the first time I encountered problems with it. At a smaller screen size the "New" section of the site was creating a horizontal scroll. I discovered this was because I had the width set to 100% so it would stretch the entire container while also  having a padding set to add space between the section and the text. The size + padding added up to over 100% of the width which caused the issue. Giving the global style of box-sizing:border-box fixed the issue.

```css
* {
    box-sizing: border-box;
  }
```
One of the challenging parts of this challenge was the mobile menu. Its something Ive never had to do. I knew i could find hundreds of tutorials online about how to do this but instead I wanted to do this on my own. I was able to break down the problem into multiple acheivable steps. I started by just creating a new container for the menu and adding the list. I struggled to get the zindex and positioning right but was able to come up with a solution. Once the zindex was right I focused on getting it aligned to the right and the padding to match the design. To align it to the right i had to add another container div to the markup so the width could be 100% and then I could set only the menu part to the right.

### Continued development

The plan is to continue working on my HTML and CSS skills by doing more Frontend Mentor challenges. These are good challenges to get hands on in creating responsive websites from just a design file.

Specifically, I need to learn more about when to use the correct units (px vs em vs rem vs %) and how to create the right amount of spacing between different sections of the website. For example, originally I set a fixed padding to the container div and used media queries to change it as needed. Eventuall I changed it to a percentage so regardless of screen size, the padding looked okay. Im sure there are other areas where I can optimize my methods.

I also plan on doing more Javascript challenges so I can get more comfortable with the language.

