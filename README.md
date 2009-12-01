Touch
=====

Touch is a no-frills ultra fast "drag" class for MooTools 1.2.
It serves the purpose to enable dragging your mouse or finger on normal-sized browsers and mobile safari.
Supports safari 3+, mobile safari 2+, firefox 2+, ie 6+.
It's API consists in 4 events, 2 public methods and 2 delta values.

This is not, by any means, an idiot-proof drag implementation.
The only purpose of this class is to easily retrieve delta values, so that you can use them for dragging, resizing, swiping, or virtual masturbation.

![Screenshot](http://mad4milk.net/plugins/Touch/Touch.png)

How to use
----------

Instantiate Touch with an element you want to read the delta values from:

	var touch = new Touch(element);

Add start, move, end and cancel events:

	touch.addEvent('start', function(){
		
	});

	touch.addEvent('move', function(dx, dy){
		
	});

	touch.addEvent('end', function(){
		
	});

	touch.addEvent('cancel', function(){
		
	});

* The start event fires when you mousedown or fingerdown the element.
* The cancel event fires when there's been no movement from the start event.
* The move event fires when there's movement while keeping your mouse or finger down. It receives delta values, which are the amount of movement made from the start position of your mouse cursor or finger.
* The end event fires when you relieve your finger or depress the mouse button, and only when there's been movement.


Example
-------

You can see a simple drag&drop implementation using Touch.js in [this shell](http://mooshell.net/asMBX/9).