---
title: 'Connect Arduino to Azure IoT - Lesson 1: Get tools (macOS) | Microsoft Docs'
description: Download and install the necessary tools and software for the first sample application for Adafruit Feather M0 WiFi on macOS.
services: iot-hub
documentationcenter: ''
author: shizn
manager: timtl
tags: ''
keywords: 'arduino development tools, iot development, iot software, internet of things software, install git on mac, install node js mac'

ms.assetid: 0262f3dd-0259-4eb0-962f-9fb534f8359e
ms.service: iot-hub
ms.devlang: arduino
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 3/21/2017
ms.author: xshi

---
# Get the tools (macOS 10.10)
> [!div class="op_single_selector"]
> * [Windows 7 or later][windows]
> * [Ubuntu 16.04][ubuntu]
> * [macOS 10.10][macos]

## What you will do

Download the development tools and the software for the first sample application for your Adafruit Feather M0 WiFi Arduino board. 

If you have any problems, look for solutions on the [troubleshooting page][troubleshooting].

> [!NOTE]
> Although the programming language of the main logic is Arduino, Node.js tools are used in the lessons to build and deploy sample applications.

## What you will learn
In this article, you will learn:

* How to install Git and Node.js.
  * [Git](https://git-scm.com) is an open source distributed version control system. The sample application for this article is stored on Git.
  * [Node.js](https://nodejs.org/en/) is a JavaScript runtime with a rich package ecosystem.
* How to use NPM to install additional Node.js development tools.
  * The minimum required version of Node.js is 4.5 LTS.
  * [NPM](https://www.npmjs.com) is one of the package managers for Node.js.

## What you need
To complete this operation, you will need:
* An Internet connection to download the development tools and the software.
* A Mac that is running macOS Yosemite (10.10) or later.

## Install Git and Node.js
To install Git and Node.js, use the [Homebrew](http://brew.sh) package management utility by following these steps:

1. Install Homebrew. If you've already installed Homebrew, go to step 2.

   1. Press `Cmd + Space` and enter `Terminal` to open a terminal.
   2. Run the following command:

      ```bash
      /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
      ```
2. Install Git and Node.js by running the following command:

   ```bash
   brew install node git
   ```

## Install additional Node.js development tools
Use [gulp.js](http://gulpjs.com) to automate the deployment of the sample application to your Arduino board.

Install `gulp`, `device-discovery-cli` by running the following command in the terminal:

```bash
sudo npm install -g gulp device-discovery-cli
```

If you experience issues installing Node.js and these additional development tools on macOS, see the [troubleshooting guide][troubleshooting] for solutions to common problems.

## Install Visual Studio Code
[Download](https://code.visualstudio.com/docs/setup/osx) and install Visual Studio Code. Visual Studio Code is a lightweight but powerful source code editor for Windows, Linux, and macOS. You use this editor later in the tutorial to edit the sample code.

## Summary
You've installed the required development tools and software for the first sample application. The next task is to create, deploy, and run the sample application on your Arduino board.

## Next steps
[Create and deploy the blink application][create-and-deploy-the-blink-application]
<!-- Images and links -->

[windows]: iot-hub-adafruit-feather-m0-wifi-kit-arduino-lesson1-get-the-tools-win32.md
[ubuntu]: iot-hub-adafruit-feather-m0-wifi-kit-arduino-lesson1-get-the-tools-ubuntu.md
[macos]: iot-hub-adafruit-feather-m0-wifi-kit-arduino-lesson1-get-the-tools-mac.md
[troubleshooting]: iot-hub-adafruit-feather-m0-wifi-kit-arduino-troubleshooting.md
[create-and-deploy-the-blink-application]: iot-hub-adafruit-feather-m0-wifi-kit-arduino-lesson1-deploy-blink-app.md