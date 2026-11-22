# Session Handoff: Webb Family Georgia Thanksgiving Adventure

**Handoff Saved:** 2026-11-22 15:00 CT
**Repo:** https://github.com/jordanwebb10/georgia-thanksgiving-adventure
**Live Site:** https://jordanwebb10.github.io/georgia-thanksgiving-adventure/
**Travelers:** Jordan Webb, Janie Gittelson, and Winston (`70 lb` black-and-white Shepherd Mix, pointy ears, white blaze, speckled muzzle, red-green-cream plaid bandana, favorite yellow-orange spiky ball)
**Trip Window:** Chicago farewell (Sun Nov 22 to Mon Nov 23) -> Road Trip (Tue Nov 24 to Fri morning Nov 27, 2026) -> Move-In at Peachtree City, GA

---

## 1. What Is Already Completed & Live
1. **Storybook Website V4 Live on GitHub Pages (`main` branch, commit `c47dae4`):**
   - **11 custom hand-inked watercolor comic panels** (`images/00-splash-three-faces` through `images/11-aggie-winston-finale`, both `.webp` and `.jpg`):
     - `00`: 3-faces circular splash cover & hero medallion
     - `01` to `06`: Hero road trip, Franklin Main St, Chattanooga bridge, Trilith feast, Welcome Home PTC, Georgia trails
     - `07`: Night 1 cozy Indiana hotel pit stop
     - `08`: Franklin Harlinsdale Farm coffee & Winston zoomies
     - `09`: Chattanooga Lookout Mountain panoramic vista
     - `10`: Sunny Friday morning lattes & croissants in Town at Trilith
     - `11` (`#aggie-finale`): Post-Credits Bonus Panel of Aggie & Winston sitting together in the sunny Georgia autumn backyard (ear scratches + spiky ball)
   - **35-second HD Mini-Movie Trailer** (`webb-georgia-adventure.mp4`, `1280x720`, 24 fps, H.264 + acoustic Rhodes soundtrack).
   - **Fixed Interactive Map (33 Starred Stops):** Switched from broken CARTO tiles to zero-API-key Esri World Street Map + Esri World Topo Map toggle.
   - **Shared Packing Checklist (`41` items across 6 categories):** Backed by `checklist.json` and `PACKING_LOG.md`, with custom item add forms and `All` / `Unpacked Only` filters.
   - **Monday Morning, Nov 23 Farewell Breakfast Added:** **Lula Cafe** (`2537 N Kedzie Blvd`, Logan Square, `9:00 AM to 3:00 PM`, walk-in only, closed Tuesdays) added to Chapter 1 timeline (`#day-1`).
   - **Night 3 Confirmed Banner:** Trilith Guesthouse suite stay & Prologue Thanksgiving Feast marked **CONFIRMED & UPGRADED!** on the public page (private booking IDs and rates intentionally kept out of this public repo).
   - **Legacy Work Worker Removed:** Old U.S. Soccer Cloudflare Worker (`georgia-thanksgiving-adventure`) was deleted cleanly so personal and work infrastructure stay separated.
2. **Aggie Character & WhatsApp Lookbook Continuity:**
   - Persona name: **Aggie** (`Antigravity -> AGY -> Aggie`), sassy, warm, chic little cream-ivory & sage-green robot with dark glass visor, amber eyes, tortoiseshell sunglasses on her head, terracotta-orange silk neck scarf, and brass ear accents.
   - Janie asked `"What would a chic little robot look like?"` and received a 3-look watercolor lookbook (Look 1: Parisian Cafe Chic; Look 2: Georgia Boutique Chic; Look 3: Celestial Pearl & Rose-Gold) plus a playful foot-tapping mid-wardrobe limbo comic nudge.
   - Local WhatsApp watcher was cleanly stopped by Jordan at 2:53 PM CT (Nov 22).

---

## 2. Open Tasks Ready to Pick Up in Cloud Mode

