# Waukesha-Pearce Industries × HubSpot — Executive Briefing

Single-file static page. No build step. `index.html` is the whole thing.

## Run it locally (for presenting live)
Open `index.html` in Chrome and go full screen (Cmd+Shift+F). Arrow keys or
scroll move through the 10 sections. Needs internet only for fonts — see
"Offline" below if venue wifi is unreliable.

## Deploy to Vercel
From this folder, with the Vercel CLI logged in:

    vercel            # first run, creates the project
    vercel --prod     # promote to the live URL

No CLI? Drag this folder into vercel.com (Add New > Project), or use Netlify
Drop (app.netlify.com/drop) for an instant link. The screenshot images must
sit in the same folder as index.html either way.

## Narrative spine
One shift (measure revenue, not activity), then three wins.

    01 Open ............. the shift
    02 Today vs Next .... neutral before/after
    03 The Big Idea ..... one change, three wins
    04 Foundation ....... revenue attribution (HERO)
    05 Win 1 ............ spend smarter (+ QR proof point)
    06 Win 2 ............ close faster (visitor ID + handoff)
    07 Win 3 ............ reach further (AI search, light service nod)
    08 Peer proof ....... dealers already on HubSpot
    09 Pricing .......... one annual number
    10 ROI ............. real HubSpot benchmark lifts + live official calculator

## Add the screenshots
Each frame has a `.slot` placeholder with the exact `<img>` line commented
above it. Name the files as below, drop them in this folder, then swap:

    screenshot-1.png   Revenue by campaign & channel        (Image 9)
    screenshot-2.png   Closed deals + marketing influence   (Image 10)
    screenshot-3.png   Leads & traffic by channel           (Image 8)
    screenshot-4.png   Visitor / company identification     (fresh grab)
    screenshot-5.png   Automated lead handoff / workflow    (fresh grab)
    screenshot-6.png   AI search visibility ranking         (fresh grab)

Swap example:
    <!-- <div class="slot">[ SCREENSHOT 1 ]...</div> -->
    <img class="shot" src="screenshot-1.png" alt="Revenue by campaign and channel">

Logos in section 08: replace the `.logo-slot` divs the same way. CONFIRM the
three dealer names and pull real logos before presenting.

## Offline mode
Fonts load from Google Fonts. To present with no internet, self-host the three
fonts (Archivo, IBM Plex Sans, IBM Plex Mono) or fall back to system fonts.
Layout is identical either way.

## Design system
- Accent #FF5C35 (HubSpot orange), used sparingly
- Dark "machined steel" #16191D / #1C2025 with a faint blueprint grid
- Light "drafting paper" #EBEDEF, white screenshot cards
- Display: Archivo Expanded · Body: IBM Plex Sans · Data: IBM Plex Mono
- House rules: no em dashes, plain language, outcome before mechanism
