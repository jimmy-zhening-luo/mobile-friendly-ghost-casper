# mobile-friendly-ghost-casper
Modified, mobile-friedly Casper theme for Ghost to fix issue where the navigation menu bar is cut off when viewing a site on small screens (e.g. mobile devices). Small fix to theme .css that works across all Ghost page types. Now, when the screen is smaller, the navbar wraps around to a second line and centers itself, rather than cutting off. Works on all supported browsers/devices, scales smoothly for all possible width ranges (tested from 200px to 2400px wide).

## Replace your existing theme with Friendly Ghost Casper
### Download required project files
1. Download original, unmodified Casper theme here:
a. https://github.com/TryGhost/Casper/releases/tag/2.0.2
2. Download screen.css and minified.screen.css from this repository.

### Modify default Casper theme to be friendly
1. Extract Casper-2.0.2.
2. Go to Casper-2.0.2\assets\css
3. Replace Casper-2.0.2\assets\css\screen.css with this repository's screen.css
4. Go to Casper-2.0.2\assets\built
5. Replace Casper-2.0.2\assets\built\screen.css with this repository's minified.screen.css
6. BE SURE TO RENAME 'minified.screen.css' to 'screen.css' within Casper-2.0.2\assets\built\

### Apply Friendly Ghost Casper theme to site 
1. Re-zip the modified Casper-2.0.2 folder.
2. Go to site's Ghost admin panel -> Settings -> Design -> Installed Themes -> "Upload a theme".
3. Select the modified Casper-2.0.2.zip
4. Click "Activate Now" to apply the new theme to site immediately.
