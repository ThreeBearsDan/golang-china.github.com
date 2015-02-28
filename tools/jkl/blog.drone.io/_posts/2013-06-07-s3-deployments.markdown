---
layout: posts
title: "Amazone S3 Uploads"
author: Brad Rydzewski
authorlink: https://drone.io/bradrydzewski
---

Today we added the ability to upload files to a bucket in Amazon S3.
![SSH Deployment Setup](/img/screenshot_deployments_s3.png)

Other recent updates worth mentioning:

### SSH Deployments and Custom Ports

SSH deployments are now allowed on non-standard ports. You can specify the port
using the standard `host:port` convention. See our SSH deployment documentation
for more information.

### Cancel Builds

Builds can be manually cancelled. This is great for testing changes to build
scripts for projects that take a long time to build. Look for the "cancel"
button on the build screen.
