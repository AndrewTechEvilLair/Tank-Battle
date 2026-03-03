TANK BATTLE
Version 1.1
A browser-based artillery game inspired by the 1991 DOS classic Scorched Earth. Two tanks face off across procedurally generated terrain — adjust your angle and power, account for wind, and blow your opponent to pieces before they do it to you.

Play
Open tank_battle_v1.1.html in any modern browser. No server, no install, no dependencies — it's a single self-contained file.
For best experience, play on a mobile device in landscape mode or on a desktop browser.

Game Modes
ModeDescriptionSpectatorWatch two AI tanks fight each otherOne PlayerYou vs the AI (OMEGA)Two PlayersHot seat — take turns on the same device

Controls
Mobile

Angle slider — left edge of screen (drag up/down)
Power slider — right edge of screen (drag up/down)
Fire — tap your tank
Weapon — tap weapon chips along the bottom

Desktop

← → Arrow keys — adjust angle
↑ ↓ Arrow keys — adjust power
Spacebar — fire
Weapon chips — click to select


Weapons
WeaponAmmoDescriptionShellUnlimitedStandard direct hit, medium blast radiusMIRV3Splits into 4 submunitions on impactBaby Nuke2Massive blast radius, high damageDirt4Builds terrain instead of destroying it — use for coverNapalm3Wide area splash damage

Features

Procedural terrain — every round generates a unique landscape via midpoint displacement
Ballistic physics — projectiles arc realistically with gravity and wind drift
Deforming terrain — explosions carve craters; dirt rounds pile up
AI opponent — CPU selects weapons situationally and improves accuracy as it wins
AI trash talk — OMEGA taunts you via the Anthropic API in One Player mode
Shot report — post-shot overlay showing weapon, angle, power, distance, peak altitude, and damage
Portrait lock — prompts rotation on mobile devices in portrait mode


Technical Notes

Built as a single HTML/CSS/JS file — no build step, no frameworks
Canvas sized via offsetWidth/offsetHeight with requestAnimationFrame timing for reliable mobile rendering
Terrain stored as Float32Array for performance
AI uses physics simulation to calculate optimal firing solutions with tunable noise
Trash talk powered by claude-haiku-4-5 via the Anthropic API (gracefully silent if the API is unavailable)


Versioning
VersionNotesV1.0Initial release — renamed from Scorched Earth to Tank BattleV1.1Version label brightness increased

Roadmap

Touch-optimized controls refinement
Async multiplayer via Firebase (turn-based, chess.com style)
Taunt system with push notifications
Weapon shop between rounds
User accounts and match history
Android APK via Capacitor + Play Store release
