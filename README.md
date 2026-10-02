# Neon Drift
Open index.html (or host the folder on GitHub Pages / Netlify / Cloudflare Pages). Works as an installable PWA when served over https.

Controls: arrows/WASD, Space=pause, tap/drag lanes on touch.
Ads: set window.NEON_ADS={rewarded:cb=>{/* show ad, then cb() */}}.
Online leaderboard: add Firebase in game.js over() where S.lb is saved.

Modes: Campaign (20 levels), Endless, Time Attack. Difficulty: Easy, Normal, Medium, Hard, Insane.
Power-ups: Shield, Magnet, Nitro, Time Warp.

v3: 30 replayable campaign missions (first clear 100 bonus, replays 60%), Shop with permanent power upgrades and boosts, car perks (coin bonus, extra heart), rewarded-ad double coins.

v4: boss missions (every 5th, 2x reward), trucks + oil slicks, new car designs, procedural music + engine sound, stars/exhaust FX.
Global leaderboard: create a Firebase Realtime Database (rules: scores .read/.write true, .indexOn s) and add <script>window.NEON_LB_URL='https://YOUR-DB.firebaseio.com'</script> before game.js in index.html.

v5 HEAVY: 50 missions, 10 real bosses with HP bars + rage phase, auto Gatling gun (8 upgrade levels), Rockets (F / FIRE) and Nukes (N / NUKE) bought in Shop, bosses must be destroyed to clear mission (3x reward).

v6: 4-star missions (next mission unlocks only at 4 stars), 3-5 laps per mission with 8 scenes + lap types (Rush Hour, Oil Field, Convoy, Coin Rain, Storm), 💎 gems on the road, NO free weapons (Gatling 900🪙, ammo-time upgrades, rockets, nukes 6💎), 3 hits = dead, car hearts by tier, elite cars cost gems, difficulty ramps harder per mission and per mode. Save key changed to nd5.

v7: heavy synthesized SFX (gatling, rocket, explosions, crash+vibration, boss roar, star jingle), hit/nuke screen flash, low-health red pulse, boss danger-lane warning + ENRAGED phase, Repair pickup, Lucky Chest after 3+ stars.
