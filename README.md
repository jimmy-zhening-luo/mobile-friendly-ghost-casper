# mobile-friendly-ghost-casper
Casper is the ubiquitous, default theme for Ghost, a blog/website suite. Out of the box, Casper's site navigation bar is cut off on smaller screens, like mobile devices, making some buttons unusable. This is a small, self-contained CSS fix to wrap and center long navbars on small screens. Works on all page types, browsers, and screen widths.

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
