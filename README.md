# NEXORA RP — FadeHost setup

## Required settings
- Node.js: **20 LTS** (recommended)
- Start command: `npm start`
- Environment variables:
  - `DISCORD_TOKEN` = your Discord bot token
  - `CLIENT_ID` = your Discord application/client ID

## Upload
Upload the contents of this folder directly into the repository root (the same level as `index.js` and `package.json`). Do not upload the folder as an extra nested directory.

## Dependencies
FadeHost should run `npm install` from the repository root. `better-sqlite3` is a native Node module, so the installed module must match the server's Node.js runtime. Do not copy `node_modules` from a different computer or Node version.

If the host provides a console after dependencies are installed, run:
`npm rebuild better-sqlite3`

If rebuilding reports missing `make`, `g++`, or Python, the hosting node/container needs native build tools enabled by the host; contact FadeHost support and ask them to enable/install the build tools or provide a compatible prebuilt better-sqlite3 binary for Node 20 Linux.
