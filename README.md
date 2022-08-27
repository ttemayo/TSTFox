<br><br>

# TSTFox
Firefox custom CSS designed to remove a lot of the clutter that comes default with Firefox, with Tree Style Tabs use in mind. The main goal was to maximize screen and browser real estate.

<br>

![Preview Image showing both the one-line style and the style for smaller screensizes.](assets/preview.png)


## Features
Horizontal tab bar removal
Min, Restore, Max, Close toolbar moved to navigation row
Tabs move back on top below a certain browser width threshold

### Tabs on Top Breakpoint

Edit the `min-width` value to change the breakpoint size on which Cascade will switch to the oneline layout.

```css
@media (min-width: 1000px) {
    
    [...]
    
}
```
<br>

## How to use this userChrome.css

1. Type `about:config` into your URL bar. Click on the **I accept the risk** button if you're shown a warning.
2. Seach for **`toolkit.legacyUserProfileCustomizations.stylesheets`** and set to **`true`**.
3. Go to your profile folder:
    - Linux: `$HOME/.mozilla/firefox/######.default-release/`
    - MacOS: `Users/[USERNAME]/Library/Application Support/Firefox/Profiles/######.default-release`
    - Windows: `C:\Users\[USERNAME]\AppData\Roaming\Mozilla\Firefox\Profiles\######.default-release`
4. If it doesn't exist, create a folder called `chrome`.
5. Copy `userChrome.css` into that folder.

