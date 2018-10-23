---
layout: post
title:  "Broadcasting SNS from AWS Realtime"
date:   2018-05-04 16:49:51 -0500
categories: jekyll update
prettyDate: April 4, 2018
datetime: "2018-05-04"
authorPic: "assets/images/avatar.jpg"
titlePic: "assets/images/clouds-cornfield-countryside-158827-e1523134005820-1000x500.jpg"
tags: [AWS, SNS, Websockets, Javascript]
---
Recently, at a client site, my team was in need of integrating real-time broadcast capability to a browser-based interface (written in React). To achieve this, we decided on establishing a persistent websocket connection between the client interface and an EC2 instance running a Node.js server. The SNS topic would then send an HTTP Post to that server on broadcast. In this post I will guide you through the process of creating a bare-bones sample SNS real-time broadcast application for your front-end application of choice.

TL;DR here’s a Git repo with the completed project code.

