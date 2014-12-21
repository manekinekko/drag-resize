drag-n-resize
============


## Getting Started


## Testing Your Element


```sh
python -m SimpleHTTPServer
```

Or other method using NodeJS:

```sh
http-server ./
```

This starts a web server on port 8000, so you can test your new element by navigating a browser to `localhost:8000/test/index.html`.

### web-component-tester

The tests are also compatible with [web-component-tester](https://github.com/Polymer/web-component-tester). You can run them on multiple local browsers via:

```sh
npm install -g web-component-tester
wct
```

## Usage

```html
<link rel="import" href="drag-n-resize.html">
```

Use this element:

```html
<div class="content">
	<drag-n-resize id="resizable"></drag-n-resize>
</div>
```

## Attributes