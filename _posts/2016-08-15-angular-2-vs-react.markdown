---
layout: post
title: "Angular 2 vs React"
subtitle: ''
date: 2016-08-15 01:27:00
author: 'Marco Pineda'
header-img: 'img/arm-wrestling-bg.jpg'
---

<p>
Do a google search of 'javascript frameworks' and you get nearly 39MM results in .55 seconds. A top five search on Github lists these frameworks as the most popular in order from most popular to least:
</p>

  <ol>
    <li>Angular</li>
    <li>React</li>
    <li>Backbone</li>
    <li>Ember</li>
    <li>Polymer</li>  
  </ol>

  <p>
  This article takes an in depth look at the top two frameworks in the JavaScript development community, Angular 2 and React
  </p>

  <h2>Angular</h2>
  <p>
  Created in 2009 by Google, Angular is considered the most used JavaScript framework for developing Single Page Applications (SPA)
  Most recently, Angular 2 hit beta. I'll be comparing Angular 1 vs Angular 2 in another blog post coming soon. This post will compare Angular 2 vs React

  <strong>Disclaimer</strong>: Technically, yes, React is a library and Angular, a framework; however, they still aid in the MV* functionality of the web and such can be compared.

  </p>

  <!-- IMAGE OF ANGULAR HERE -->
  <a href="#">
      <img src="{{ site.baseurl }}/img/angular-bg.png" alt="Angular Image">
  </a>
  <span class="caption text-muted">Angular Logo. Angular is maintained by Google.</span>

  <h3>Features of Angular</h3>  
  <p>
  Angular 2 is all component and directive based. Controllers and $scope have been replaced. They have been replaced by components and directives. Components are directives with a template. A component is in HTML called with the <angularComponent> tag, the name of the selector within the HTML.
  </p>


  <h3>Consistency</h3>
  <p>
  Angular is a framework and provides significantly more opinions and functionality out of the box. With React, you usually pull a number of other libraries off the shelf to build an app. You’ll want libraries for routing, enforcing unidirectional flows, web API calls, testing, dependency management, and so on. The number of decisions is can be overwhelming.

  Angular offers more opinions out of the box, which helps you get started more quickly without feeling intimidated by decisions. This enforced consistency also helps new hires feel at home more quickly and makes switching developers between teams more practical.
  I admire how the Angular core team has embraced TypeScript, which leads to the next advantage…
  </p>

  <h3>TypeScript</h3>
  <p>
  This ties into the the section above on consistency. Angular 2 has taken a hard stance on which flavor of JavaScript to use. React examples are inconsistent and are presented in ES5 and ES6 and currently offers three different ways to declare components. This create mayhem for n00bs like myself. Angular also embraces decorators instead of extends.
  </p>

  <p>
  While Angular 2 does not require TypeScript, the Angular core team uses it as default in documentation. That means examples and projects and documentations are all consistent.  
  </p>

  <h2>Reduce Turnover</h2>
  <p>
  The Angular 2 of today has been carefully an methodically developed and reinvention of a mature, comprehensive framework. In React, it’s your responsibility to sift through a bunch of disparate, fast-moving, open-source libraries into a comprehensive whole that plays well together. It’s both time-consuming and frustrating.
  </p>

  <h2>ReactJS</h2>
  <p>
  Time to shine React.
  </p>

  <h3>JSX</h3>
  <p>
  JSX is an HTML-like syntax that compiles down to JavaScript. Markup and code are composed in the same file. This means code completion gives you a hand as you type references to your component’s functions and variables. In contrast, Angular’s string-based templates come with the usual downsides: No code coloring in many editors, limited code completion support, and run-time failures. You’d normally expect poor error messaging as well, but the Angular team created their own HTML parser to fix that. (Bravo!)

  </p>


  <!-- IMAGE OF REACT HERE -->
  <a href="#">
      <img src="{{ site.baseurl }}/img/react-bg.png" alt="React JS Image">
  </a>
  <span class="caption text-muted">React is a framework maintained by Facebook </span>


  <p>
  If you don’t like Angular string-based templates, you can move the templates to a separate file. Composing components in a single compile-time checked file is one of the big reasons JSX is so special.
  </p>

  <h3>Move Fast & Break Stuff</h3>
  <p>
  When you make a typo in React’s JSX, it won’t compile. This means you know immediately exactly which line has an error. React tells you immediately when you forget to close a tag or reference a property that doesn’t exist. In fact, the JSX compiler specifies the line number where the typo occurred. This behavior speeds development.
  </p>

  <p>
  In contrast, when you mistype a variable reference in Angular 2, nothing happens at all. Angular 2 fails quietly at run time instead of compile-time. It fails slowly. I load the app and wonder why my data is not displaying. Not fun.
  </p>

  <h3>Optimized for JavaScript</h3>
  <p>
  This is the fundamental difference between React and Angular. Unfortunately, Angular 2 remains HTML-centric rather than JavaScript-centric.
  </p>

  <p>
  Angular’s HTML-centric design remains its greatest weakness.
  </p>

  <p>
  JavaScript is far more powerful than HTML. Thus, it’s more logical to enhance JavaScript to support markup than to enhance HTML to support logic. HTML and JavaScript need to be glued together somehow, and React’s JavaScript-centric approach is fundamentally superior to Angular's HTML-centric approach.
  </p>

  <p>
  Angular 2 continues Angular 1’s approach of trying to make HTML more powerful. So you have to utilize Angular 2's unique syntax for simple tasks like looping and conditionals. For example, Angular 2 offers both one and two way binding via two syntaxes that are unfortunately quite different:
  </p>


  <h2>Tech Specs</h2>
  <p>
  Alright, let's get down to the nitty-gritty. The Tech Specs.
  </p>

  <ul>
    <li>Angular 2: 566k (766k with RxJS)</li>
    <li>Ember: 435k</li>
    <li>Angular 1: 143k</li>
    <li>React + Redux: 139k</li>
  </ul>

  <h2>IRL</h2>
  <p>
    Several popular websites are coded in Angular and React. Below is a breakdown of each.

    <ul>
      <li>List of <a href='https://github.com/facebook/react/wiki/Sites-Using-React'>React sites</a></li>
      <li>List of Angular sites <a href="https://www.madewithangular.com">Angular Sites</a></li>
    </ul>

  </p>



  <h2>Summary</h2>
  <p>
  Angular 2 is a huge improvement over version 1. The new component model is simpler to grasp than v1’s directives, it supports isomorphic/universal rendering, and it uses a virtual DOM offering 3–10x improvements in performance. These changes make Angular 2 very competitive with React. There’s no denying that its full-featured, opinionated nature offers some clear benefits by reducing “JavaScript fatigue”.
  </p>
  <p>
  Angular 2’s size and syntax is considerably bigger than React. Angular’s commitment to HTML-centric design makes it complex compared to React’s simpler JavaScript-centric model. In React, you don’t learn framework-specific HTML shims like ngWhatever.
  </p>
