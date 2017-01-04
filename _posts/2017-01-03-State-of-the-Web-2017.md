---
layout: post
title:  "State of the Web, 2017 Edition"
date:   2017-01-3 19:21:00
categories:
 - javascript
banner_image: aurelia.png
comments: true
---
As 2017 begins, I've been reflecting on the pace of technology on the web.

My preferred environment two years ago:<br/>
 - Angular 1 in ES5<br/>
 - Bower + NPM<br/>
 - Grunt<br/>
 - LESS<br/>
 - jquery, lodash & moment<br/>
 - RequireJS (although it pissed me off to no end with Angular1)<br/>
 - WebStorm<br/>
 - ASP.NET Web API<br/>

Today, the picture is different. ES2015 and ES2016 have arrived, however TypeScript seems to be dominating the scene and has rapidly expanded across multiple frameworks. Angular 2 is the most well known but Aurelia has used been out a little longer. Grunt gave way to gulp, which in turn is being threatened by Webpack. From my perspective TypeScript is the best thing to happen to the web in a long time because of the ease of refactoring. That said, it too has had some hicups with the process of aquiring definitions changing _three times_ in the last year.... and don't get me started on debugging with async / await.

Aurelia, my framework of choice, has also seen many releases and iterations. Like Angular 2, you can write your apps in TypeScript and it uses JSPM out of the box... unless you use the Aurelia CLI - which counter-intuitively regresses (IMHO) to RequireJS over JSPM (for many reasons). Either way, the build pipeline seems to have gotten much more complex this year... and simple bugs have been harder to squash.

I used Bootstrap (although a heavily modified fork) and LESS on a project for the Travel Channel. It was more painful than I recall either Bootstrap or LESS being in the past. Possibly due to the many, many custom modifications (like 28 columns?!?!). Possibly due to poorly defined requirements that rapidly evolved and required many, many hacks. Possibly due to my limited LESS knowledge. Lately, however, I'm using pure SASS with Bourbon... and eyeing CSS Variables to add to my workflow.

My current best of breed environment:<br/>
 - Aurelia & TypeScript<br/>
 - Aurelia CLI... though I'm ready for the webpack-dashboard build to mature so I can migrate away from this r.js (again!)<br/>
 - npm & better-npm-run<br/>
 - lodash & moment (jquery is no longer needed)<br/>
 - SASS + Bourbon + \_include-media<br/>
 - MateralizeCSS<br/>
 - VS Code + Team Essentials<br/>
 - Node + Hapi.js<br/>

It's just such an exciting time right now. Stodgy old back-end dev's cry that it's too fast (especially the JSP folks who haven't done anything new in YEARS!)... I say, it's not _fast enough_! Hurry up already!
