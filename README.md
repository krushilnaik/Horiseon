# Horiseon

[<img src="https://i.imgur.com/nT9LavM.png" width="150" />](https://krushilnaik.github.io/Horiseon)

The first assignment for the Rutgers coding bootcamp: optimizing the landing page of a hypothetical SEO firm.

## Table of Contents

[Tasks](#tasks)

[The Results](#the-results)

[The How](#the-how)

[Possible Improvements](#possible-improvements)

## Tasks

-  From bootcamp:
   -  [x] Ensure some form of 508 Compliance
   -  [x] Improve DRYness
   -  [x] ~~Ironic~~ SEO
-  From myself:
   -  [x] Asset and delivery optimization

## The Results

![Site GIF](./screens/horiseon.gif)

### PageSpeed Insights scores before optimization... 💀

|                          Desktop                          |                         Mobile                          |
| :-------------------------------------------------------: | :-----------------------------------------------------: |
| ![desktop scores](./benchmarks/desktop/pagespeed-pre.png) | ![mobile scores](./benchmarks/mobile/pagespeed-pre.png) |

### ... and after 😍

|                          Desktop                           |                          Mobile                          |
| :--------------------------------------------------------: | :------------------------------------------------------: |
| ![desktop scores](./benchmarks/desktop/pagespeed-post.png) | ![mobile scores](./benchmarks/mobile/pagespeed-post.png) |

---

### Chrome Lighthouse scores before optimization... 👀

|                          Desktop                           |                          Mobile                          |
| :--------------------------------------------------------: | :------------------------------------------------------: |
| ![desktop scores](./benchmarks/desktop/lighthouse-pre.png) | ![mobile scores](./benchmarks/mobile/lighthouse-pre.png) |

### ... and after 😍

|                           Desktop                           |                          Mobile                           |
| :---------------------------------------------------------: | :-------------------------------------------------------: |
| ![desktop scores](./benchmarks/desktop/lighthouse-post.png) | ![mobile scores](./benchmarks/mobile/lighthouse-post.png) |

---

## The How

-  The images were shrunken down to their CSS-defined max widths/heights to prevent unnecessary down-scaling. Afterwards, they were compressed via [tinypng](https://tinypng.com)

   -  NOTE: Since this is still an assignment to be graded by a human, minification of HTML and CSS will be skipped

-  35% of `./assets/css/styles.css` was found to be redundant so I cut those out, consolidating elements with similar properties where sensible.
   -  NOTE: Higher mobile scores (and beauty in general) can be achieved by making the site responsive, but we haven't covered that yet. I'll come back and implement this later

---

## Possible Improvements:

-  Network analyses show an abysmal render time (~9s) on "Slow 3G" throttling. I figure this is to be expected, but if anyone knows a way to bring it under 3 seconds, let me know or submit a pull request! 👍
