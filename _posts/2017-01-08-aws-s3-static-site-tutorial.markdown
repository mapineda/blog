---
layout: post
title: "How To Host Static Site on AWS S3 - Tutorial"
subtitle: ''
date: 2017-01-08 09:07:00
author: 'Marco Pineda'
header-img: 'img/host-s3-bg.jpg'
---

<p>
AWS is the uncontested IAAS provider. Sure, there are other services like Azure, Google Cloud and VMware but none come close to matching Amazon's suit of services. I've studying up to take the AWS Certified Cloud Architect - Associate exam ( shout out to <a href='https://twitter.com/samkroon'>Sam Kroonenburg</a> and <a href='https://t.co/VbhlVUys1z'>acloud.guru</a> for an awesome course! ) and today I've learned how to host a static site using AWS S3. Tonight, I will pass on this knowledge on to you.
</p>

<p>
This tutorial assumes you have an AWS account (if not, create a free one, super easy) and that you know basic HTML.
Before we get into the tutorial, let's review why hosting on S3 is so wonderful. Skip this if you want to get to the tutorial.
</p>


  <h2>Why S3?</h2>
  <p>Several benefits to using S3 to host static websites. For example if you were hosting some big event and needed a landing page, S3 would be the place to do it. Below is a list of pros and cons to using S3.</p>

  <h4>Pros</h4>
  <ol>
    <li>Simple</li>
    <li>Scales Automatically</li>
    <li>Serverless</li>
    <li>Don't have to worry about load balancing</li>
  </ol>

  <h4>Cons</h4>
  <ol>
    <li>Static content only</li>
    <li>Can't do something server-side</li>
  </ol>

  <p>Let me reiterate that S3 is only for static content. This means no Dot Net, PHP etc. S3 is ideal for landing pages.</p>

  <!-- IMAGE OF S3 HERE -->
  <a href="#">
      <img src="{{ site.baseurl }}/img/s3-bg.png" alt="AWS S3 Image">
  </a>
  <span class="caption text-muted">S3. S3 is property of Amazon.</span>

  <h3>Le Grand Tutorial</h3>  
  <p>
  Alright, you've made it this far. Great! Let's get to it. This tutorial assumes you've already made a free AWS account. Go ahead and log in.  
  </p>


  <h3>Step 1</h3>
  <p>
  Once you're logged in to AWS Management Console, navigate to Services and Click on S3.
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/step1.png" alt="AWS S3 Image">
  </a>


  <h3>Step 2</h3>
  <p>
   Once in S3, go ahead and create a new bucket. Name the bucket, leave everything as default and click NEXT.
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/create-bucket.png" alt="AWS S3 Bucket Image">
  </a>


  <h3>Step 3</h3>
  <p>
  Click the bucket, go into properties and select "STATIC WEBSITE HOSTING", then choose "Use this bucket to host a website". Make the landing page "index.html" and the error page "error.html"
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/static-web-site-hosting.png" alt="AWS Static Site Hosting Image">
  </a>


  <h3>Step 4</h3>
  <p>
  Create an index.html page and error.html page in your favorite code editor. I'm using Atom.
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/index-example.png" alt="Atom Code Editor">
  </a>

  <h3>Step 5</h3>
  <p>
  Go back to S3 Bucket and go ahead and upload the files. Go ahead and hit next.
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/upload.png" alt="Upload AWS S3 Image">
  </a>


  <h3>Step 6</h3>
  <p>
   Go into your bucket, go to Permissions, Click on Everyone then tick the box that says Read to make your site public so Everyone can Read and see your site.
  </p>

  <a href="#">
      <img src="{{ site.baseurl }}/img/permissions.png" alt="Permissions AWS S3 Image">
  </a>

  <h3>Step 7</h3>
  <p>
  Go into properties, go to static site hosting and click on the AWS endpoint to take you to your newly hosted static site!
  </p>


  <p>Hope you enjoyed this tutorial, if you have any questions, feel free to tweet at me: <a href='https://twitter.com/marcoapineda13'>@marcoapineda13 </a></p>
