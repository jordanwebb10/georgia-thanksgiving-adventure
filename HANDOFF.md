# Session Handoff: Webb Family Georgia Thanksgiving Adventure

**Handoff Saved:** 2026-11-22 15:00 CT
**Repo:** https://github.com/jordanwebb10/georgia-thanksgiving-adventure
**Live Site:** https://jordanwebb10.github.io/georgia-thanksgiving-adventure/
**Travelers:** Jordan Webb, Janie Gittelson, and Winston (`70 lb` black-and-white Shepherd Mix, pointy ears, white blaze, speckled muzzle, red-green-cream plaid bandana, favorite yellow-orange spiky ball)
**Trip Window:** Chicago farewell (Sun Nov 22 to Mon Nov 23) -> Road Trip (Tue Nov 24 to Fri morning Nov 27, 2026) -> Move-In at Peachtree City, GA

---

## 1. What Is Already Completed & Live
1. **Storybook Website V5 Live on GitHub Pages (`main` branch):**
   - **11 custom hand-inked watercolor comic panels** (`images/00-splash-three-faces` through `images/11-aggie-winston-finale`, both `.webp` and `.jpg`):
     - `00`: 3-faces circular splash cover & hero medallion
     - `01` to `06`: Hero road trip, Franklin Main St, Chattanooga bridge, Trilith feast, Welcome Home PTC, Georgia trails
     - `07`: Night 1 cozy Indiana hotel pit stop
     - `08`: Franklin Harlinsdale Farm coffee & Winston zoomies
     - `09`: Chattanooga Lookout Mountain panoramic vista
     - `10`: Sunny Friday morning lattes & croissants in Town at Trilith
     - `11` (`#aggie-finale`): Post-Credits Bonus Panel of Aggie & Winston sitting together in the sunny Georgia autumn backyard (ear scratches + spiky ball)
   - **Secret 16-Bit Post-Credits Interactive RPG Cutscene (`#secret-postcredits`):**
     - Triggered via the retro teaser bar right below Panel 11 (`"WAIT... DON'T CLOSE THE BOOK YET!"` / `"Tap for Secret Post-Credits Scene"`).
     - Flips cleanly from watercolor comic style into a starry midnight 16-bit SNES/GBA arcade theater (`'Press Start 2P'` & `'Silkscreen'` typography, twinkling CSS pixel stars, chunky gold/cyan double border, subtle CRT scanline sheen, mobile-first layout, and full `prefers-reduced-motion` + keyboard support).
     - **4-Beat Interactive Tap-Through RPG Cutscene** featuring `images/12-postcredits-trio.{webp,jpg}` (`1100x614`): Winston, Guardian Angel Bella, and 16-bit Pixel Aggie (with her borrowed Mind Stone) gear up for `"MISSION: SAVE MOM!"`, with typewriter dialogue, Sound ON/OFF toggle, Skip to Title, and authentic iOS Safari-safe Web Audio synth ported directly from `winston-game` (Winston's double-woof formant bark, Bella's 5-note starlight chime, Aggie's chic 3-tone robot chirp, gentle typewriter blips, and triumphant 16-bit title fanfare).
     - **Grand Finale Title Card** cross-fading to `images/13-postcredits-titlecard.{webp,jpg}` (`1100x614`) with a high-contrast retro arcade overlay (`COMING SOON` / `WINSTON & AGGIE'S GEORGIA ODYSSEY` / `MISSION: SAVE MOM!` / `Featuring Guardian Angel Bella • Powered by Mind Stone & Spiky Ball`), plus `Replay Cutscene` and `Close Secret Scene` controls.
   - **35-second HD Mini-Movie Trailer** (`webb-georgia-adventure.mp4`, `1280x720`, 24 fps, H.264 + acoustic Rhodes soundtrack).
   - **Fixed Interactive Map (33 Starred Stops):** Switched from broken CARTO tiles to zero-API-key Esri World Street Map + Esri World Topo Map toggle.
   - **Shared Packing Checklist (`41` items across 6 categories):** Backed by `checklist.json` and `PACKING_LOG.md`, with custom item add forms and `All` / `Unpacked Only` filters.
   - **Monday Morning, Nov 23 Farewell Breakfast Added:** **Lula Cafe** (`2537 N Kedzie Blvd`, Logan Square, `9:00 AM to 3:00 PM`, walk-in only, closed Tuesdays) added to Chapter 1 timeline (`#day-1`).
   - **Live 5-Day Route Weather Forecast Added (`#weather-summary` + Per-Day Chapter Strips):** Pre-rendered Open-Meteo snapshot for Nov 23 to Nov 27 (`Chicago`, `South Indy / Columbus`, `Franklin`, `Chattanooga`, `Trilith / Peachtree City`) with hourly activity-window temps, precip `%`, wind `mph`, sunset times, and automatic zero-API-key Open-Meteo live browser refresh + manual Refresh button.
   - **Secret 16-Bit Post-Credits Mini-Movie (`#secret-postcredits`, `postcredits-georgia-odyssey.mp4`):** Playable auto-advancing 36-second 16-bit animated trailer (`1280x720`, 24 fps, H.264 + custom 16-bit chiptune & Winston bark/Aggie chirp soundtrack): Jordan & Janie head to the store for paper plates, Winston wakes from a bad dream in the new house with Bella nowhere to be found, nose-dials Aggie on the phone, Aggie unlocks the back smart-lock, and Winston escapes into Peachtree City (`WINSTON'S GEORGIA ODYSSEY: LOST IN PEACHTREE CITY | Wait... Where Is Bella?`).
   - **Night 3 Confirmed Banner:** Trilith Guesthouse suite stay & Prologue Thanksgiving Feast marked **CONFIRMED & UPGRADED!** on the public page (private booking IDs and rates intentionally kept out of this public repo).
   - **Legacy Work Worker Removed:** Old U.S. Soccer Cloudflare Worker (`georgia-thanksgiving-adventure`) was deleted cleanly so personal and work infrastructure stay separated.
2. **Aggie Character & WhatsApp Lookbook Continuity:**
   - Persona name: **Aggie** (`Antigravity -> AGY -> Aggie`), sassy, warm, chic little cream-ivory & sage-green robot with dark glass visor, amber eyes, tortoiseshell sunglasses on her head, terracotta-orange silk neck scarf, and brass ear accents.
   - Janie asked `"What would a chic little robot look like?"` and received a 3-look watercolor lookbook (Look 1: Parisian Cafe Chic; Look 2: Georgia Boutique Chic; Look 3: Celestial Pearl & Rose-Gold) plus a playful foot-tapping mid-wardrobe limbo comic nudge.
   - Local WhatsApp watcher was cleanly stopped by Jordan at 2:53 PM CT (Nov 22).

---

## 2. Open Tasks Ready to Pick Up in Cloud Mode

### A. Site Passcode Lock (Option 1: COMPLETED & LIVE!)
- **Status:** `index.html` on GitHub Pages is now **AES-256-GCM encrypted** (PBKDF2-HMAC-SHA256, `250,000` iterations, Web Crypto native browser decryption) with `<meta name="robots" content="noindex, nofollow">` and a comic-themed `"Webb Family Private Storybook"` unlock screen (supports iPhone/desktop password autofill, Show/Hide toggle, remembered unlock via derived AES key in `localStorage`, and a `"Lock Storybook"` button in the footer).
- **Important for future edits:** Do NOT overwrite `index.html` with unencrypted HTML. Plaintext source stays locally on Jordan's laptop, and NEVER commit the passcode string to Git. If Jordan later wants Option 2 (full image/asset encryption in a fresh repo with clean Git history), ask for confirmation first.

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
