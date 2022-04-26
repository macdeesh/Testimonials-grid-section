# Testimonials-grid-section
Frontend Mentor Project

This is a solution to the [Testimonials grid section Challenge](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). 

## Links

- Solution URL: [https://github.com/macdeesh/Testimonials-grid-section]
- Live Site URL: [https://macdeesh.github.io/Testimonials-grid-section/]

## Screenshot

![](./ScreenShot.png)
   
## What I learned 

- To create the grid with different size cards I used ```grid-template-areas``` with ```grid-template-columns```, ```grid-template-rows``` and 
```max-width``` and used the names of the areas in the specefic class styling ```grid-area: side;``` or  ````grid-area: white-card;``` :

```css
.card-container {
    display: grid;
    justify-content: center;
    gap: 1.5rem;
    max-width: 996px;
    margin-bottom: 1rem;
    line-height: 1.4;
    grid-template-areas: "violet-card violet-card grayish-card side"
        "white-card blackish-card blackish-card side";
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: auto;
 }
 
 .white-card {
    background-color: var(--White-color);
    grid-area: white-card;
    color: var(--Dark-grayish-blue);
}
````

- I changed the height of the body to ```min-height: 100vh;``` instead of ```height: 100vh;``` because the viewport doesn't fit the size of the grid when I shrink the window in the y-axis (up and down).

- I used ```<blockquote>``` to wrap the two paragraphs of quotes instead of ```<div>```, but that makes the height of the cards change, by adding a big white-space or margin below the paragraph, so kept using ```<div>``` to avoid the mess. The solution to fix this problem is including a css reset at the start of my stylesheet. Next time I will use ```<blockquote>``` without any problem.
   
## Author

 - Github - [Macdeesh](https://github.com/macdeesh)
 - Twitter - [@Macdiish](https://twitter.com/Macdiish)
