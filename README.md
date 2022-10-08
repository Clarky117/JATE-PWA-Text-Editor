# JATE Text Editor

![None](https://img.shields.io/badge/license-None-blue)
  
## Table of Contents
1. [Description](#description)
2. [Skills Used](#skills-used)
3. [Installation](#installation)
4. [Readme Visual](#visuals)
5. [Repository and Deployed Application](#links-to-repository-and-deployed-application)
  
## Description

This text editor known as Jate, runs in the browser, and is a single-page application that meets PWA criteria. Jate features a number of data persistence techniques that serve as redundancy in case an option is not supported in the browser, also has functionality offline.

## Skills Used

Considering starter code is provided it is important to be able to read the code already there, identify what it does and what is needed to meet the acceptance criteria.

The first thing needed here is to open the `package.json` file that exists on the root level and input what scripts need to be implemented, thus creating `start:dev`, `start`, `server`, `build`, `install` and `client`.

Next in `webpack.config.js` we add and configure the workbox plugins for the service worker and manifest file. Then under rules the CSS loaders and babel are added to the webpack.

Moving onto `database.js` using the package `idb`, we add logic to both get and update the data that we will be storing in indexedDB. When the user clicks away or closes the application, their notes will be stored to pick up where they left off.

Under `src-sw.js` we implement the asset caching.

Now these are taken care of the last thing needed to complete this PWA is implementing the logic in `install.js` so the user has an installable app.

# Installation

## App

- Visit [heroku](https://clarkys-jate.herokuapp.com/)
- Click download icon

## Repo

- Clone repository
- Open in VS Code and open a new terminal
- run `npm i`
- run `npm run (your input)` depending on what you want to do, refer `package.json` for script


## Visuals

Webpack Config VS Code
![pic](/server/images/1-jate-vscode.png)

Deployed App IndexedDB
![pic](/server/images/2-jate-console.png)

## Links to Repository and Deployed Application

- Repository - [Clarky's Repo](https://github.com/Clarky117/JATE-PWA-Text-Editor)
- Live App - [Jate Text Editor](https://clarkys-jate.herokuapp.com/)
