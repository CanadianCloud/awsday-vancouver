# AWS Community Day Vancouver

City of Builders website for https://canadiancloud.org/awsday-vancouver/.

Planned custom domain: https://vancouver.awsday.ca.

## Preview

Serve this directory with any static HTTP server, for example:

```sh
python -m http.server 8080
```

No framework, package installation, build step, tracking or backend is required.

## Content

`index.html` contains editable, accessible page content and dialog panels. Shared appearance lives in `styles.css`; `app.js` handles navigation and native dialogs. Images and locally hosted fonts live in `assets/`. All paths are relative, so the site also works under the GitHub project path.

Dates, venue, speakers and programme are deliberately unconfirmed. Every Get updates link opens the Vancouver group's events page: https://luma.com/awsvan. Volunteer, speaker and sponsorship enquiries open the visitor’s email app addressed to the published info@awsday.ca contact.

To publish confirmed details, replace the corresponding panel and hero copy, and point the updates CTA at the confirmed registration URL. Update canonical, social metadata, sitemap and CNAME if the domain changes.

## Hosting

GitHub Pages serves `main` from `/`. The custom domain `vancouver.awsday.ca` is set in `CNAME`, with DNS pointing to `canadiancloud.github.io`.

## Assets

City artwork was generated for this design. Community photo reused from CanadianCloud/awsday.github.io, public/Instagram/ig3.jpg, and captioned as a past Canadian community event. Nunito is licensed under the SIL Open Font License; see assets/OFL.txt.

## Past Vancouver events

The homepage footer links to `past-events/`. Local archive copies are stored at `past-events/2024/`, `past-events/2025/`, and `past-events/2026/`. The 2024 and 2025 copies preserve the original static exports, including linked schedules, speakers, photographs and maps. Redundant nested archives and unused source fonts are excluded; fonts served by each archive are kept in its `_next` resources.

The 2026 export was built from CanadianCloud/awsday.github.io commit `e3238b0177c67a8b073750cf0ff72b57609ffbd3` with Vancouver as the default view and base path `/past-events/2026`. It preserves the original event content, including the Vancouver schedule and interactive Science World map. The old live website was not modified.

Shared `past-events/archive.js` and `archive.css` add a historical notice, keep legacy internal navigation within each archive, and close historical signup controls. Each year has `provenance.json` with source URL, capture date, original HTML hash and event date. Add future years to the archive index without overwriting existing year folders.
