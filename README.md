# Lotus notes packs

Static, signed liner notes exported by a Music Lotus server (`lotus notes export`). Serve this
directory from any static host (GitHub Pages, Netlify, S3, nginx, the Lotus server itself).
A client needs only the base URL and the server's public key.

Server key `8S5sc7cJpSpOBVnivFR9tA`: `WJqEYf19eeDyBbiEyvlsQTUnMwm8MRDTZ0JwvaxzUTY`

- `BillyStrings/` Billy Strings: 2013–2026, 620 shows, 0 liner notes, notes in progress
- `GratefulDead/` Grateful Dead: 1965–1995, 2097 shows, 892 liner notes, notes in progress
- `KingGizzardAndTheLizardWizard/` King Gizzard & The Lizard Wizard: 2011–2026, 249 shows, 249 liner notes, ready
- `MountainGoats/` The Mountain Goats: 1992–2026, 463 shows, 463 liner notes, ready
- `MyMorningJacket/` My Morning Jacket: 1999–2026, 426 shows, 150 liner notes, notes in progress
- `Soulive/` Soulive: 1999–2026, 414 shows, 0 liner notes, notes in progress
- `TheWarOnDrugsMusic/` The War on Drugs: 2009–2026, 73 shows, 73 liner notes, ready
- `Ween/` Ween: 1989–2024, 717 shows, 0 liner notes, notes in progress

- `index.json` lists the packs and the key; `index.json.sig` signs it.
- `<collection>/manifest.json` lists every file of a pack with its sha256;
  `manifest.json.sig` signs it.
- Check a pack: `lotus notes verify <url>/<collection>/ --public-key <key>`.

The packs hold public facts, short cited notes and links: no audio, no listener data.
