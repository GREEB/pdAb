# 🙏 pdAb 🙏

Pdab is a little script to show an overlay to adblock users.

![example](https://i.imgur.com/VcoCEaf.png|alt=example)

## Usage
1. Detect if user uses Adblocker

   [detectadblock](http://www.detectadblock.com/).

   [fuckadblock](https://fuckadblock.sitexw.fr).
   

2. Run pdab function with desired parameters 🎨

Example:
```sh
 pdab(true, '#212121', '#ffffff', '#d96064', '#96e272', '#404040', '33px', '23px', 'Adblock Detected', 'Alis.io will only be able to stay online if you whitelist us', 'You can do it up here somewhere', '#ee9295', '#d96065', 0.95, true, '#overlays');

```
Parameters:
```sh
pdab(insist, background, mainTextColor, subTextColor, actionTextColor, actionTextBackground, mainTextSize, subTextSize, mainMsg, subMsg, actionMsg, smileyMainColor, smileySecColor, opacity, blur, blurSelector);

```

* Insist (BOOLEAN) To keep overlay open
* Background (HEX) Background for pdab
* Main-Text-Color (HEX)
* Sub-Text-Color (HEX)
* Action-Text-Color (HEX)
* Action-Text-Bg (HEX)
* Main-Text-size (PX)
* Sub-Text-size (PX)
* Main-msg (STRING) Main msg e.g Adblock Detected
* Sub-msg (STRING) Sub msg e.g {URL} will only be able to stay online if you whitelist {URL}
* Action-msg (STRING) Action msg on the top right
* Smiley-Main-Color (HEX) Main smiley color (skincolor)
* Smiley-Sec-Color (HEX) Border color
* Opacity (0.00 - 1.00) Opacity for pdab to tease the website in the bg
* Content Blur (BOOLEAN) To help blend pdab with the bg only needed if ^ is < 1
* Content Selector (id, class) What to blur
