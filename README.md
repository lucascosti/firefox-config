# firefox-config
A place to store what I need to change for Firefox on Windows.

In about:config, change:
* `layout.css.devPixelsPerPx` to `1` ; This makes the chrome and content not respect the DPI setting of the OS. Prior to Firefox 22, the OS DPI setting would affect the chrome only (good), but not the web content. After FF22 it affected both (bad).
* `gfx.direct2d.disabled` to `true` ; This stops fonts becoming fuzzy.

In the profile folder, create a `chrome` directory and put in the `userChrome.css` file to set the correct size for all the chrome text. With `layout.css.devPixelsPerPx` to `1`, all the chrome becomes teeny-tiny otherwise.
