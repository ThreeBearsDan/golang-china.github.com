---
layout: posts
title: "Groovy, Gradle, Google AppEngine"
author: Brad Rydzewski
authorlink: https://drone.io/bradrydzewski
---
A few weeks ago Guillaume Laforge, the creator of Groovy, contacted us on 
[Google+](https://plus.google.com/114130972232398734985/posts/dxCoWnCu9DJ)
asking for Groovy, Gradle and Google AppEngine support:
![Google+ Groovy Request](/img/google_plus_groovy.png)

We were up for the challenge! Today we are happy to announce support for
Groovy, Gradle and Google AppEngine for the Python and Java runtimes
(including JVM languages like Groovy, of course).

### Groovy

When creating new project, you will have the option to choose the Groovy
runtime. Included with the Groovy runtime are Gradle, Maven and Ant.

![Groovy Option](/img/screenshot_languages_groovy.png)

### Google AppEngine

Once your project is created, you can add an AppEngine deployment step. For
now, you will need to copy and paste your AppEngine refresh token, found in the
`.appcfg_oauth2_tokens` or `.appcfg_oauth2_tokens_java` file in your `$HOME`
directory:

![Groovy Option](/img/screenshot_deployments_gae.png)

And that’s it! Simple right?

Drone will traverse your project's directory structure, find and parse your
app.yaml, and execute the necessary commands to deploy your code.

### Sign up for Free

Not using Drone for continuous integration yet? It is easy to get started and
completely free for open source projects. [Sign up today](https://drone.io/register).
