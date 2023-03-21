### Setup
Add the js and css CDN and create a new window

```html
<script src="https://russell2259.github.io/Nightmare-Windows/windows.js"></script>
<link rel="stylesheet" href="https://russell2259.github.io/Nightmare-Windows/windows.css">
```
```js
new Window({
"title": "Example",
"type": "url",
"url": "https://example.com",
"width": 600,
"height": 400,
})
```

### Advanced
```js
new Window({
"title": "Example", //Window Title - Required
"type": "html", //URL, Html or Js - Required
"url": "https://example.com", //For url
"html": "<button>hi</button>", //For html
"js": "https://example.com/script.js", //For js url
"width": 800, //Width - No quotes
"height": 600, //Height - No quotes
"theme": "dark" //Light or Dark
})
```

### Creating Apps
**url**

Just add a url which will be added in an iframe

**html**

Just add html code which will be added in the window

**js**

Add a url to a js file that will be run onclick. Allows for more custom features

When creating a js app it will inject a var called `appid` which is the window. You can append a element inside using `appid.appendChild(element)`
