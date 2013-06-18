jVanilla
========

jVanilla is a menu jQuery plugin that takes an existing pure CSS drop-down menu (so it degrades gracefully without JavaScript) and adds the following enhancements.

- Animations when showing submenus
- Support one submenu level
- Timed delay on mouseout
- Top level menu links can be inactive (on hover effect)
- Last submenu right-aligned

Usage:

	$(document).ready(function (){
		$('.menu-hover').jVanilla({
			speed               : 50,       // speed in milliseconds 
											// of the opening animation
			animation           : 'fading', // type of the animation 
											// fading || sliding
			eventType           : 'hover',  // type of event that trigger
											// animation hover || click
			delay               : 100,      // the delay in milliseconds that 
											// the mouse can remain outside 
											// the submenu without it closing
			isHoverClickable    : false,    // set to true if you want to enable 
											// the click on the first level link
			isLastRightAlign    : true      // set to false if you want to align 
											// left the last submenu
		});
	});
