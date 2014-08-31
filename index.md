---
layout: default
title: Welcome
---

# {{ page.title }}

<div class="toc" markdown="1">
Contents:

* [What's S5? What's S6?](#whatis)
* [S6 in Action - Sample Slide Shows Online](#demos)
* [Templates](#templates)
    * [Classic](#classic)
    * [Modern](#modern)
* [Bonus: What's Slide Show (S9)? Slide Show Generator for S6](#s9)
* [About, License - Questions? Comments?](#about)
</div>


Slide Show Templates Using HTML5, CSS3 'n' JavaScript

## What's S5? What's S6?  {#whatis}

Simple Standards-based Slide Show System (S5) is Eric Meyer's (of CSS fame) public domain
(free, open source) slide show package inspired by Opera Show and others that works
in all modern browsers without any plugin required
because it includes its own slide show machinery in JavaScript.
More [S5 Project Site »](http://meyerweb.com/eric/tools/s5)

S6 started as a rewrite of S5 using the jQuery JavaScript library - offering
easier to understand and easier to extend code. Add plugins, effects and more.
Contributions welcome!

## S6 in Action - Sample Slide Shows Online  {#demos}

Try some slide show samples powered by S6:

- [Slide Show (S9) 10-Minute Tutorial](http://slideshow-s9.github.io/demos/tutorial.html)
- [Prototype vs jQuery: To and from JavaScript Libraries](http://slideshow-s9.github.io/demos/jquery.html)
- [10 Things Every Java Programmer Should Know About Ruby](http://slideshow-s9.github.io/demos/10things.html)
- [Ruby 1.9: What to Expect](http://slideshow-s9.github.io/demos/ruby19.html)
- [`beer.db` - Using Open Beer & Brewery Data in Ruby](http://slideshow-s9.github.io/demos/beer_db_intro.html)
- [`football.db` - Using Open Football Data - Get Ready for the World Cup in Brazil 2014](http://slideshow-s9.github.io/demos/open_data_world_cup_with_js.html)
- [Using Markdown for Websites, Presentations, or Books](http://slideshow-s9.github.io/demos/markdown.html)
- [Building Your Own Web Components (Tags / Elements)](http://slideshow-s9.github.io/demos/webcomponents2.html)

Keyboard controls:

| Action                                             | Key                                                         |
| -------------------------------------------------- | ----------------------------------------------------------- |
| Go to next slide                                   | Space Bar, Right Arrow Down Arrow, Page Down, Click Heading |
| Go to previous slide                               | Left Arrow, Up Arrow, Page Up                               |
| Go to first slide                                  | Home                                                        |
| Go to last slide                                   | End                                                         |
| Toggle between slideshow and outline view (Ø)      | T                                                           |
| Show/hide slide controls (Ø « »)                   | C, Move mouse to bottom right corner                        |


## Templates  {#templates}

### Classic {#classic}

~~~
 <div class='slide cover'>
    <h1>Your Slide Title Here</h1>
    <ul>
      <li>Item One Here</li>
      <li>Item Two Here</li>
    </ul>
  </div>

  <div class='slide'>
    <h1>Steps Demos</h1>

    <!-- mark list with class step to mark all items at once -->
    <ul class='step'>
      <li>Item 1.1 Here</li>
      <li>Item 1.2 Here</li>
    </ul>

    <!-- or mark individual list items -->
    <ul>
      <li class='step'>Item 2.1 Here</li>
      <li class='step'>Item 2.2 Here</li>
    </ul>

    <!-- or mark paragraphs, div blocks or whatever -->
    <p class='step'>Another Step</p>

  </div>

  <div class='slide'>
    <h1>Another Slide Title Here</h1>
    <p>yada yada yada</p>
  </div>

  <!-- h1.fullscreen => uses only centered heading with no content/body -->
  <div class='slide'>
    <h1 class='fullscreen'>Another Slide - Using Fullscreen Heading</h1>
  </div>
~~~

### Modern  {#modern}

~~~
    <section class='slides'>
      <!-- Add your slides here. Delete or comment out the slides below. -->
      
      <article class='cover'>
        <h1>
          Title Goes Here Up
          <br>
          To Two Lines
        </h1>
        <p>
          Carlos Ruby
          <br>
          November 11, 2020
        </p>
      </article>
      
      <article>
        <h3>
          Simple slide with header and text
        </h3>
        <p>
          This is a slide with just text. This is a slide with just text.
          This is a slide with just text. This is a slide with just text.
        </p>
        <p>
          There is more text just underneath with a <code>code sample: 5px</code>.
        </p>
      </article>

      <article>
        <h3>
          Slide with bullet points that builds
        </h3>
        <ul class="build">
          <li>
            This is an example of a list
          </li>
          <li>
            The list items fade in
          </li>
          <li>
            Last one!
          </li>
        </ul>

        <div class="build">
          <p>Any element with child nodes can build.</p>
          <p>It doesn't have to be a list.</p>
        </div>
      </article>

      <article>
        <h3>
          Slide with an image
        </h3>
        <p>
          <img style='height: 500px' src='images/example-graph.png'>
        </p>
        <div class='source'>
          Source: Carlos Ruby
        </div>
      </article>

      <article class='fill'>
        <h3>
          Image filling the slide (with optional header)
        </h3>
        <p>
          <img src='images/example-cat.jpg'>
        </p>
        <div class='source white'>
          Source: Carlos Ruby
        </div>
      </article>
      
      <article class='nobackground'>
        <h3>
          A slide with an embed + title
        </h3>
        
        <iframe src='http://slideshow-s9.github.io'></iframe>
      </article>

      <article class='slide nobackground'>
        <iframe src='http://slideshow-s9.github.io'></iframe>
      </article>

      <article class='fill'>
        <h3>
          Full-slide embed with (optional) slide title on top
        </h3>
        <iframe src='http://slideshow-s9.github.io'></iframe>
      </article>
      
    </section>
~~~



## Bonus: What's Slide Show (S9)? Slide Show Generator for S6   {#s9}

A Ruby gem that lets you create slide shows and author slides in plain text
using a wiki-style markup language that's easy-to-write and easy-to-read
and ships "out-of-the-gem" with S6 templates built-in.
More [Slide Show (S9) Project Site »](http://slideshow-s9.github.io)


## About, License   {#about}

The slide show (S6) scripts and templates are dedicated
to the public domain. Use it as you please with no restrictions whatsoever.


{% include questions.md %}
