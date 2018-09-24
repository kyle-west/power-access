# power-access

This is a native web component that allows for an accessibility layer on top of 
your web application.


# Register Shortcut

```js
let registrar = new KeyboardShortcutRegistrar();
registrar.register(options, callback)
```

### Options

```js
let options = {
  keyStroke: 'Control+c',              // The key stroke that fires the callback
  displayKeys: '<CTRL> + c',           // The text shown in place of keyStroke to user (if supplied)
  label: 'Copy text to the clipboard'  // The description shown to the user of the action
}
```

# Shortcut Menu

```html
<link rel="import" href="/path/to/power-access.html">
...
<power-access></power-access>
```

# Inject HTML / Styles
```js
document.querySelector('power-access').injectHTML = `
  <style>
    h1 {
      color: red;
    }
  </style>
  <p>This is an injected description paragraph.</p>
`
```