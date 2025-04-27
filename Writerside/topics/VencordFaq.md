# FAQ Vencord Edition

<primary-label ref="stable"/>
<secondary-label ref="beta"/>

<img src="https://media.discordapp.net/stickers/1039992459209490513.png" alt="Vencord Logo"/>

### Before starting

<p id="quick_css_blank_or_empty">
    Before going or reading any further, make sure that you have
    installed <format color="red">%chillax% </format>
    following the instructions given in
    <a href="Installation-guide.md">Installation Guide</a> for Vencord.
    The rest of documentation is written in regards with our recommended
    installation method.
    However, if you are using a different method such as downloading
    it from <a href="https://betterdiscord.app/theme/Chillax">BetterDiscord website</a>
    and then enabling it via theme then
    you should therefore open the theme folder
    and then open <strong>chillax.theme.css</strong> file
    using your preferred text editor
    (<i>few suggestions are <a href="https://code.visualstudio.com/">VSCode</a>, Notepad, etc.</i>)
    and edit in accordance with the below instructions.
</p>

### 1. How to change the background/background image of %chillax%?

[//]: # (<secondary-label ref="updated"/>)

The steps are first `settings`, then go to the `VENCORD` Section and then `Themes`.
Finally, click `Edit Quick CSS` which should open the integrated
[Monaco](https://microsoft.github.io/monaco-editor/) (*It's already there no need
for installation as this is part of the Vencord itself*) code editor.
Now using this Editor, you can easily edit CSS with hot reloading.
See the below-attached screenshots:

1. <img src="go_to_settings.png" alt="How to go to Settings" border-effect="rounded"/>

2. <img src="edit_quick_css.png" alt="Where to find `Edit Quick CSS`" border-effect="rounded"/>

3. <img src="monaco_editor.png" alt="Monaco editor" border-effect="rounded"/>

Now to go to line number `50` (*at the time of writing, the line number
is 50 which in a later version might change*) or where the variable `--wallpaper`
defined and change the url that is within the single quote `""`
to the **wallpaper**/**gif** **cdn url** that you want to set.

> After opening the `Edit Quick CSS` it is all blank or empty?
> Please check out the detailed [installation instructions](Installation-guide.md) on
> how to install %chillax% the recommended way or follow [this reference](#before-starting).

{style="tip"}

See the below screenshots:

<img src="bg_change.png" alt="The place where to change the url" border-effect="rounded"/>

Now your favourite background image/gif should be applied.
Moreover, if you need to control the opacity of the background,
please adjust the CSS variable `--bg-opacity`.

> If you’re getting an image from the web, make sure that it is a 
> image CDN link and **not the webpage itself**.
> Best way to get the image CDN link from the web is to
> right-click on the image and then select `Open image in new tab` option
> from your browser.
> 

{style="warning"}



> **Note**: If you’re using discord CDN, they expire after some time.
> For this the background may suddenly become black, or it might start
> blinking or shaking.
> In such cases fetch a new link or download the image and host it
> somewhere like GitHub.

{style="note"}

#### Procedure to host images on GitHub:

<procedure title="To host image on GitHub" id="github-image-hosting-process">
   <step>
      First create a public GitHub repository with the name of your choice.
  </step>
   <step>
      Once done creating the repository, add image(s)/gif(s) via the <ui-path> Add File > Upload Files</ui-path>.
  </step>
   <step>
      After image uploading commit the changes and go back to the repository.
  </step>
   <step>
      Now click on the image/gif that you want to set and this will take
      you the image/gif which is now hosted on GitHub.
  </step>
   <step>
      After that right-click (mouse)
      on the image and then click on <format style="bold">Open image in a new tab</format>.
  </step>
   <step>
      Finally, copy the URL/Link from the browser and paste into the appropriate CSS Variable
      described/shown earlier.
  </step>
   <p>Congratulation! Now you know how to host images on GitHub.</p>
   <p>This process not only applies to image/gif but also for virtually anything including fonts etc.</p>
</procedure>

> **Note**: If the link is not working or the image is not showing up,
> then please make sure that the link that you're using is the RAW GitHub link.
> A typical raw GitHub link would look like `https://raw.githubusercontent.com/{username}/{repositoryname}/{branchname}/{path_to_your_file}`.
> Notice that the link starts with `https://raw.githubusercontent.com` and then it will be
> followed by a `\` and then your `username` etc.
> For instance, here is an example of %chillax% logo 
> hosted on GitHub `https://raw.githubusercontent.com/Chillax-ORG/Images/main/mainredlogo.png`.

{style="note"}

### 2. How to change/use another font(s)?

[//]: # (<secondary-label ref="updated"/>)

First, make sure that the font you're trying to
use is already hosted somewhere if it is not already.
Most of the time you will be using [google fonts](https://fonts.google.com/).
From there, choose the font you're looking for and adjust all the settings
and everything (*font weights, size, etc.*) and then copy the CSS import url.
See the below screenshots:

1. <img src="font_change_1.png" alt="Search for a font that you like" border-effect="rounded"/>

2. <img src="font_change_2.png" alt="Click on `Get Font`" border-effect="rounded"/>

3. <img src="font_change_3.png" alt="Now click on get embedded code" border-effect="rounded"/>

4. <img src="font_change_4.png" alt="Select the CSS Import Option" border-effect="rounded"/>

5. <img src="font_change_5.png" alt="Now it should look something similar to the way it is shown" border-effect="rounded"/>

6. <img src="font_change_6.png" alt="Copy the CSS import url and notice the font name" border-effect="rounded"/>
    * Only copy the highlighted part.
      In your case, the link can be different.
7. <img src="font_change_7.png" alt="Now paste the copied link at the very top as shown"/>
    * Now go to <ui-path> Settings > Themes > Edit Quick CSS</ui-path>.
    * Paste the copied link at the top just like the above screenshot and put the `;` at the end of it.
8. <img src="font_change_8.png" alt="Change the font name"/>
    * Now change the `--font-name` to the name of the font that you have
      just imported.
    * Optionally adjust the `--font-size` if you need to.

> If the font is not working correctly, then double-check
> the font name that you've provided in Step 8.
> Please make sure that the font name is the same as shown by Google Font
> during Step 5 and 6 (the font name that was shown to you when you followed Steps 5 and 6).

{style="warning"}

And now the new font(s) should be applied.

#### Alternatively, if you want to use a downloaded font: 

* Host the font somewhere. [GitHub](https://www.github.com) is a good place.

* For GitHub, all you have to do is create a new repo and upload the font there.

* The process on how to host a font on GitHub is very similar to
  the described procedure [here](#procedure-to-host-images-on-github).

* After clicking on the font file, right-click (*mouse*) on the <ui-path>RAW</ui-path> button
  located in the right corner and then click <ui-path>Open link in a new tab</ui-path> button.
  Finally, copy **RAW** GitHub URL/Link.

* Now just like in the previous Step 7, we import the font, but this time
  use the **RAW** GitHub link instead of the Google font approach.
  See the below for comparison:

```css
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
```

instead, it will be

```css
    @font-face {
    font-family: "Font Name"; /* Replace with the name of the font here */
    src: url("RAW GitHub Link"); /* Replace with the hosted github raw link */
}
```

### 3. How to change the font size?

* Go to <ui-path> Settings > Themes > Edit Quick CSS</ui-path>.

* Find the CSS Variable `--font-size` and change it to your needs.

That's it.

### 4. How to change the accent color (*The Below **RED** thing/part* see attached screenshot)?

<img src="mention_stuff.png" alt="Accent color" border-effect="rounded"/>

* Go to <ui-path> Settings > Themes > Edit Quick CSS</ui-path>.

* Find the CSS Variables `--accentcolor`, `--accentcolor2` and change them to your needs.

* You may want to play around with them to find the right balance.

> Must-need to change both for it to take full effect.
>
> **Note**: `--accentcolor` is for [rgb](https://rgbcolorpicker.com/) and `--accentcolor2` is
> for [hex](https://colors-picker.com/hex-color-picker/).

{style="warning"}

### 5. How to change the theme welcome username?

* Go to <ui-path> Settings > Themes > Edit Quick CSS</ui-path>.

* Find the CSS Variables `--user-name` and change it.

### 6. How to make it so that desktop `wallpaper/wallpaper engine's` wallpaper is visible through?

