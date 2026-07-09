# ygo-rush-cards-images

Repository for storing Yu-Gi-Oh! Rush Duel card images using passcodes that match the ProjectIgnis ID format.

## Passcode guidelines

Announced OCG/TCG cards receive a 9-digit prerelease passcode until official release, then switch to the official passcode.

Speed Duel and Rush Duel each have dedicated ranges:

- Speed Duel: `30ZYYYXXX`
- Rush Duel: `160ZYYXXX`

### Components

- `XXX`: card index within its set
- `Y` or `YY`: set index, incremented by one for each chronological set of that product type

Set index notes:

- Structure Decks: `YY` comes from the prefix (for example `SD38`, `ST18`, `SR10`)
- Structure Deck Enhancement Packs: share deck `YY`, with `XXX + 50`
- Deck Build Packs: `YY` continues from the previous one
- Duelist Packs: `YY` comes from the prefix
- TODO: there is potential overlap with this scheme and it may be reworked

### OCG/TCG prerelease passcode ranges

- Main set: `10ZZYYXXX`
  - Series `ZZ`: currently `11`
- Side set: `1002YYXXX`
  - All `VJMP-JP` (V Jump) promos are considered part of set `200`
  - All `WJMP-JP` (Weekly Shounen Jump) promos are considered part of set `203`
  - All `SJMP-JP` (Saikyou Jump) promos are considered part of set `204`
- Structure Deck and Starter Deck: `1003YYXXX`
- Deck Build Pack and Duelist Pack: `1004YYXXX`

### Rush Duel ranges (`160ZYYXXX`)

- `Z` product type:
  - `0`: KP Deck Modification Pack ("main booster")
  - `2`: CP Character Pack ("side booster")
  - `3`: ST Starter Deck
  - `4`: Promos

## Unofficial cards

Unofficial cards currently use multiple historical ranges, but are being reorganized toward `511YYYXXX`.

## Alternate artwork policy

Cards with passcodes aliased to another passcode within `10` are treated as alternate artworks.
