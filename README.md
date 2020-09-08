## What is Javascript

JavaScript was developed by Brendan Eich, a developer at Netscape Communications Corporation, in 1995. It was created mainly as a language to make web pages look alive.

It went through a plethora of names: initially by the name Mocha, then briefly LiveScript, before being officially named JavaScript. Despite the name, JavaScript is not in any way a spinoff of Java.

JavaScript adds dynamic functionality to websites, such as the pop ups you see on many websites when you mouse over certain items in the browser. Though it was only developed to be used in a browser environment, JavaScript has now evolved into non-browser environments such as web servers in the form of NodeJs. In fact, JavaScript can run on any device that has a special program called "the JavaScript engine".

## The JavaScript engine

Browsers have an embedded JavaScript engine which parses and compiles JavaScript code into machine readable instructions. Examples of JavaScript engines and their code names are:

* V8 - used in Chrome and Opera.
* SpiderMonkey used in Firefox.
* Trident" and Chakra used in different versions of Internet Explorer
* ChakraCore used in Microsoft Edge
* SquirrelFish used in Safari

Different engines have different features and capabilities. Knowing which engine is used for which browser is important in know the features supported by that browser. For example, if a certain feature is known to be supported by V8, then you will know that it probably works in Chrome and Opera.

## JavaScript programs

Programs written in JavaScript are called *scripts* and are provided and executed as plain text with a ".js" file extension. JavaScript scripts don't need any special compilation to run. They can be embedded in the HTML and executed automatically as the page loads.

## Capabilities of in-browser JavaScript

JavaScript does not provide low-level access to memory or CPU which makes it a relatively "safe" programming language. In-browser JavaScript was created for webpage manipulation which requires only interaction with the user and the webserver.

In-browser JavaScript has the following capabilities:

* Adding new HTML content to a web page.
* Modifying the existing content styles.
* Reacting to user actions, such as mouse clicks, mouse pointer movements, key presses, e.t.c.
* Sending requests to remote servers, downloading and uploading files.
* Getting and setting browser cookies.
* Showing alerts, prompts and confirmations to users.
* Storing data on the client-side ("local storage").

## Limitations of in-browser JavaScript

JavaScript has limited capabilities in the browser all for the safety of the user. The goal is to prevent a "rogue" webpage from accessing user's private information or tempering with the user's data.

In-browser JavaScript has the following restrictions:

* JavaScript on a webpage cannot read or write or copy or execute files on the hard disk drive because it has no direct access to the Operating System low-level system functions.
* In modern browsers, it has limited access to files on hard disk through user actions, such "dropping" a file into a browser window or selecting a file via an `<input>` tag.
* JavaScript from one page is restricted access to another page if the pages come from different sites (Same Origin Policy).

## Contents
1. [Language Structure](My%20Notes/LanguageStructure.md)
