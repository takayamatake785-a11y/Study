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


## Study Quest v7.0 — Visual Upgrade
- Added 16 dedicated WebP monster portraits in `assets/monsters/`.
- Goblin, oni, dwarf, and slime families now use dedicated art across their existing evolution stages.
- Bestiary cards, battle portraits, companion cards, and evolution trees share the same portrait assets.
- Wolf, undead, spirit, and dragon families retain their v5 artwork in this first visual pass; their dedicated evolution art is planned for a follow-up visual pack.
- Existing local save key (`studyQuest_v1`) is preserved to support v5 save-data continuity.
- Service worker cache updated to `study-quest-v7` and pre-caches all monster portraits.


## v7.0 更新
- 性別を敵出現時に決定し、仲間になっても引き継ぐ仕組みを追加（ドワーフは男性のみ）
- 仲間の個体才能・外見色・食べ物履歴を保存
- 食べ物による親密度上昇と、3回ごとの髪・目・体色変化
- 仲間のおやつ購入欄を追加
- 鬼の女性専用進化「妖鬼」を追加
- ゴブリン・鬼・ドワーフの新規イラストを追加
- 既存の localStorage キー studyQuest_v1 を維持


## v7.2
- おやつと魔物の封印札を所持XP限定に変更
- 全滅時の固定5 GOLDペナルティ
- 仲間の初期能力を調整し、回復にMP消費・戦闘中2回制限を追加
- 髪・目だけの外見変化と段階的な色変化表示
- 仲間画面の簡易表示／全表示切替
- 紺色系UIテーマに統一
- 既存の `studyQuest_v1` セーブキーを維持


## v7.3 — 冒険者成長・高レベル冒険エリア拡張
- 学習XPによる冒険者レベルを最大Lv.99に設定
- レベルアップ時の冒険者ステータス成長を継続
- Lv.24以降の高難度エリアを追加し、最大Lv.99帯まで段階的に解放
- エリアごとの推奨レベル帯に合わせて敵レベルが変化
- Lv.20以降の敵ステータス成長を緩やかに調整
- 既存の保存キー `studyQuest_v1` と既存データを維持
- 戦闘の行動・スキル・報酬システムは変更せず、既存の仕組みを維持
