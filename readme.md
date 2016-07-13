<table>
	<tr>
		<td><img src="https://ga-shop-production-herokuapp-com.global.ssl.fastly.net/assets/images/apple-touch-icon_2-2s3.png">
		</td>
		<td>
		<h3>Lightning Talk</h3>
		<h1>Polymer</h1>
		<h6>Kate Nelson</h6>
		</td>
	</tr>
</table>

Polymer is an open-source project led by a team of developers working within the Chrome organization at Google.


## Problem Polymer Solves

Polymer is a web library built on top of [Web Components](https://developer.mozilla.org/en-US/docs/Web/Web_Components). It is designed to leverage the evolving web platform on modern browsers. 

Polymer allows you to create custom elements (resuable web components). Your browser knows how to handle these elements (ex: takes care of default HTML and JS handling).


## References
+ [The Polymer Project](https://www.polymer-project.org/) 
+ [Polymer Cheat Sheet](https://www.cheatography.com/jonathanberi/cheat-sheets/polymer-js/) 
+ [Web Components Overview](https://blogs.windows.com/msedgedev/2015/07/14/bringing-componentization-to-the-web-an-overview-of-web-components/)



## Demo
###Custom Elements  

The path to a custom element uses the component name listed in this element's bower.json file—rather than the actual directory name. 

+ Elements are reusable and organized to be used alongside other elements, so components are referenced outside the project. 

**Local (/Shadow) DOM** is the set of DOM elements managed by your element.

+ Local DOM lets you add a scoped DOM tree inside an element, with local styles and markup that are decoupled from the rest of the web page.

###Defines the element:
![Profile Wireframe](https://s31.postimg.org/le9ifiuzf/Screen_Shot_2016_07_13_at_8_49_03_AM.png)

+ "dom-module" wraps the element's local DOM definition.
+ "template" is where you specify your element's stucture and style.
+ Styles within the "style" tag are scoped to the local DOM and won't affect the rest of your document.
+ Custom styling properties are used to keep users fromm styling your element's internal features accidentally.

---

###The Polymer call *registers* the element so it’s recognized by the browser:
![Profile Wireframe](https://s31.postimg.org/8onnlge0b/Screen_Shot_2016_07_13_at_8_56_58_AM.png)



+ The argument to the Polymer call is the new element’s prototype.
+ The "is" property on the prototype is the new element’s name. It needs to match the id on the <dom-module> that contains the element’s template.



##Polymer vs. ReactJS
+ **Polymer:** HTML-like, easy for new users, less complicated than React, HTML imports
+ **React:** Server-side rendering is better (rendered on server and browser in the same way), JS modules