<primary-label ref="advanced-users-only"/>
<secondary-label ref="experimental"/>
<secondary-label ref="wip"/>
<secondary-label ref="updated"/>

> **This is currently broken on Vencord

{style="warning"}

> **We recommend you to not go for that**

{style="warning"}

However, if you've decided to make up your mind, then

* Go to <ui-path>Settings > Vencord > Enable Window Transparency</ui-path> and turn it on.

* Now <ui-path> Settings > Themes > Edit Quick CSS</ui-path> and remove the `--wallpaper` CSS Variable
  mentioned in [here](#1-how-to-change-the-background-background-image-of-chillax).

* Your window should now be `transparent` or `see through` etc.

* Now you may want to add a bit of blur to make things readable in the `container__037ed`.
  However, discord uses electron, and we've found it to work differently on different
  OS, and the window manager of your OS also plays a vital role here.
  So, the below CSS snippet may or may not work properly (*Translucence is enabled in
  window manager level*).
  In case it does not work, it will at least make the `container__037ed`
  basically that region a bit darker.

  ```css
    .container_c48ade {
        background-color: rgba(255, 255, 255, 0) !important; /* Semi-transparent white for light theme */
        /* Or use this for dark theme: background-color: rgba(0, 0, 0, 0.1); */
        backdrop-filter: blur(1px) !important; /*Blur the background*/
        border-radius: 10px; /* Rounded corners */
        /* Or use this for dark theme: border: 1px solid rgba(0, 0, 0, 0.2); */
        box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37) !important; /* Optional: Add a box shadow for depth */
    }
  ```

> **Note**: *Linux users this may be a hit or miss due to infinite number of factors
> (Too many DEs, WMs & Display Protocols).*
> But using WM, you can **natively add/force** translucence
> at window level
> (i.e., [hyprland](https://hyprland.org/),
> [qtile](https://qtile.org/), [KWin](https://userbase.kde.org/KWin), etc.),
> and you won't have to do any of the above-mentioned things.

{style="note"}


### 7. How to change the font of the group chat?

* We have already mentioned how you can import a custom font and
  use it [here](#2-how-to-change-use-another-font-s).

* Now, the steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* After that, find the CSS variable `--group-chat-font` and provide the font name 
  that you like to use within `" "` (double quote).

* Make sure that the font that you're trying to set is available in the theme context.

### 8. %chillax% is laggy or slow, very slow, any fix?

<secondary-label ref="updated"/>

* Make sure that **Hardware Acceleration** is on.
  If not, then turn it on.

* The steps are first `Settings`, then `Advance` and then turn on `Hardware Acceleration`.

#### *Almost 99% of the time this is the reason behind lag.*

If you're **not** on a very low-end system with limited hardware acceleration support,
the theme should work fine without any lag.

However, as a last resort you can

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* [Uncomment](https://developer.mozilla.org/en-US/docs/Web/CSS/Comments) line `41` different/or which
  says `/*@import url("https://warrayquipsome.github.io/Chillax/Addons/SimpleLessLag.css");*/`
  See the below screenshots:

1.  <img src="lag_stuff_1.png" alt="Uncomment the shown line (CSS code)" border-effect="rounded"/>

    * Uncomment this line, and it should look something like the below
      screenshot:

2.  <img src="lag_stuff_2.png" alt="Uncomment the shown line (CSS code)" border-effect="rounded"/>

* This should make it a little less laggy.

Consequently, you can try out [OpenAsar](https://openasar.dev/), which is part
of the [Vencord installer](https://github.com/Vencord/Installer/issues/11).
This should make Discord a bit more performant, reducing the lag by a bit.

### 9. How to make the member list always stay visible instead of on hover?

[//]: # (<secondary-label ref="updated"/>)

This is basically an addon; to remove it:

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `33` and maybe different in your case*) containing
  `@import url("https://warrayquipsome.github.io/Chillax/Addons/AvatarOnlyMemberList.css");`.
  Now the member list will always be visible instead of on hover.
  See the below screenshots:

1.  <img src="always_visible_member_list.png" alt="CSS import that styles the member list" border-effect="rounded"/>

    * Now remove/comment out this line.

2.  <img src="commented_out.png" alt="Comment out this line as shown" border-effect="rounded"/>

    * Finally, you should have something like this:

3.  <img src="results.png" alt="Always visible member list" border-effect="rounded"/>

### 10. How to get back the old emojis?

[//]: # (<secondary-label ref="updated"/>)

This is also very similar to the previous [FAQ](#9-how-to-make-the-member-list-always-stay-visible-instead-of-on-hover).
This thing is also an addon.
Remove it to get back default emojis:

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `29` and maybe different in your case*) containing
  `@import url("https://mwittrien.github.io/BetterDiscordAddons/Themes/EmojiReplace/base/Microsoft.css");`.

* Now you should have the old emojis.

### 11. How to get rid of the Folder Icons and Make it like the old discord?

[//]: # (<secondary-label ref="updated"/>)

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `34` and maybe different in your case*) containing
  `@import url("https://warrayquipsome.github.io/Chillax/Addons/FolderRedesign.css");`.

* Now it should be normal like the old Discord.

### 12. How to get rid of the Radial Status/Ring around the user profile picture/image?

[//]: # (<secondary-label ref="updated"/>)

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `35` and maybe different in your case*) containing
  `@import url("https://discordstyles.github.io/RadialStatus/dist/RadialStatus.css");`.

Now, it should be similar to the default discord style with slight drop shadow around the
transparent images.

### 13. How to get rid of the Friend Grid?

[//]: # (<secondary-label ref="updated"/>)

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `36` and maybe different in your case*) containing
  `@import url("https://warrayquipsome.github.io/Chillax/Addons/FriendGrid.css");`.

Now the friend grid should be similar to the default Discord.


### 14. How to use Dark/Light mode in %chillax% Theme?

You can enable `Dark` or `Light` mode from the Discord Settings.
Steps are:

* Now go to `Settings` > `Appearance`.

* Finally, choose either Light mode or Dark mode based on your preference,
  and Chillax will reflect that.

### 15. After applying the Chillax theme, it looks funny and/or transparent/see through background is missing, what to do?

Before applying the theme:

* Firstly, make sure that there is **no custom** CSS or CSS snippet(s) is/are running.

* Secondly, make sure that **no third party** plugin or any **plugins** in general related to theming
  are running (*if debugging, disable all plugins for quicker conclusion*).

* Thirdly, `Settings` > `Appearance` is set to either **Dark** or **Light** mode.

* Now apply the Latest version
  of [Chillax](https://raw.githubusercontent.com/warrayquipsome/Chillax/main/chillax.theme.css)
  which is currently %current_version%.

* Now you should have %chillax% with the default look and feel.

### 16. How to get rid of the mobile icon beside the avatar?

[//]: # (<secondary-label ref="updated"/>)

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now go to the line `101` or find the line that says `--rs-phone-visible: block;` and
  change this line to the below line:

    ```css
        --rs-phone-visible: none;
    ```

* Now mobile icon or phone icon should be gone.

### 17. How to get back the default discord color for urls and links?

<secondary-label ref="newly-added"/>

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* **Remove** or **comment out** the line (*currently line number `37` and maybe different in your case*) containing
  `@import url("https://warrayquipsome.github.io/Chillax/Addons/ColoredLinks.css");`.

Now the urls and links should have the default discord like styles and colors.


### 18. How to change the color of every urls and links in discord?

<secondary-label ref="newly-added"/>

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now apply the below CSS snippet, which will change the color of every
  url to the color of your choice.

```css
    [href^="http://"], [href^="https://"], [href^="www."] {
    color: #30d944 !important; /* change it to whatever you like */
}
```

### 19. How to change the input placeholder value from "*Life is so much easier when you just take a moment to chill*" to something that I want?

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now find the CSS variables `--chillax-input-field` and `--chillax-input-field-locked`.

* Change them according to what you like most. 

> CSS variable `--chillax-input-field` and `--chillax-input-field-locked`
> provided for fine-grained control over the locked and unlocked channel input placeholder text.

{style="note"}


### 20. How to change the Avatar Only Member list's rounder corner/border radius?

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now find the CSS variable `--memberlist-border-radius` and change the pixel as per your preference.

* If you don't like the border radius and want it to be a rectangle, set the value to `0 px`.

> Note the value must end in `px` or `rem` or `em`.

{style="note"}


### 21. How to change the typing indicator text?

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now find the CSS variables `--chillax-input-typing-indicator-one-person` and `--chillax-input-typing-indicator-many-person`.

* Change them according to what you like most.

> CSS variable `--chillax-input-typing-indicator-one-person` and `--chillax-input-typing-indicator-many-person`
> provided for fine-grained control over the number of persons typing at a time.
> Customize them however you please.

{style="tip"} 

### 22. How to get back the scroll wheel/scroller/scrollbar in %chillax%?

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Now find the CSS variable `--chillax-scroller-color` which is by default set to `transparent`.

* Change it to a [hex](https://colors-picker.com/hex-color-picker/) color of your choice,
  and the scrollbar/scroll wheel should appear.

> In some places, the scroll wheel/scrollbar is hidden until you hover over.
> 
{style="note"}


### 23. How to make the `Mute` and `Headphone` icon always stay visible even when not hovering over user control?

<secondary-label ref="updated"/>

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

*  Now paste the below CSS snippet:

```css
/* Mute and Headphone icon always stays visible even when not
   hovering over user control */
.panels_c48ade .buttons__37e49:hover > * {
    opacity: 1 !important;
}
```

* Now the mute and headphone icon should always be visible.

### 24. How to hide annoying elements such as nitro, shop, sticker picker etc. tab?

<secondary-label ref="updated"/>

* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* [Uncomment](https://developer.mozilla.org/en-US/docs/Web/CSS/Comments) line `43` different/or which
  says `@import url("https://warrayquipsome.github.io/Chillax/Addons/HideAnnoyingElements.css");`.

Now those annoying tabs and such will disappear.

### 25. How to change the spotify progress squid/progress bar GIF to a custom one?

<secondary-label ref="newly-added"/>


* The steps are first `Settings`, then go to the `Themes` Section and then `Edit Quick CSS`.

* Find the CSS variable `--chillax-spotify-control-squid-gif-url` (_at the time of writing, the line number
is **134** which in a later version might change_) and change the url/link
  to your GIF that you are trying to set.

* After that make sure to adjust the `--chillax-spotify-control-squid-width` and
  `--chillax-spotify-control-squid-height` accordingly if the GIF seems out of place.


## Still Have Question(s)?

Join our support
<format color="#ffA36b">
        [Discord Server](https://discord.com/invite/DrfX6286kF)
</format>
and ask for help and don't be <control>shy</control>.
