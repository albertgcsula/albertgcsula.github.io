---
layout: post
title:  "Bootstrap Tutorial"
date:   2014-07-21 12:00:00
categories: projects, tutorials
---

This tutorial will show how to create a simple bootstrap boilerplate and implement some simple and some of the most common Bootstrap components.

To start off, what is Bootstrap? <br />
<a href="http://getbootstrap.com/" target="_blank">Bootstrap</a> is a front-end framework for faster and easier web development. Basically a collection of tools (CSS, JavaScript and markup structure) for creating websites.

How do you use Bootstrap? <br />
You can simply download the tools Bootstrap provides from their <a href="http://getbootstrap.com/" target="_blank">website</a>, or access them through a CDN.

Here is a really simple Bootstrap starter template.

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap Starter Template</title>
    <!-- Bootstrap -->
    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="http://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css">
  </head>
  <body>
    <div class="jumbotron">
      <h1>Hello, world!</h1>
      <p>This is super simple bootstrap starter template.</p>
    </div>

    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
    <!-- Latest compiled and minified JavaScript -->
    <script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/js/bootstrap.min.js"></script>
  </body>
</html>
{% endhighlight %}

That's it, you are not able to start using all of the tools bootstrap has to offer.

In this turorial we are going to build a page consisting of some of the commonly used compoments of Bootstrap. It looks like this:

<img class="img-responsive" src="{{ site.url }}/img/demo.jpg">

The goal is to build this page using Bootstrap components and make it fully responsive.

You can view all of the markup for the demo page <a href="http://www.albertgu.com/projects/bootstrap-starter/" target="blank">here</a>.

The first portion of the page uses a component of Bootstrap that is widely used and quite easy to implement. It is the <a href="http://getbootstrap.com/components/#jumbotron" target="_blank">Jumbotron</a> component. The markup for this section of the page is really straight forward, it's the same code from the boiler plate, you can change the appearance of the Jumbotron easily with CSS.

{% highlight html %}
<div class="jumbotron">
  <h1>Style is Everything</h1>
  <p>Find yours at Burlington and save up to 60% off department store prices everyday.</p>
</div>
{% endhighlight %}

The next section of the page is another popular component which has been greatly simplified with the use of Bootstrap, the <a href="http://getbootstrap.com/javascript/#carousel" target="_blank">Carousel</a>. With not too many lines of markup you can implement a simple Carousel slider in a plug and play fashion.

{% highlight html %}
<div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
  <!-- Indicators -->
  <ol class="carousel-indicators">
    <li data-target="#carousel-example-generic" data-slide-to="0"></li>
    <li data-target="#carousel-example-generic" data-slide-to="1"></li>
    <li data-target="#carousel-example-generic" data-slide-to="2"></li>
  </ol>
  <!-- Wrapper for slides -->
  <div class="carousel-inner">
    <div class="item active">
      <img src="img/slide1.jpg" alt="...">
    </div>
    <div class="item">
      <img src="img/slide2.jpg" alt="...">
    </div>
    <div class="item">
      <img src="img/slide3.jpg" alt="...">
    </div>
  </div>
  <!-- Controls -->
  <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left"></span>
  </a>
  <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right"></span>
  </a>
</div>
{% endhighlight %}

That's it, you now have a simple slider in which you can place the content you desire.

For the last section of the page we will use another very useful Bootstrap componenet, the <a href="http://getbootstrap.com/css/#grid" target="_blank">Grid System</a>. Grid systems are used for creating page layouts through a series of rows and columns that house your content. For this page we will use a grid system that starts out stacked on mobile devices and tablet devices (the extra small to small range) before becoming horizontal on desktop (medium) devices. Mess around with the different grid options to see how the layout changes on both mobile and desktop.

{% highlight html %}
<div id="bur-grid">
  <!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
  <div class="row">
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid1.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid2.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid3.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid4.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid5.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
    <div class="col-md-4">
      <div class="bur-thumbnail">
        <a href="#">
          <img class="burimg img-responsive" src="img/grid6.jpg" alt="...">
          <span class="icon-wrap"></span>
        </a>
      </div>
    </div>
  </div>
</div>
{% endhighlight %}

Be sure to read through all the links provided for each component to get a more complete and thorough explanation and to explore the components more.

You can download all of the files for the demo page <a href="http://www.albertgu.com/projects/bootstrap-starter/bootstrap-starter.zip">here</a>.
