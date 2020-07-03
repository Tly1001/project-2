# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project #2: Reacathon

## Overview

The second project is to **build a React application** that consumes a **public API**.

### Technical Requirements

Your app must:

* **Consume a public API** – this could be anything but it must make sense for your project.
* **Have several components** - At least one classical and one functional.
* **The app can have a router** - with several "pages", this is up to your disgression and if it makes sense for your project.
* **Include wireframes** - that you designed before building the app.
* **Be deployed online** and accessible to the public.

---

### Dependancies
React-router-dom
Bulma
axios

## Necessary Deliverables

* A **working application**, hosted somewhere on the internet
* A **link to your hosted working app** in the URL section of your Github repo
* A **git repository hosted on Github**, with a link to your hosted project, and frequent commits dating back to the _very beginning_ of the project
* **A `readme.md` file** with:
  * Explanations of the **technologies** used
    * A couple of paragraphs about the **general approach you took**
    * **Installation instructions** for any dependencies
    * Link to your **wireframes** – sketches of major views / interfaces in your application
   * Descriptions of any **unsolved problems** or **major hurdles** your team had to overcome

---

## Walk-Through

### Hero Page

<img src="https://imgur.com/r71gXD8.jpg">

***Random dish page***
* ***Logo*** - takes you back to hero page
* ***Heart button*** - shows dish recipe
* ***Cross button*** - shows a new dish
* ***Corner cheeseburger*** - takes you to ingredient search

<img src="https://imgur.com/axNd9hd.jpg">

***Dish details***

<img src="https://imgur.com/hAnslLr.jpg">

<img src="https://imgur.com/vSNfDUJ.jpg">

<img src="https://imgur.com/VgOqxgG.jpg">

<img src="https://imgur.com/JqRcoCq.jpg">

<img src="https://imgur.com/UhDqLTa.jpg">

---

## Process

Before we started I created the overall wireframe for the pages built in Figma. For this project I wanted to give a clear outline of what the end product would be, so that the instructors would have a thorough grasp of what we were trying to achieve and to save time when it came to the styling phase.

With a design reference already in mind it was a lot easier than creating my own from scratch. 

<img src="https://imgur.com/Cm3pUA2.jpg">

Next was adding relationships to the pages, to further understand how each page would communicate with each other. 

<img src="https://imgur.com/qGgIl8q.jpg">



### Pages

Home Page - front end URL - '/'

DinderRandom - Front end URL - '/dinder'
             - Back end - GET RANDOM RECIPE

DinderMatch - Front end URL - '/dinder/:id
            - Back end URL - GET SINGLE RECIPE BY ID

Options - (navbar burger style with form on open) - This has Category option & main ingredient option which then filters the get random page by this data inputted by the user

Error - when a user navigates to an incorrect page

## Wins and Blockers

---

## Future Features

Log in page
Favourites page - for logged in user
Categories Drop-down
Animation for swiping

---

## Key Lessons Learnt




