# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

So this project was a challenge to recreate a QR code component as closely as possible to the original.

### Screenshot

![My Screenshot of the QR Component Project](./Screenshot%202023-02-04%20at%2017-13-56%20Frontend%20Mentor%20QR%20code%20component.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

First I structured the project with HTML. Going by the font sizes, I went with and h1 and p and wrote what was on the design.

For styling, I decided to tackle this with a top-down approach. I started with the background. Then for the white box, I figured it was best to approach it as a div. Since the QR code was already in the starter pack, I just uploaded the image into the HTML.index file that accompanied it.

There was a style guide in the starter pack, so I followed the color schemes therein that aligned with each part of the design. I also made sure to follow the mentioned font sizes and styles.

### Built with

I didn't use any special frameworks or tools, just plain HTML and CSS. I used Visual Studio Code as my editor. I also used GitHub for desktop.

### What I learned

I had a bit of a brain-fart when setting up the background color. I kept using the universal selector to style it (though I knew deep down it wasn't the right one.) Luckily, I had a little help from my sister who reminded me it was the body tag I should be selecting. Thanks sis!

Though I was able to center my element, I realized upon looking at the design that it had to be vertically and horizontally centered. I learned there's more than one way to horizontally and vertically center an element(and center one in general). I've tried all the ones I've found and the position and transform: translate method got me the closest to the look of the original design. I also used border-box sizing for a cleaner look.

The thing was that after I've done that, the attribution that was already set up and position on the bottom center in the project HTML file, went in the opposite direction, up top. I tried to fix it, but instead changed the position to absolute. Personally, I liked it so I kept it.

I used a div for the white box and gave it an id (simply named #white-box). At first I tried to style it with the id, but as I was looking for ways to center it, the examples I saw used a class selector. So I went that route and named it .white-box). Which makes sense since an id is unique to the element it's used on.

There was a lot of commenting out and trying different sets of code, so I wouldn't lose anything in case I want to reuse or return to previous lines later. So I guess I've learned the value of comments!

I'm also getting the hang of importing Google Fonts onto the stylesheet.

I also noticed that while my favicon worked on Firefox, it didn't show up on Chrome. I looked for solutions as to why that is and at first thought it was a cache issue. But then I learned that Chrome doesn't show locally stored images, and that it has to be uploaded to the server. Apparently that's not the case with Firefox.

Here's the css I used to center:

```css
.white-box{
    background: hsl(0, 0%, 100%);
        font: 15px 'Outfit', sans-serif;
        text-align: center;
        border-radius: 20px;
    padding: 15px;
    width: 350px;
    position: relative;
    box-sizing: border-box;
}

.white-box{
    margin: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
```

I think, more than anything, I've learned a little about letting go of perfectionism. As I became frustrated about my result not looking exactly like the original, I forgot what the instrctions were: to get as close to the original as possible. If what I had was the best I could do, then so be it.

### Continued development

I want to learn how to better present elements and to get more familiar with Flexbox. I'm still trying to learn it, and it was one of the methods I used in my attempts to position the div, so I'd like to familiarize myself with it more.

### Useful resources

- [w3Schools](https://www.w3schools.com/css/css_align.asp) - This was one of the pages that helped me understand how to align elements various ways with various methods. It provided examples of each situation, especially on vertical and horizontal centering. It also helped with centering the image.

- [FreeCodeCamp](https://www.freecodecamp.org/news/how-to-center-anything-with-css-align-a-div-text-and-more/) - This article was another resource I used to learn specifically how to center an element. This also helped me with centering vertically and horizontally.

## Author

- Frontend Mentor - [@jwashingtondev](https://www.frontendmentor.io/profile/jwashingtondev)
- GitHub - [jwashingtondev](https://github.com/jwashingtondev)
