# \<cr-toast\>

A Clash Royale styled toast notification for Polymer 2.

Only one `cr-toast` at a time will be visible on screen.

Use `opened` to show the toast:

Example:

```html
<cr-toast text="Hello world!" opened></cr-toast>
```

Also `open()` or `show()` can be used to show the toast:

Example:

```html
<cr-button on-click="openToast">Open Toast</cr-button>
<cr-toast id="toast" text="Hello world!"></cr-toast>

...

openToast: function() {
  this.$.toast.open();
}
```

Set `duration` to 0, a negative number or Infinity to persist the toast on screen:

Example:

```html
<cr-toast text="Terms and conditions" opened duration="0">
  <a href="#">Show more</a>
</cr-toast>
```

This element applies the mixin `--sc-ccbackbeat` but does not import `cr-fonts/cr-fonts.html`.
In order to apply the `SC CCBackBeat` font to this element, make sure you've imported `cr-fonts/cr-fonts.html`.
