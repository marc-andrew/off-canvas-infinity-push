off-canvas-infinity-push
========================

Off Canvas Infinity Push is a jQuery plugin that gives you the ability to make any desktop navigation into a mobile navigation.
This plugin offers unlimited sub navigations. 

### Demos
* [Left Navigation](http://www.marcandrew.net/off-canvas-infinity-push/)
* [Right Navigation](http://www.marcandrew.net/off-canvas-infinity-push/index2.html)
* [Responsive](http://www.marcandrew.net/off-canvas-infinity-push/index3.html)
* [No Auto Scroll](http://www.marcandrew.net/off-canvas-infinity-push/index4.html)
* [No Off Canvas](http://www.marcandrew.net/off-canvas-infinity-push/index5.html)
* [Reset](http://www.marcandrew.net/off-canvas-infinity-push/index6.html)

### Live Examples
* [Whistles](http://www.whistles.com/)
* [Brown Bag Clothing](http://www.bbclothing.co.uk/)
* [Woodhouse](http://www.woodhouseclothing.com/)

### Getting Started
Load [jQuery(1.7+)](http://jquery.com/) and include Off Canvas Infinity Push plugin files.
Add the stylesheet (jquery.ma.infinitypush.css) and the plugin (jquery.ma.infinitypush.js or jquery.ma.infinitypush.min.js) in your website.
The stylesheet can be modified to fit the website design.

```html
<!-- Basic stylesheet -->
<link rel="stylesheet" type="text/css" href="plugin/jquery.ma.infinitypush.css" />

<!-- Include js plugin -->
<script src="plugin/jquery.ma.infinitypush.js"></script>
```

### Basic Navigation Markup

```html
<nav id="primary-navigation">
	<ul>
		<li><a href="#">Link</a>

			<ul>
				<li><a href="#">Link</a>

					<ul>
						<li><a href="#">Link</a>

							<ul>
								<li><a href="#">Link</a></li>
								<li><a href="#">Link</a></li>
								<li><a href="#">Link</a></li>
								<li><a href="#">Link</a></li>
							</ul>

						</li>
						<li><a href="#">Link</a></li>
						<li><a href="#">Link</a></li>
						<li><a href="#">Link</a></li>
					</ul>

				</li>
				<li><a href="#">Link</a>

					<ul>
						<li><a href="#">Link</a></li>
						<li><a href="#">Link</a></li>
						<li><a href="#">Link</a></li>
						<li><a href="#">Link</a></li>
					</ul>

				</li>
				<li><a href="#">Link</a></li>
				<li><a href="#">Link</a></li>
			</ul>

		</li>
		<li><a href="#">Link</a></li>
		<li><a href="#">Link</a></li>
		<li><a href="#">Link</a></li>
		<li><a href="#">Link</a></li>
	</ul>
</nav>
```

### Call the plugin
Now call the Off Canvas Push Infinity initializer function and your mobile navigation is ready.

```html
<script type="text/javascript">

	$(document).ready(function(){

		$('#primary-navigation').infinitypush({
			openingspeed: 300,
			closingspeed: 300
		});

	});

</script>
```

### Options

- `offcanvas`: true,                               // Set to "false" to turn off the off canvas
- `offcanvasspeed`: 400,                           // Opening animation for the off canvas in milliseconds
- `offcanvasleft`: true,                           // Set to "false" for the right hand side position
- `openingspeed`: 400,                             // Opening push animation in milliseconds
- `closingspeed`: 400,                             // Closing animation in milliseconds
- `pushdirectionleft`: true,                       // Set the push direction from right to left. "false" for left to right
- `spacing`: 90,                                    // The spacing is in pixel
- `autoScroll`: true,                              // Set to "false" if you don't need the auto scroll up
- `scrollSpeed`: 300,                              // Scroll up animation in milliseconds
- `destroy`: false                                 // Set to "true" to reset the navigation

### License
The MIT License (MIT)
