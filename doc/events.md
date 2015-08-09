# Events

You can register listeners on a Pannellum viewer to detect when the viewer is loaded,
 if it's currently rendering something.

# Registering a listener

You can easily register a new listener with the `addEventListener` method, for instance to 
register the handler `onLoadedHandler` for the `load` event :

```js
var pannellumViewer = window.pannellum.viewer('myOwnPannellumContainer', panoCfg);
// ...
pannellumViewer.addEventListener("load", onLoadedHandler);
```

# Removing a listener

To remove the `onLoadedHandler` listener for the event `load` :
```js
pannellumViewer.removeEventListener("load", onLoadedHandler);
```

# Existing events


## load
Exectued when a scene is loaded into the viewer.


## render
Triggered when the viewer finish a new render, for instance when you have motion in the viewer.