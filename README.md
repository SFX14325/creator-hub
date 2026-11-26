# Creator Hub v1.0

Static website, separate from Knowledge Garden. All entries are fictional placeholders. No payment processing or account system.

## Deploy
Create a separate GitHub repository (e.g. creator-hub). Upload the contents of this folder to its root. In Settings > Pages choose Deploy from a branch, main, / (root). Open the Pages URL. Do not replace your Knowledge Garden repository.

## Local preview
From this folder run `python -m http.server 8000`, then open http://localhost:8000. Double-clicking index.html is not supported because browsers restrict local JSON fetches.

## Edit
- settings.json: theme colors, background path, currency (ISO code), donation URL, demo label. Set demo false only after replacing all sample data.
- data/profile.json: name, bio, about, avatar path.
- data/socials.json: name and external URL; blank URLs are disabled.
- data/clips.json: title, YouTube video ID (11 characters, from a Shorts URL), thumbnail path. Blank IDs show placeholders. Playback requires internet and embeddable videos.
- data/schedule.json: timezone label and events with full English weekday, time, type, title. Times are displayed as entered, not converted.
- data/donations.json: public display name, cumulative total_amount (number), donation_count (number). Ranking and total are calculated automatically. Publish only with supporter permission. Use anonymous entries as appropriate.
- data/merchandise.json: title, description, optional numeric price, image, URL, status. Blank URL displays a non-clickable status.
- assets/: replace placeholder SVGs or add your own images and update paths. Paths are relative to the site root. Use HTTPS links.

The two side panels remember their expanded state locally. On small screens they become collapsible sections above the main content, closed by default. Clips scroll horizontally and load YouTube only when selected. No build step or external dependencies.
