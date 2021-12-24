`highlight.js` syntax definition for kdl.

For more about highlight.js, see https://highlightjs.org/

For more about kdl, see https://kdl.dev/

### Usage

If you're not using a build system and just want to embed this in your webpage:

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/kdl.js"></script>
<script type="text/javascript">
    hljs.highlightAll();
</script>
```

If you're using webpack / rollup / browserify / node:

```javascript
var hljs = require('highlightjs');
var hljsDefineKDL = require('highlightjs-kdl');

hljsDefineKDL(hljs);
hljs.initHighlightingOnLoad();
```
