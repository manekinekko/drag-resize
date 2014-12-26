drag-resize
============

This is a Polymer element that enables any DOM element to be draggable and resizable.

## Usage

1) Install the component from bower:

```shell
bower install drag-resize
```

2) Insert the component into your page:

```html
<link rel="import" href="drag-resize.html">
```

3) Add the ```<drag-resize></drag-resize>``` anywhere in your document:

```html
<body>
	
	<!-- content -->

	<drag-resize></drag-resize>
	
	<!-- content -->

</body>
```

4) Then, add the ```drag-resize``` attribute to the elements you want to be draggable & resizable, ex.:

```html
<drag-resize></drag-resize>

<!-- add the attribute "drag-resize" to make this element draggable and resizable -->
<div drag-resize>this is a DIV element.</div>

<!-- this element won't be draggable nor resizable -->
<div>this is a DIV element.</div>
```

## Attributes

### aspectRatio 
is a property that preserves the aspectRatio.

```
@property aspectRatio
@type bool
@default false
```

### selectedElement 
is the current selected element.

```
@property selectedElement
@type DOMElement
@default null
```

### resizeHandle 
is the resize handler of the element.

```
@property resizeHandle
@type DOMElement
@default null
```

### allowBlur
is the attributes that allows automatic blur onclick.

```
@property allowBlur
@type bool
@default true
```

### enable 
is the attribute that toggles globally the resize.

```
@property enable
@type bool
@default true	    	
```

### zIndex 
is the highest Z-Index allocated.

```
@property zIndex
@type number
@default 1
```

### bbox 
is the Bounding box area, in pixels.

```
@property bbox
@type object
@default { elmX: 0, elmY: 0, elmH: 0, elmW: 0 }
```

### mouse 
is the mouse information.

```
@property mouse
@type object
@default { x: 0, y: 0, last: { x: 0, y: 0 }, offset: { x: 0, y: 0 } }
```

### minWidth 
is the minimum pixel width of the element.

```
@property minWidth
@type number
@default 30
```

### minHeight 
is the minimum pixel height of the element.

```
@property minHeight
@type number
@default 30
```

### minLeft 
is the minimum left position, in pixels.

```
@property minLeft
@type number
@default -9999
```

### maxLeft 
is the maximum left position, in pixels.

```
@property maxLeft
@type number
@default 9999
```

### minTop 
is the minimum top position, in pixels.

```
@property minTop
@type number
@default -9999    
```

### maxTop 
is the minimum top position, in pixels.

```
@property maxTop
@type number
@default 9999
```

### zoomRatio 
is the zoom ratio used to scale the element.

```
@property zoomRatio
@type number
@default 1
```

### zoomLevel 
is the original zoom level.

```
@property zoomLevel
@type number
@default 1
```

## Testing Your Element


```sh
python -m SimpleHTTPServer
```

Or other method using NodeJS:

```sh
http-server ./
```

This starts a web server on port 8000, so you can test your new element by navigating a browser to `localhost:8000/test/index.html`.


## License

Copyright (c) 2014 Wassim Chegham. All rights reserved.
This code may only be used under the BSD style license found at http://polymer.github.io/LICENSE.txt
The complete set of authors may be found at http://polymer.github.io/AUTHORS.txt
The complete set of contributors may be found at http://polymer.github.io/CONTRIBUTORS.txt
Code distributed by Google as part of the polymer project is also
subject to an additional IP rights grant found at http://polymer.github.io/PATENTS.txt
