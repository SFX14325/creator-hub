# Creator Hub V1
Static GitHub Pages site. Upload index.html, style.css, config.js and app.js to the root of a new public repository. In Settings > Pages, select Deploy from a branch, main, / (root). Open the URL GitHub provides.

Edit config.js for profile, social links, clips and weekly schedule. Empty URLs are non-clickable placeholders. For YouTube Shorts, paste only the video ID from youtube.com/shorts/VIDEO_ID into video_id. Videos must allow embedding. Use relative image paths such as assets/avatar.png and upload those files. Schedule day 0 is Monday, 6 is Sunday. Times are manually entered in the configured timezone, not automatically converted. Edit CSS variables in style.css for colors. The side background is a CSS pattern; replace its background-image with your own repeating image if desired.

Open index.html locally for a preview. Actual YouTube playback requires internet access and may require serving the page over HTTP rather than file://.
