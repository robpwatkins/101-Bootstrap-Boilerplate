# 101-Bootstrap-Boilerplate

## Checklist

* Overview
* Get Ready for Bootstrap
* Reboot
* Add a Nav Menu
* Grid Layout
* Buttons!
* Suggested Viewing
* Know Your Docs
* Terms to Know
* Questions for Student Discussion

### Purpose

These instructions are taken from the textbook for you to easily view them here as well as learn Markdown language, if you like!

#### Get Ready for Bootstrap

The steps we take in this section will mirror the [Getting Started Docs @getbootstrap.com](https://getbootstrap.com/docs/4.4/getting-started/introduction/).

First, link the CDN to your web page:

|HTML Link Bootstrap's CDN in the `<head>` of your page|
|---|

```html
  <head>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
  </head>  
```

Now we have to bring in the JavaScript and another JS library called jQuery that runs alongside the components we're going to build. Put these links at the bottom of your `body` element:

|HTML Link Bootstrap's JS CDN at the bottom of the `<body>` element|
|---|

```html
  <body>
    <!-- Your other code will go here -->
    <!-- ... -->





    <!-- and above here -->
    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
  </body>
```

Now you're ready to begin building!!!

#### Reboot

Remember when we added a CSS reset to our bank of knowledge? The reason for that was to create a blank slate for our other styles to be added. Turns out, Bootstrap has its own form of CSS reset called Reboot. You don't have to do anything special to get it to work. Once you've linked the CSS CDN at the top of your page it works.

Try it! Create an `h1`. See the different font? There's plenty more but we have a lot to get to so if you're curious come back later to the [Reboot page](https://getbootstrap.com/docs/4.4/content/reboot/) to learn more.

#### Add a Nav Menu

Go to the [Components page](https://getbootstrap.com/docs/4.4/components/alerts/) and scroll down to [Navs](https://getbootstrap.com/docs/4.4/components/navs/).

Here you can see there are pre-built navigation menus you can use. All of them are 100% customizable but the benefit you have here is that you didn't have to build it all from scratch. So scroll down until you see: "Horizontal alignment".

![bootstrap-nav-screenshot](../images/bootstrap-nav-screenshot.png)
Notice the example and the code snippet below it? You can just click the copy button and paste it into the `body` of your HTML file then see what happens in live-server!!

Try it!!

Now replace `justify-content-center` with `justify-content-end`. Do you see that? We can change the entire layout with a simple change of class names!!

#### Grid Layout

Speaking of layout...since you know display flex this should be very easy for you. To lay out a page or a section all you'll need to do is create a `div` container element with the class name `container-fluid`.

|HTML Grid Container Element|
|---|

```html
<div class=".container-fluid">
<!-- to create a row for items create another container element with the class name: "row" -->
  <div class="row">
  <!-- inside any row you have 12 columns for items to be arranged on. -->
  <!-- These three elements will each take up 4 columns to fill up the screen -->
    <div class="col-sm">
      first column
    </div>
    <div class="col-sm">
      second column
    </div>
    <div class="col-sm">
      third column
    </div>
  </div>
</div>
```

Try it! Paste it underneath your nav menu and see what happens!

When you do this, the [row elements will have 12 columns](https://getbootstrap.com/docs/4.4/layout/grid/) added to them automatically. (*They use display: flex to do this.*) So if you put three items inside, each element will take up 4 columns. Only 2 items? Each will take up 6 columns. But you can change that by giving it the number of columns it should take up with...you guessed it...a class name!!

```html
<div class="col"></div>
<div class="col-8"></div>
<div class="col"></div>
```

In the example above the first and last `div` will only have 4 columns to divide themselves into because the second `div` is set to take up the middle 8 columns.

#### Buttons!

Buttons are incredibly useful to have on hand and Bootstrap does a wonderful job at creating many of them!! Go to the [Buttons page](https://getbootstrap.com/docs/4.4/components/buttons/) and read up. You can change nearly anything you want by just changing class names so throw a few buttons in a new "row" and see what you can create!!

Have fun! Play! This is the way you truly deepen your understanding.

### Wrap-Up

Bootstrap is an incredibly useful tool to jump start your app or website. You can use this technology for your 101 final project but you don't have to feel obligated! We really just want for you to have all the options available to you, give you a solid road map, and a fundamental understanding so you can navigate, discover, and become your own developer!!

Have fun and keep coding!

*****
*****

### Suggested Viewing

> *NOTE: the video from BlondieBytes below is on an older version of Bootstrap but the basics are still the same.*

* [BlondieBytes on Bootstrap v3](https://www.youtube.com/watch?v=yalxT0PEx8c)
* [Academind on Boostrap v4](https://www.youtube.com/watch?v=7g8Gg2QVdeU)

### Know Your Docs

Obviously [Bootstrap](https://getbootstrap.com/docs/4.4/getting-started/introduction/).

## Terms to Know

* Bootstrapping

## Questions for Student Discussion

1. Why would we use Bootstrap?
1. What advantages do you see to working with Bootstrap?
1. Why is responsive design so important?
1. What's the first step to building a website? What's after that? When does Bootstrap come in that sequence?
