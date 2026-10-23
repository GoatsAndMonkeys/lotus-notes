# Lotus notes packs

Static, signed liner notes exported by a Music Lotus server (`lotus notes export`). Serve this
directory from any static host (GitHub Pages, Netlify, S3, nginx, the Lotus server itself).
A client needs only the base URL and the server's public key.

Server key `8S5sc7cJpSpOBVnivFR9tA`: `WJqEYf19eeDyBbiEyvlsQTUnMwm8MRDTZ0JwvaxzUTY`

- `MountainGoats/` MountainGoats

- `index.json` lists the packs and the key; `index.json.sig` signs it.
- `<collection>/manifest.json` lists every file of a pack with its sha256;
  `manifest.json.sig` signs it.
- Check a pack: `lotus notes verify <url>/<collection>/ --public-key <key>`.

The packs hold public facts, short cited notes and links: no audio, no listener data.
