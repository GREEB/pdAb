# 🙏 pdAb 🙏

Pdab is a little script to show an overlay to adblock users.

![example](https://i.imgur.com/VcoCEaf.png|alt=example)

## Usage
1. Detect if user uses Adblocker

   [detectadblock](http://www.detectadblock.com/).

   [fuckadblock](https://fuckadblock.sitexw.fr).


2. Run pdab function with desired parameters 🎨

Example:
```JavaScript
 pdab(
 true,
 '#212121',
 '#ffffff',
 '#d96064',
 '#96e272',
 '#404040',
 '33px',
 '23px',
 'Adblock Detected',
 'Alis.io will only be able to stay online if you whitelist us',
 'You can do it up here somewhere',
 '#ee9295',
 '#d96065',
 0.95,
 true,
 '#overlays',
 );

```
Parameters:
```JavaScript
pdab(
  insist,
  background,
  mainTextColor,
  subTextColor,
  actionTextColor,
  actionTextBackground,
  mainTextSize,
  subTextSize,
  mainMsg,
  subMsg,
  actionMsg,
  smileyMainColor,
  smileySecColor,
  opacity,
  blur,
  blurSelector,
);

```

* insist (BOOLEAN) To keep overlay open
* background (HEX) Background for pdab
* mainTextColor (HEX)
* subTextColor (HEX)
* actionTextColor (HEX)
* actionTextBackground (HEX)
* mainTextSize (PX)
* subTextSize (PX)
* mainMsg (STRING) Main msg e.g Adblock Detected
* subMsg (STRING) Sub msg e.g {URL} will only be able to stay online if you whitelist {URL}
* actionMsg (STRING) Action msg on the top right
* smileyMainColor (HEX) Main smiley color (skincolor)
* smileySecColor (HEX) Border color
* opacity (0.00 - 1.00) Opacity for pdab to tease the website in the bg
* blur (BOOLEAN) To help blend pdab with the bg only needed if ^ is > 1
* blurSelector (id, class) What to blur
