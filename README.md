# Study Quest v4.0

Dark-fantasy visual refresh and expanded study-to-RPG reward loop.

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
Upload and replace the six root files plus the `assets` folder in the existing GitHub Pages repository. Keep the folder structure exactly as provided.

## Data
The app continues using localStorage key `studyQuest_v1`. Spendable XP is `xp`; lifetime XP used for levels is `totalXP`. Purchases only subtract spendable XP. Back up JSON before updating.
