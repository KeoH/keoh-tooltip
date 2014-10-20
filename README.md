#keoh-tooltip


##Introduction

'keoh-tooltip' is a simple web component. Thanks to [Polymer](https://www.polymer-project.org/) we can create our components in the html.

##Installation of keoh-tooltip

The installation is very simple using [Bower](http://bower.io/):


	bower install --save keoh-tooltip


Then, in you html import Plataform (from Polymer) and import 'keoh-tooltip' too.


	<script src="bower_components/platform/platform.js"></script>
	<link rel="import" href="bower_components/keoh-tooltip/keoh-tooltip.html">


##How to use

Now you can use 'keoh-tooltip' in this html file. You must put it inside of another html element.


	<h1>
		Title of the page
		<keoh-tooltip>Message in the tooltip</keoh-tooltip>
	</h1>


###Position

By default the tooltip appears at the bottom of the element, but you can change it using the 'position' attribute.


	<h1>
		Title of the page
		<keoh-tooltip position="top">Message in the tooltip</keoh-tooltip>
	</h1>


The posible values for 'position' are: 'top', 'bottom' and 'right'

###Styling

You can change the default style of 'keoh-tooltip'. I recomend putting a class and overwrite the values like this.


	<h1>
		Title of the page
		<keoh-tooltip class="tip">Message in the tooltip</keoh-tooltip>
	</h1>

In your css:

	.tip::shadow .tooltip{
		color: red;
		border-color: blue;
	}
