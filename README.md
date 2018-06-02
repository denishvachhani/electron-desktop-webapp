# Prices

Simple [Electron](http://electronjs.org) application that shows the current
price of oil, gold, and silver using the STOOQ API.

I have also mention steps to package this electron app along with generate (.dmg) file.

![screenshot](https://cloud.githubusercontent.com/assets/671378/21198004/6e7a3798-c1f2-11e6-8228-495de90b7797.png)

## Getting started

- Install [Node LTS](https://nodejs.org)
- Clone this repository
- `cd electron-desktop-webapp`
- `npm install` to install the application's dependencies
- `npm start` to start the application

## Packaging elecron app

- Run `npm install electron-packager -g` to install [electron-packager](https://github.com/electron-userland/electron-packager)
- Create package with command `electron-packager .` (Make sure you are inside project directory)
- It will generate (.App) directory for your electron app

## Generate (.dmg) file 

- Run `npm i electron-installer-dmg -g` to install [electron-installer-dmg](https://github.com/mongodb-js/electron-installer-dmg)
- Once packaged as mention above, we can create dmg with command `electron-installer-dmg <path/to/.app> <appname>`
- It will generate .dmg file

## For other installer type ( windows, linux etc )
- [Other OS installer] https://github.com/electron-userland/electron-packager#related

## Here are some ideas on how it can be improved using other Electron APIs.

- Double-click commodity to open directly on https://stooq.com
- Refresh automatically on an interval.
- Add the price of platinum (`PL=F`) to the app.
- Export prices to a `.csv` file.
- Show percentage change in price.
- Show notifications when prices go above/below certain amounts.