### A. Lock Down the GitHub Pages Site with a Shared Passcode (GitHub-Only)
- **Jordan's preference:** Wants to stay strictly on **GitHub** (no extra Cloudflare/Vercel accounts) with a passcode/code only he and Janie know.
- **Important GitHub limitation already briefed:** Free and Pro GitHub Pages have no native server-side password login (only GitHub Enterprise Cloud supports private GitHub Pages).
- **Recommended GitHub-only implementation (pending Jordan's passcode & asset preference):**
  - Build a clean **Web Crypto AES-256-GCM encrypted** `index.html` gate (same zero-server cryptography as StatiCrypt): displays a cozy storybook `"Enter Our Family Passcode"` unlock screen, derives the AES key in-browser via PBKDF2, decrypts the full storybook content on match, and saves unlock state locally on Jordan & Janie's phones (with `<meta name="robots" content="noindex, nofollow">` added).
  - Clarify with Jordan before implementing:
    1. Exact passcode (or placeholder so he can run/set it cleanly), and
    2. Whether he wants **HTML text/itinerary encrypted** (fast, ~5 min) OR **images encrypted too** (and note that Git history in the current public repo would still retain old unencrypted commits unless rotated to a fresh repo).

### B. Night 1 (Tue Nov 24) & Night 2 (Wed Nov 25) Hotel Bookings (70 lb Dog Friendly)
Still need final booking confirmation from Jordan (never enter credit card info automatically; prep links/details cleanly):
- **Night 1 (Tue Nov 24 to Wed Nov 25, South Indy / I-65 S):**
  - Top value pick: **La Quinta Inn & Suites Columbus - Edinburgh** (`101 Carrie Ln`, I-65 Exit 76B, trims 25 min off Day 2, `4.2★`, `75 lb` max, `$25` pet fee, free hot breakfast, `~$116 to $125` all-in). *(Note: automated browsers hit Akamai 403 on wyndhamhotels.com; give Jordan direct URL or Booking.com free-cancel fallback.)*
  - Exit 99 alternative: **Best Western Plus Greenwood** (`1281 S Park Dr`, `4.2★`, `80 lb` max, `$25` pet fee, `~$116 to $144` all-in).
  - Avoid: La Quinta Indy South (`50 lb` conflicting cap), HIE Greenwood (no pets), Residence Inn / Hampton Inn Greenwood (`50 to 60 lb` cap).
- **Night 2 (Wed Nov 25 to Thu Nov 26, Franklin, TN):**
  - Clear winner: **Candlewood Suites Nashville - Franklin** (`1305 Murfreesboro Rd`, `2.2 mi` / 5 min to Main St, `4.5★`, `80 lb` max, `$75` pet fee, full kitchen, free cancel on Best Flexible, `~$167` OTA / `~$192` direct all-in; Studio King `385 sq ft` or 1-BR Suite `625 sq ft`).
  - Critical catch to remember: **Drury Plaza Franklin** prohibits leaving dogs unattended in rooms AND requires **stairwells only (no elevators)** for dogs. Avoid La Quinta Franklin (`3.1★`, `60 lb` cap).
- **Night 3 (Thu Nov 26 to Fri Nov 27, Trilith Guesthouse & Prologue Thanksgiving Feast):**
  - **ALREADY CONFIRMED** (suite upgrade + Thanksgiving feast arranged; reminder for Jordan to verify in his Marriott Bonvoy app that his personal card, not work card, is attached).

### C. Chicago Farewell Omakase Dinner
- Jordan confirmed he wanted **Omakase Box** (`3038 W Armitage Ave`, Logan Square).
- **Schedule catch:** Omakase Box is **CLOSED Mondays and Tuesdays**, **OPEN tonight Sunday Nov 22 (`4:30 PM to 9:00 PM`)** via Tock: https://www.exploretock.com/omakaseboxchicago (`$98` 15-course counter at `5:30/5:45/7:30/7:45 PM`, `$59` 11-course express at `4:30/4:45 PM`, `$65` dining room omakase).
- **Monday night (Nov 23) open backups if skipping tonight:**
  - **Sushi by Bou (Fulton Market, The Emily Hotel, `311 N Morgan St`)**: Open Mon `5:00 PM to 11:00 PM`.
  - **Tanoshii West Loop (`720 W Randolph St`)**: Open Mon `4:30 PM to 9:45 PM`.
  - **Izakaya Shinya (`2255 W North Ave`, Logan Square / Bucktown)**: Open Mon `5:00 PM to 2:00 AM`.
- **Awaiting Jordan's choice** on Sunday tonight vs. Monday night backup.

### D. Waiting on Janie's Lookbook Verdict
- Whenever Jordan shares Janie's pick from the Chic Little Robot Lookbook (Look 1, Look 2, Look 3, or a remix), generate Aggie's official finalized mascot portrait matching her verdict!

---

## 3. Private Details Stored Off-Repo (Do Not Commit Here)
Full private relocation records (Trilith confirmation number, Marriott Bonvoy ID, staff/realtor phone numbers, 21-contact `.vcf`, executed 306 Calgary Drive lease PDF, Rocket Mortgage payoff quote, and local `Downloads` cleanup confirmation list) remain strictly in Jordan's local Obsidian vault (`03 - Spaces/Me/Efforts/Effort - ATL Move/`) and Google Drive.
