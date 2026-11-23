# Study Quest v5.0

Dark-fantasy visual refresh and expanded study-to-RPG reward loop.

## v5 additions
- Recruit monsters after victories at a very low species/rank/level-adjusted chance, or attempt capture with Monster Seals. Every recruited monster must be named.
- Companion roster (30 maximum), party of up to three, manually selected companion action each turn (attack/heal/guard), no passive party bonuses.
- Random gender and personality, gradual personality growth through intimacy, study and adventure bonds, companion leveling, and paid stat training.
- Branching, irreversible evolution with level-first requirements, intimacy for advanced paths, and hinted special conditions.
- New Dwarf and Oni families; more humanlike evolutionary direction for humanoid races while preserving species identity.
- Normal defense is moderate; Iron Wall is a powerful limited-use skill.
- Study rewards also grant a modest amount of GOLD (30% of earned XP, rounded down).

## v4 additions
- All normal and urgent quest entries reset to incomplete each new local calendar day; quest definitions, completed-day history in logs, XP, and levels are preserved.
- XP exchange shop: spendable XP buys potions, equipment, and skill books. Spending XP does not reduce lifetime XP or level.
- Reward shop entries can be added, redeemed, and deleted.
- Dedicated illustrated battle backgrounds for plains, forest, and dungeon/ruins.
- Battle hit flash/slash effects.
- Synthesized UI and battle sounds using Web Audio; audio begins after the first user tap and can be muted at device level.
- Black/white dark-fantasy theme with Japanese Mincho-style typography and framed panels.
- Monster portrait and text layout spaced to prevent overlap.

## Deploy
Upload and replace the root files plus the `assets` folder in the existing GitHub Pages repository. Keep the folder structure exactly as provided.

## Data
The app continues using localStorage key `studyQuest_v1`; existing v4 data is retained and new monster fields are added. Spendable XP is `xp`; lifetime XP used for levels is `totalXP`. Purchases only subtract spendable XP. Back up JSON before updating.

## Validation
JavaScript syntax checks and ZIP integrity checks were run. Full iPhone/Safari end-to-end interaction testing has not been completed; after deployment, test recruitment, naming, party commands, capture, and evolution with a JSON backup safely stored first.


## Study Quest v6.0 — Visual Upgrade
- Added 16 dedicated WebP monster portraits in `assets/monsters/`.
- Goblin, oni, dwarf, and slime families now use dedicated art across their existing evolution stages.
- Bestiary cards, battle portraits, companion cards, and evolution trees share the same portrait assets.
- Wolf, undead, spirit, and dragon families retain their v5 artwork in this first visual pass; their dedicated evolution art is planned for a follow-up visual pack.
- Existing local save key (`studyQuest_v1`) is preserved to support v5 save-data continuity.
- Service worker cache updated to `study-quest-v6` and pre-caches all monster portraits.
