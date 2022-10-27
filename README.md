# The Ignored Bits In Frontend Web Development

## Table Of Contents

- [The Ignored Bits In Frontend Web Development](#the-ignored-bits-in-frontend-web-development)
  * [Part One : The Web Browser Engine.](#part-one---the-web-browser-engine)
    + [Introduction To Browser Internals](#introduction-to-browser-internals)
      - [Web Browsers Engines](#web-browsers-engines)
      - [Webkit](#webkit)
      - [Blink.](#blink)
      - [Gecko](#gecko)
      - [How web browsers work](#how-web-browsers-work)
    + [Measuring Web Performance In Browsers](#measuring-web-performance-in-browsers)
      - [Core Metrics](#core-metrics)
        * [LCP](#lcp)
        * [FCP](#fcp)
        * [TTI](#tti)
        * [TBT](#tbt)
        * [FID](#fid)
        * [MPFID](#mpfid)
        * [CLS](#cls)
        * [FCI](#fci)
    + [Browser Components](#browser-components)
      - [Network](#network)
        * [Latency and Bandwidth (Perceived Speed)](#latency-and-bandwidth--perceived-speed-)
        * [TCP](#tcp)
        * [UDP](#udp)
        * [TLS](#tls)
        * [Wifi and Mobile Networks](#wifi-and-mobile-networks)
        * [HTTP(1, 1.2, 2, 3)](#http-1--12--2--3-)
        * [Real Time](#real-time)
      - [Storage](#storage)
        * [Cookies.](#cookies)
        * [Local storage.](#local-storage)
        * [Session storage.](#session-storage)
        * [IndexedDB.](#indexeddb)
        * [Web SQL.(deprecated)](#web-sql-deprecated-)
        * [Cache storage](#cache-storage)
      - [Parsing](#parsing)
      - [Rendering](#rendering)
      - [Scripting](#scripting)
  * [Part Two: Performance and Optimization.](#part-two--performance-and-optimization)
    + [HTML](#html)
    + [CSS](#css)
    + [JavaScript](#javascript)
    + [Images](#images)
    + [Video](#video)
  * [Audio](#audio)
  * [Fonts](#fonts)
  * [Gif](#gif)
  * [SVG](#svg)
  * [Network](#network-1)
  * [Cache](#cache)
  * [Rendering](#rendering-1)
  * [Part Three: Accessibility, Security, Analytics, and Privacy](#part-three--accessibility--security--analytics--and-privacy)
    + [Accessibility](#accessibility)
    + [Security](#security)
    + [Analytics](#analytics)
    + [Privacy](#privacy)



## Part One : The Web Browser Engine.


### Introduction To Browser Internals

When developing browser based web applications, its is beneficial to know the internals of the fundational software in which web application runs, i.e,  the web browser. This essential knowledge helps to write efficient applications by understanding the nuances of why things behaves in a certain way.


#### Web Browsers Engines

Web Browser Engine or also known as Layout Engine or Rendering Engine is a core software component of major Web Browsers. This engine is responsible for the transforming HTML documents and other resources of the web page such as images, videos, fonts, gifs, 3D shapes to an interactive visual representation on the users device.

There are a number of web browsers developed until now and is ever growing in numbers. As a developer writing applications running inside these web browsers, instead of targeting to different browsers, it would be relevant discussing the browsers engines, since major browsers have similar engines under their hood.

Major browser engines:



1. Blink
2. Gecko
3. Webkit


#### Webkit

This engine is originally a fork from KDE project. Currently maintained by Apple and used in Safari and iOS browsers. It has two following components.



1. WebCore

    It is a layout, rendering, and DOM library for HTML and SVG elements.

2. JavaScriptCore


#### Blink.

Blink was formed as fork from Webkit. It is currently actively developed and maintained by Google. This is the underlying software for Chromium like browsers, including, Google Chrome, Brave, Edge etc. Unlike Webkit, Blink has few additional major components.



1. DOM, HTML DOM and CSS rendering engines.
2. Web IDL implementation.
3. Skia Graphics engine.
4. V8 JavaScript Engine.


#### Gecko

This is a browser engine developed by Mozilla and used in Firefox. 


#### How web browsers work
TBD


### Measuring Web Performance In Browsers


#### Core Metrics


- ##### LCP


- ##### FCP


- ##### TTI


- ##### TBT


- ##### FID


- ##### MPFID


- ##### CLS


- ##### FCI


### Browser Components


#### Network


- ##### Latency and Bandwidth (Perceived Speed)


- ##### TCP


- ##### UDP


- ##### TLS


- ##### Wifi and Mobile Networks


- ##### HTTP(1, 1.2, 2, 3)


- ##### Real Time


    - ###### XHR Polling


    - ###### EventSource


    - ###### WebSockets


    - ###### WebRTC


#### Storage


  - ##### Cookies.


  - ##### Local storage.


  - ##### Session storage.


  - ##### IndexedDB.


  - ##### Web SQL.(deprecated)


  - ##### Cache storage


    - ###### Memory Cache


    - ###### Service Worker Cache


    - ######  HTTP Cache


    - ###### Push Cache


#### Parsing


#### Rendering


#### Scripting


## Part Two: Performance and Optimization.


### HTML
Enable text compression


### CSS
Minify CSS
Remove unused CSS


### JavaScript
 Minify JavaScript


### Images
Defer offscreen images
Properly size images
Serve images in modern formats
Efficiently encode images


### Video
Use video formats for animated content


## Audio


## Fonts
Basic font loading
Loading groups of fonts
Loading fonts with a timeout
Prioritised loading
Custom font display
Optimise for caching


## Gif


## SVG


## Network
Preconnect to required origins
Preload key requests
Reduce server response times (TTFB)


## Cache
Avoid multiple page redirects


## Rendering
Eliminate render-blocking resources
Lazy load third-party resources with facades
Reduce the impact of third-party code
Avoid non-composited animations
Avoid layout shifts


## Part Three: Accessibility, Security, Analytics, and Privacy


### Accessibility


### Security


### Analytics


### Privacy
