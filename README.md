# sigame-clicker

This bot-like tool allows you to click reply button without any significant delay in quiz game named "SiGame".

## Usage

For now, you need to fork this repo and launch `sigame-clicker.js` file like this:

```
node sigame-clicker.js
```

After that, the process will start running.

To enable triggering mode, you need to press tilda key (`~`) and point cursor to the place on the screen, where the reply progress bar will be located. When enabled, script will check with an interval of `100ms` if the pixel color under cursor pointer contains has white (`ffffff`) value in RGB format. If positive, it immediately invokes RMB click (default reply button hotkey in SiGame) and you are ready to answer active question. After triggering click, script resets triggering mode to `false` to prevent any accidental clicks further on.

## Future roadmap

* Add support for CLI params to read and recognized by the script, so you don't need to modify source files to adjust triggering functionality by yourself.
* Add options to trigger reply triggering based not only on pixel color beneath cursor but generally (probably fix coordinates at which the color will be read based on the screen dimensions).
* Implement some kind of a building thing (`?`) and publish this package to the npm registry.

