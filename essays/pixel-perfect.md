---
layout: essay
type: essay
title: "Pixel Perfect Design"
# All dates must be YYYY-MM-DD format!
date: 2024-02-22
published: true
labels:
  - Reflection
  - Frameworks
  - HTML
  - CSS
---

## Our Framework Floaties

**Splash!** You're thrown into the deep end of the pool and have no idea how to swim. What do you do? Probably splash and thrash your body around trying to get a grip on something to help keep you from sinking. Then, once you've gotten a hold of yourself, you hoist your body out and never step near a body of water again. Well, maybe you don't completely give up on swimming, but you get the point. Learning to swim for the first time can be a very scary experience, especially if you're thrown into the deep end. It's terrifying, and can sometimes have the inverse effect of making you want to stay away from bodies of water. That is why we have these wonderful tools called floaties. They provide a foundation for you to learn how to swim and float all on your own. But wait, why am I talking about swimming and floaties? What does any of this have to do with **"Pixel Perfect Design"**? Well, programmers have floaties too, and they are called frameworks.

Frameworks are a programmers tools that help keep us afloat amidst the languages and different syntax. They provide a structure and foundation to allow us to build entire websites and applications upon. However, they aren't as simple as throwing floaties on and instantly staying afloat. There is still some work to be done to be able to understand how to properly swim through the all the elements, classes, functions, etc.

I just started using my own framework floaties not too long ago for interactive web design, and I really appreciate the functionality that it provides. I began using HTML and CSS, and while it wasn't a horrible experience trying to design websites with the raw languages, it did leave a lot to be desired in terms of built-in classes. It was like a double-edged sword, where I had a lot of power to fully customize every aspect within my website, however I didn't know where to start due to the open-ended nature of raw HTML and CSS. Once I imported the Bootstrap 5 framework, however, and started to design with that wrapped around me, I realized how much easier it can be when there is some foundation to start with. Yes, using a framework such as Bootstrap still has you learning the nuances of it, but once you are able to grasp those you can really start to sail. It just takes a little commitment and investment of your time and effort, but that's just a small payoff to the results that you can produce once you've gotten a hang of it.

An example of a project that I worked on while using the Bootstrap 5 framework was the recreation of the Professional Korean ESports team [SK T1](https://www.t1.gg/) website. Below is a snippet of HTML code using Bootstrap 5 for the carousel of images on the website.

```js
<!--- Carousel --->
<div id="mainCarousel" class="carousel slide" data-ride="carousel">
  <!--- Wrapper --->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carouselContainer">
        <img class="d-block w-100" src="https://m.en.shop-t1.gg/_dj/img/GoalStudio_Mobile.jpg" alt="t1">
      </div>
    </div>

    <div class="carousel-item">
      <div class="carouselContainer">
      <img class="d-block w-100" src="https://pbs.twimg.com/media/E15ennrUYAYMQcR.jpg" alt="t1 hq">
      </div>
    </div>

    <div class="carousel-item">
      <div class="carouselContainer">
        <img class="d-block w-100" src="https://us-a.tapas.io/sa/b6/0c1d9f53-afde-4ae4-984f-8122c49257f8.jpg" style="height: 700px" alt="tapas">
      </div>
    </div>
  </div>

  <button class="carousel-control-prev" type="button" data-bs-target="#mainCarousel" data-bs-slide="prev">
    <i class="bi bi-arrow-left" style="font-size: 40px; margin-left: -90px" aria-hidden="true"></i>
      <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#mainCarousel" data-bs-slide="next">
    <i class="bi bi-arrow-right" style="font-size: 40px; margin-right:-90px" aria-hidden="true"></i>
    <span class="visually-hidden">Next</span>
  </button>
</div>
```
In the snippet above, almost every class assignment utilized Bootstrap's built-in carousel classes, which made life a whole lot simpler. Instead of trying to create my own classes to cycle through the content, I simply just pulled from the Bootstrap stylesheet. 

## Frameworks Walked So We Could Run

As I mentioned before, frameworks provide structure and foundation for programmers, and the example that I gave using Bootstrap 5 is only one type out of the sea of frameworks out there. In fact, the snippet of code is exactly that, just a snippet out of an entire website. The entire code is much longer, and Bootstrap has its footprints all over it. Without the foundation, it still would have been possible to fully implement the website, but I would not want to splash around trying to develop a beautiful and interactive website for all of you out there. 

A section of my recreation of the T1 website is shown below: 

<img class="img-fluid" src="../img/essay-img/t1.png" width="500" height="275" alt="Picture" style="display: block; margin: 0 auto" />
