---
layout: post
title: "Basics of Computer Vision & OpenCV"
subtitle: ''
date: 2017-06-24 08:07:00
author: 'Marco Pineda'
header-img: 'img/computer-vision.jpg'
---

  <p>
  This post covers the basics of Computer Vision and Open CV.
  <p>

  <h2>Topics Covered:</h2>
    <ul>
      <li>What are Images?</li>
      <li>How Images Are Formed.</li>
      <li>Storing Images on Computers</li>
      <li>Getting Started with OpenCV: reading, writing, displaying images</li>
      <li>Grayscaling</li>
      <li>Color Spaces</li>
      <li>Histograms</li>
      <li>Drawing Images</li>
    </ul>

    <h1>Getting Started:</h1>
    <hr>

      <h2>What Are Images?</h2>
        <ul>
          <li>2-Dimensional representations of the visible light spectrum.</li>
        </ul>

        <p>Examples:</p>
          <ul>
            <li>photographs</li>
            <li>picture on laptop screen</li>
          </ul>

      <h3>Vocabulary:</h3>
      <ul>
        <li>DPI - Dots Per Image</li>
        <li>Visible Light Spectrum - wavelengths of light human eyes can detect</li>
      </ul>

<hr>

      <h2>How are Images Formed??</h2>
        <ul>
          <li>Images are formed when light hits an object, relects off the object onto a film, sensor or retina.</li>
        </ul>

        <p>To optimize images, we use a small opening called an aperature to block off excess light and focus the image; reducing blur. We can also use lenses to control the image formation.</p>

        <h3>Lenses</h3>
        <p>Both our eyes and cameras use an adaptive lens to control many aspects of the image formation such as:</p>

        <p>Aperature Size</p>
          <ul>
            <li>Controls the amount of light allowed through (f-stops in cameras)</li>
            <li>Depth of field(Bokeh)</li>
          </ul>

        <p>Length Width</p>
          <ul>
            <li>Adjust focus distance (near or far)</li>
          </ul>

        <h3>How Humans See</h3>
        <p>Both our eyes and cameras use an adaptive lens to control many aspects of the image formation such as:</p>

        <p>Aperature Size</p>
          <ul>
            <li>Controls the amount of light allowed through (f-stops in cameras)</li>
            <li>Depth of field(Bokeh)</li>
          </ul>

        <p>Length Width</p>
          <ul>
            <li>Adjust focus distance (near or far)</li>
          </ul>

        <h3>How Computers See - OpenCV</h3>
        <p>OpenCV uses RGB (Red, Green, Blue) color space by default.</p>

        <p>Each pixel(x,y) in an image has 3 values ranging in 0 - 255(8-bit)</p>

        <p>Those values are:</p>
        <ul>
          <li>Red</li>
          <li>Green</li>
          <li>Blue</li>
        </ul>

        <p>Mixing different color intensities of each color gives us the full color spectrum, example Yellow:</p>
        <ul>
          <li>Red - 255</li>
          <li>Green - 255 </li>
          <li>Blue - 0 </li>
        </ul>

        <p>Length Width</p>
          <ul>
            <li>Adjust focus distance (near or far)</li>
          </ul>

<hr>
    <h2>How A Computer Stores Images</h2>

    <p>Images are stored in multi-dimensional arrays</p>

    <p>Think of an array as a table.</p>
    <label>1-Dimensional Table</label>

    <table>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
    </table>


    <h3>Black, White or Grayscale</h3>

    <p>Black and white image, images are saved in a 2-Dimensional array.</p>

    <p>Two types of B&W images</p>
    <ul>
      <li>Grayscale - ranges in shades of gray</li>
      <li>Binary - pixels are either black or white</li>
    </ul>
<hr>

  <h2>Getting Started With OpenCV</h2>

    <h3>What is OpenCV?</h3>
      <ul>
        <li>OpenCV = Open Computer Vision</li>
        <li>Launched in 1999 by Intel</li>
        <li>Written in C++</li>
        <li>1st major release in 2006, second in 2009 and third in 2015</li>
        <li>Latest stable version is OpeCV 2.4.13</li>
      </ul>

    <h3>Get Started - Reading, Writing & Displaying Images:</h3>
    <p>See tutorial on reading, writing and displaying images using OpenCV</p>
<hr>

  <h2>Grayscaling</h2>

    <h3>Why Grayscaling?</h3>
    <p>In OpenCV, many functions grayscale images before processing. This is done to simplify the image to reduce noise and increase processing time as there is less information in the image.</p>

    <h3>What is Grayscaling?</h3>
    <p>Converting an image from full color to shades of gray (black & white).</p>

    <h3>Getting Started: Grayscaling Tutorial </h3>
    <p>See tutorial on Grayscaling using OpenCV</p>
    <p>In the tutorial you will learn:</p>
    <ul>
      <li>How to convert color image to grayscale</li>
    </ul>

<pre>
#import packages
import cv2
import numpy as np

#read image using cv2.imread()
input = cv2.imread('./images/input.jpg', 0)

#output to grayscale using cv2.imshow()
cv2.imshow('Grayscale', input)
cv2.waitKey(0)
cv2.destroyAllWindows()
</pre>

<hr>
  <h2>Color Spaces</h2>

    <h3>What are Color Spaces?</h3>
    <p>Color spaces are a way to represent color.</p>

    <p>The most common terms to represent color:</p>
    <ul>
      <li>RGB - Red, Gree, Blue</li>
      <li>HSV - Hue, Saturation, Value</li>
      <li>CMYK - Cyan, Magenta, Yellow, Black(K)</li>
    </ul>

    <h3>Getting Started: Color Spaces Tutorial </h3>
    <p>See tutorial on Color Spaces using OpenCV</p>

<hr>

  <h2>Histograms</h2>

    <h3>Why Histograms?</h3>
    <p>Great way to visualize individual color components.</p>

    <h3>Getting Started: Histogram Tutorial </h3>
    <p>See tutorial on Histograms using OpenCV</p>

<hr>
  <h2>Drawing Images</h2>

    <h3>Getting Started: Drawing Tutorial </h3>
    <p>See tutorial on Drawing Images using OpenCV</p>

<hr>
