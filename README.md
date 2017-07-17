# \<webda-browser-compatibility-component\>

Project name:

 - webda-browser-compatibility-component from http://webda.io/

[![Build Status](https://travis-ci.org/loopingz/webda-browser-compatibility-component.svg?branch=master)](https://travis-ci.org/loopingz/webda-browser-compatibility-component)

Description:

 - polymer component that display a paper-toast message if the client-browser doesn't match your requirements

Installation: bower install --save webda-browser-compatibility-component

Usage:

 - Define your requirements by editing the bannedAgents and/or minAgents values in webda-browser-compatibility-mixin.html:

        bannedAgents : {
            type: Object,
            value : [
              {name: "Chrome", untilVersion: "59.0.3071.114"},
              {name: "MSIE" , untilVersion: "42"}
            ]
        },
        minAgents : {
            type: Object,
            value : [
              {name: "Chrome", minVersion: "59.0.3071.116"},
              {name: "Firefox" , minVersion: "42"},
            ]
        }

 - Change the warningMsg value in webda-browser-compatibility-component.html to display the message you want:

       warningMsg: {
         type: String,
         value: 'Your browser is not supported'
       }

- Feel free to style the <paper-toast> or use an another component  


Credits:
 - loopingz https://github.com/loopingz
 - 8llouch  https://github.com/8llouch

External library:
 - faisalman ua-parser-js  https://github.com/faisalman/ua-parser-js
