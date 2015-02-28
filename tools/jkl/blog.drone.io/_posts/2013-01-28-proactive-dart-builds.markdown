---
layout: posts
title: "Proactively Testing your Dart Projects"
author: Brad Rydzewski
authorlink: https://drone.io/bradrydzewski
---

Do the weekly Dart releases ever break your build? Of course not! But
just in case, we've added a new feature to proactively build and test your
Dart project every time a new version of Dart is released.

We're calling this feature **triggers**.

To setup a trigger, navigate your project's **settings > triggers** page:

![Proactive Dart Builds](/img/screenshot_triggers_dart.png)

And that's it! Simple right?

And even if you aren't using triggers, Drone guarantees that your code is
tested using the latest version of the SDK. Before each build, Drone will
check for a new version of the SDK (and DumpRenderTree, dart_analyzer, pub, etc)
and will upgrade if available:

![Dart Upgrades](/img/screenshot_stdout_dart-upgrade.png)

Not using Drone for continuous integration yet? It is easy to get started and
completely **free** for open source projects. [Sign up today](https://drone.io/register).
