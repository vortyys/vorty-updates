# vorty-updates

Latest versions of the vorty.dev FiveM resources, read by **vorty-core** to show update notices in the server console.

## Releasing an update

Edit `versions.json`, raise the resource's `version` and fill in what changed:

```json
"vorty-mdt": {
  "label": "vorty MDT",
  "version": "2.2.0",
  "date": "2026-11-02",
  "changes": ["Warrant search with filters", "Fixed the BOLO list"],
  "files": ["server/warrants.lua", "html/js/app.js"],
  "download": "https://portal.cfx.re/assets/granted-assets"
}
```

Servers see it at their next check (start of the server, then every few hours). `files` and `download` are optional.
