# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) General Assembly Project #2: Dinder (Paired project)

<a href="https://dinder-for-recipes.netlify.app/">Deployed Link<a/>

The second project is to **build a React application** that consumes a **public API**.

### Technical Requirements

Brief:

* **Time given** - 36 Hours.
* **Consume a public API** – this could be anything but it must make sense for your project.
* **Have several components** - At least one classical and one functional.
* **The app can have a router** - with several "pages", this is up to your disgression and if it makes sense for your project.
* **Include wireframes** - that you designed before building the app.
* **Be deployed online** and accessible to the public.

---

## Concept

We decided to create food recipe app due to me and my partners' shared interest in cooking, with tinder in mind as a design inspiration.

## Functionality

* Browse random dishes
* Get the recipe of the dish they liked

## Technologies Used
* JSX
* CSS
* JavaScript
* React.JS
* React-router-dom
* Axios
* Bulma
* Insomnia
* Recipe API

---

## Walk-Through

### Hero Page

<img src="https://imgur.com/r71gXD8.jpg">

### Random dish page
* ***Logo*** - redirects back to hero page
* ***Heart button*** - shows dish recipe
* ***Cross button*** - shows a new dish
* ***Corner cheeseburger*** - directs to ingredient search

<img src="https://imgur.com/axNd9hd.jpg">

### Dish details
* ***Cross button*** - redirects to random dish page
* ***Star button*** - saves recipe to favourites(no functionality)

<img src="https://imgur.com/hAnslLr.jpg">

### Ingredient search instructions

<img src="https://imgur.com/vSNfDUJ.jpg">

### Ingredient search

<img src="https://imgur.com/VgOqxgG.jpg">

### Random search with ingredient

<img src="https://imgur.com/JqRcoCq.jpg">

### Ingredient search recipe

<img src="https://imgur.com/UhDqLTa.jpg">

---

## Wireframe

<a href="https://www.figma.com/file/Y1gbyc00bHPZqZpkZwb8Jd/Dinder?node-id=0%3A1">Figma link<a/>

Before we started I created the overall wireframe for the pages built in ***Figma***. For this project I wanted to give a clear outline of what the end product would be, so that the instructors would have a thorough grasp of what we were trying to achieve and to save time when it came to the styling phase.

With a design reference already in mind it was a lot easier than creating my own from scratch. 

<img src="https://imgur.com/Cm3pUA2.jpg">

Next was adding relationships to the pages, to further understand how each page would communicate with each other. 

<img src="https://imgur.com/qGgIl8q.jpg">

## Process

1. We first started with me building the JSX of the random dish and recipe pages, whilst my partner worked on the get requests to the recipe API using a REST framework.

2. From there I worked on extracting the data of the get requests for the created pages to be displayed, my partner moved onto styling with bulma in mind.

3. At this point we were at MVP so I began working on the Hero page and promptly into joining my partner in styling the rest.

4. We had about 5 hours of time left so we commited to working on one of our 'nice to haves' which was an ingredient search option.

5. The last 2 hours were spent cleaning up code, final finishing touches for styling, and making small aninimation features for the home screen and buttons.

---

## Featured code

### Ingredient/Measurement Listing

This code I was particularly proud of because it put our progress to a halt trying to extract the data from the GET request and display it the way we wanted on the page. The ingredients and measurements were in 2 separate arrays which at first we thought of a very untidy way of doing so (explained in the wins and blockers section). This essentially extracts from 2 arrays, concatenates the respective items and places them into a new array.

```
const ingredientsList = []
    const getIngredientsList = () => {
      const ingredients = []
      const measures = []
      const array = Object.entries(this.state.meals.meals[0])
      
      array.map(key => {
        if (key[0].search('Ingredient') > 0 && key[1]) {
          ingredients.push(`${key[1]}`)
        }
        
        if (key[0].search('Measure') > 0 && key[1]) {
          measures.push(`${key[1]}`)
        }
      })
      
      for (let i = 0; i < ingredients.length - 1; i++) {
        if (ingredients[i]) {
          ingredientsList.push(`${ingredients[i]}: ${measures[i]}`)
        }
      }
    }
```



## Wins and Blockers

The worst blocker we came across was once the recipes were fetched, extracting the array of ingredients and concatenating them with their respective measurements which was also in their own array became an issue. Due to the time constraint we eventually had to bite the bullet and hard code 40 separate variables (20 for ingredients, 20 for measurements) which I then looped through to show on the page. At the end I luckily had time to clean it up, removed the variables; replacing it with a map function which felt a lot less reptitive.

Another issue that we came across was when the ingredient search cheeseburger was clicked whilst already in an ingredient search, the modal would not appear for it. This took quite some time to debug but I managed to solve this by adding a ternary statement that would check the url, which would then refresh the page if it was currently on the ingredient search page.

A big win was how nice we got the pages to look, especially the recipe show pages on both desktop and mobile devices. This was my first time pair coding and was definitely a big learning experience which I was fully appreciative of.

---

## Future Features

* Register/Log in page
* Favourites page - for logged in user
* Categories Drop-down
* Animation for swiping

---

## Key Lessons Learnt

The biggest lesson I learned is the importance of communication with your team. Being my first pair coding project we stumbled at first due to differences in coding style and thought process, but quickly landed on our feet and managed to pull off a big win in my books. I learned to not focus too much on clean code in the initial phase, but to get a working product first, then once everything is done to go back and do so.

This was also a project for us to practice React.JS and GET requests which we had been learning over 4 days, which I felt a lot more confident with using having completed this project.




