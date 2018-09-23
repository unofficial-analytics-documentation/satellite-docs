# Script Loading

This documentation discusses script loading while using the Satellite Library.

## Async `_satellite` Library Loading and Static `_satellite` Library Loading

There are generally two approaches for loading analytics scripts—asynchronously and synchronously. Asynchronous script loading is beneficial for overall webpage loading performance. Synchronous script loading is beneficial for ease of implementation. 

Below are general patterns for loading Satellite Library. 

### Async Library Loading

Async Library Loading is loading scripts to a webpage. This means that on a webpage's initial load there is no Satellite Library or other analytics code. The Satellite Library is loaded via JavaScript by being dynamically added to the page. 

```javascript
// Pseudo code referencing code written by: Jacob Kelley, Jon Ong
const promises = []
// Push our DTM scripts to be loaded
const dtmScripts = DTM_SCRIPTS[environment] || DTM_SCRIPTS.default
promises.push(Promise.all(dtmScripts.map(src => loadScript(src, {
  timeout: 500,
}))).then(() => poll(dtmReadyConditionFn, 10, 1000)))
```

### Static Library Loading

Static Library Loading is having DTM scripts on a static page or adding scripts at build time—so rendered content is like a static page.

```html
<script type="text/javascript" src="https://somecustomeanalytics.com/lib.js"></script>
<script type="text/javascript" src="https://somecustomeanalytics.com/dtm-observer.js"></script>
<script type="text/javascript" src="https:////assets.adobedtm.com/somerandomstring/satelliteLib-someotherrandomstring.js"></script>
```
