# DC Stamp Hunt — NPS Passport Itinerary

A 3-day National Park Service passport-stamp trip to Washington, DC, built around the
**Passport To Your National Parks® Collector's Edition** book.

**Live site: https://harikrishnad1997.github.io/dc-stamp-hunt-trip/**

## The trip

- **Thu Nov 19 – Sun Nov 22, 2026** · Harikrishna Dev + Rajashree Chandar
- Flights: American Airlines, Chicago O'Hare (ORD) ↔ Washington Reagan National (DCA)
- Hotel: Washington Plaza Hotel, 10 Thomas Circle NW
- **Day 1 (Fri Nov 20)** — National Mall on foot, west to east: Lincoln, Vietnam,
  Korean War, DC War Memorial, MLK Jr., FDR, Jefferson, Washington Monument Lodge,
  Eisenhower (day ends ~3 PM)
- **Day 2 (Sat Nov 21)** — Downtown / Shaw / Anacostia on foot + Metro/bus: White House
  Visitor Center, Ford's Theatre (10 AM entry), Woodson Home (1:15 PM tour), African
  American Civil War Memorial, Frederick Douglass NHS (3:30 PM tour), then the rental-car
  pickup at DCA in the evening
- **Day 3 (Sun Nov 22)** — by car: Theodore Roosevelt Island, C&O Canal Georgetown,
  LBJ Memorial Grove, the Pentagon 9/11 Memorial (on foot), Arlington Cemetery
  (Arlington House — its bookstore has the LBJ Grove stamp), Georgetown (C&O Canal +
  the Old Stone House for the Rock Creek stamp), Kenilworth Aquatic Gardens, Belmont-Paul,
  Fort Washington Park (MD), then the flight home

Everything is booked (flights, hotel, all three Saturday tours, rental car). The only
open item is the **optional Washington Monument ticket** — more are released on
Recreation.gov Thu Nov 19, 2026 at 3:00 PM ET.

Good to know:

- **Mary McLeod Bethune Council House is closed for renovation** (Sep 9, 2026 –
  Jan 27, 2027). It's an exterior-only stop on Day 2; its passport stamp is at the
  Frederick Douglass NHS visitor center.
- **Parking on Day 3 is free at every stop** — NPS lots, plus DC meters are not
  enforced on Sundays (Georgetown and Belmont-Paul street parking).
- Confirmation numbers are deliberately **not** in this repo or on the public site —
  they're in the PDF itinerary and the booking emails.

## What's in this repo

| File | What it is |
| --- | --- |
| `index.md` | The full itinerary page (Jekyll source for the live site): day plans, bookings summary, live weather widget, stamp + brochure + packing checklists, NPS stamp-location reference, America 250 stamp checklist |
| `map.html` | Standalone interactive map (Leaflet + OpenStreetMap): every stop as a numbered pin, color-coded by day, filterable by day via the layer control, with Day 3 parking pins and a layer of every visitor center / stamp desk |
| `_config.yml` | Jekyll theme config (`jekyll-theme-cayman`) |

The weather section on the site is a small live widget using the free
[Open-Meteo](https://open-meteo.com) API (no key) — it refreshes on every page open
and highlights the trip days once they're inside the 10-day forecast window.
Photos are Wikimedia Commons images (public domain / Creative Commons), hotlinked
with credits at the bottom of the page.

## Publishing notes

- The repo is **private**, but the GitHub Pages site is **publicly viewable** by
  anyone with the link.
- Pages is configured as **Deploy from a branch → `main` → `/(root)`** (repo
  Settings → Pages). If the site ever returns 404, check that setting first —
  on Oct 23, 2026 the source was accidentally set to "None," which unpublishes
  the site; re-selecting `main` restored it.
- To update the itinerary, edit `index.md` (and `map.html` for the map) and push to
  `main`; Pages rebuilds automatically in about a minute.
