# Horiseon

<p align="center">
	<a href="https://krushilnaik.github.io/Horiseon">
		<img src="https://i.imgur.com/nT9LavM.png" height="40" />
	</a>
</p>

The first assignment for the Rutgers coding bootcamp: optimizing the landing page of a hypothetical SEO firm.

## Table of Contents

1. [Tasks](#tasks)

2. [The Results](#the-results)

   -  [Desktop](#desktop)
   -  [Mobile](#mobile)

3. [The How](#the-how)

4. [Possible Improvements](#possible-improvements)

## Tasks

-  From bootcamp:
   -  [x] Ensure some form of 508 Compliance
   -  [ ] Improve DRYness
   -  [x] ~~Ironic~~ SEO
-  From myself:
   -  [x] Asset and delivery optimization
   -  [ ] Make the site responsive

## The Results

### Desktop

![Site GIF](./screens/horiseon.desktop.gif)

### Mobile

![Site GIF](./screens/horiseon.mobile.gif)

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

-  35% of `./assets/css/styles.css` (renamed to `style.desktop.css`) was found to be redundant so I cut those out, consolidating elements with similar properties where sensible.
   -  NOTE: Higher mobile scores (and beauty in general) can be achieved by making the site responsive, but we haven't covered that yet. I'll come back and implement this later

---

## Possible Improvements:

-  The site would've benefitted from making the `<section>`'s content accordions on mobile, but that wasn't feasible without restructuring the DOM so I made due with what was given
-  Network analyses show an abysmal render time (~9s) on "Slow 3G" throttling. I figure this is to be expected, but if anyone knows a way to bring it under 3 seconds, let me know or submit a pull request! 👍
