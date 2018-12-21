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
  hidden: false;                       // [OPTIONAL] default:false, show the shortcut in the power-access menu
}
```

# Shortcut Menu

```html
<link rel="import" href="/path/to/power-access.html">
...
<power-access></power-access>
```

# Inject HTML / Styles
> As of version 1.0.0, style injections are not longer supported, since the `<power-access>` component no longer uses ShadowDOM.