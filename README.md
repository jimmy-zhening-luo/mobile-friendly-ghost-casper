# mobile-friendly-ghost-casper
Casper is the default, and most-widely used theme for the Ghost blog/website platform. By default, Casper's site navigation bar appears cut off on smaller screens, such as mobile devices. (On content pages, the navigation bar is almost entirely missing on sites with longer logos, since the navigation bar is stuck on the same line as the logo.) Although the user can scroll to the right with their fingers (or drag the text, if on a smaller PC screen), there is no affordance indicating that is possible, and the result is inelegant, often resulting in lopped off text, or even worse, missing menu options.

This is a modified, mobile-friedly Casper theme for Ghost to fix issue where the navigation bar is cut off when viewing a site on small screens (e.g. mobile devices). Small fix to theme .css that works across all Ghost page types. Now, when the screen is smaller, the navbar wraps around to a second line and centers itself, rather than cutting off. Works on all supported browsers/devices, scales smoothly for all possible width ranges (tested from 200px to 2400px wide).

I noticed this issue when booking an appointment with one of my healthcare providers; their "Contact Me" button happened to be the last button on their navigation bar, and was consistently cut off on every single page when I was visiting the site on my phone. They're an awesome provider and I wanted to make sure patients could reach them, so I pumped out this fix for them in a couple hours. I hosted this on my own Ghost/Casper instance and tested across multiple browsers, platforms, screen sizes, and versions of Ghost/Casper, and it seems to work great. They are not technical, but were able to easily deploy the modified theme package to their Ghost site through their content management portal. They loved the result, so I wanted to share the code for anyone else who uses Casper and runs into this problem.

## Replace your existing theme with Friendly Ghost Casper (easy)
### Download required project files
1. Download original, unmodified Casper theme here:
  1. 2.8.1 (latest as of 1/12/2019): https://github.com/TryGhost/Casper/releases/tag/2.8.1
  2. 2.0.2 (older): https://github.com/TryGhost/Casper/releases/tag/2.0.2
2. In this repository, download <release>\built\screen.css

### Modify default Casper theme to be friendly
1. Extract Casper-<release>. (For this example, using 2.8.1.)
2. Go to Casper-2.8.1\assets\built
3. Replace Casper-2.8.1\assets\built\screen.css with this repository's 2.8.1\built\screen.css

### Apply Friendly Ghost Casper theme to site 
1. Re-zip the modified Casper-2.8.1 folder (to .zip).
2. Go to site's Ghost admin panel -> Settings -> Design -> Installed Themes -> "Upload a theme".
3. Select the modified Casper-2.8.1.zip
4. Click "Activate Now" to apply the new theme to site immediately.

## Newer version of Casper? Making an arbitrary or future version of Casper friendly
### Download required project files
1. Download original, unmodified Casper theme here (whichever version you want): https://github.com/TryGhost/Casper/releases
2. In this repository, download mobile-friendly.css

### Modify default Casper theme to be friendly
1. Extract Casper-<release>.
2. Go to Casper-<release>\assets\built
3. Edit Casper-<release>\assets\built\screen.css
4. Open mobile-friendly.css from this repository.
5. Append the contents of mobile-friendly.css to Casper-<release>\assets\built\screen.css
6. (Optional) Re-minify the contents of Casper-<release>\assets\built\screen.css (with the appended mobile-friendly.css). Use a minifier that supports the latest CSS standards, i.e. https://www.cleancss.com/css-minify/
7. Save Casper-<release>\assets\built\screen.css

### Apply Friendly Ghost Casper theme to site 
1. Re-zip the modified Casper-<release> folder (to .zip).
2. Go to site's Ghost admin panel -> Settings -> Design -> Installed Themes -> "Upload a theme".
3. Select the modified Casper-<release>.zip
4. Click "Activate Now" to apply the new theme to site immediately.
