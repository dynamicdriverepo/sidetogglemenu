# Responsive Side Toggle Menu #

*Description:* Side Toggle Menu lets you add a side bar menu to your page that slides in from the left or right edge of the browser window. It supports two types of unveiling- either by nudging the rest of the page and making room for itself, or overlaying the page (and not displacing its neighbours).  CSS3 transitions are used to power the animation, ensuring a smooth visual experience even on low powered mobile devices. And speaking of mobile devices, the menus are adaptive in that it automatically switches to a basic drop down menu using a toggle button at the top of the page when the user's device width is 480px or less (configurable). Finally, the menus are dismissed when the user clicks anywhere on the page that's outside the menus, or when clicking on a link inside the menu.

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.7 or above (served via Google CDN)
+ sidetogglemenu.js
+ sidetogglemenu.js
+ togglemenu.txt (external menu definition for 2nd demo)

*Step 2:* Add the below code to the HEAD section of your page:

	<link rel="stylesheet" href="sidetogglemenu.css" />
	
	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.8/jquery.min.js"></script>
	
	<script src="sidetogglemenu.js">
	
	/*
	* Responsive Side Toggle Menu(c) Dynamic Drive (www.dynamicdrive.com)
	* Last updated: May 28th, 13'
	* Visit http://www.dynamicdrive.com/ for this script and 100s more.
	*/
	
	</script>
	
	<script>
	
	jQuery(function(){ // on DOM load
		menu1 = new sidetogglemenu({  // initialize first menu example
			id: 'togglemenu1',
			marginoffset: 10
		})
	
		menu2 = new sidetogglemenu({  // initialize second menu example
			id: 'togglemenu2',
			position: 'right',
			source: 'togglemenu.txt',
			revealamt: -5
		})
	})
	
	</script>

*Step 3:* Then, add the below sample markup to your page:

	<button onClick="menu1.toggle();" class="sideviewtoggle">Toggle Menu 1</button>
	<button onClick="menu2.toggle()" class="sideviewtoggle">Toggle Menu 2</button>
	
	<div id="togglemenu1" class="sidetogglemenu">
	
		<ul>
		<li><a href="http://www.dynamicdrive.com/">Dynamic Drive</a></li>
		<li><a href="http://www.dynamicdrive.com/style/">CSS Library</a></li>
		<li><a href="http://www.dynamicdrive.com/forums/">Forums</a></li>
		<li><a href="http://tools.dynamicdrive.com/imageoptimizer/">Gif Optimizer</a></li>
		<li><a href="http://tools.dynamicdrive.com/favicon/">Favicon Creator</a></li>
		<li><a href="http://tools.dynamicdrive.com/button/">Button Maker</a></li>
		</ul>
		
		<p style="padding:10px">
		This menu's markup is defined inline on the page. With the setting <code>pushcontent: true</code>, the menu shifts the rest of the page's content to make room for itself when revealed.
		</p>
	
	</div>

## Responsive Side Toggle Menu set up ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex1/sidetogglemenu.htm>
