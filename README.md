XYZ AM Community Apps Registry

A public JSON registry of apps that live on or integrate with XYZ AM.
This repo is the canonical source for tools, games, extensions, utilities, and community projects available at *.xyz.am.

Why this exists

- Discovery: power an apps directory, tag browsing, and search
- Consistency: one lightweight format for all apps
- Community: anyone can submit an app via pull request
- Automation-ready: easy to validate + generate pages from

## Registry format

Apps live in apps.json under the "apps" array.

Minimal example:

```json
{
  "name": "My Cool App",
  "subdomain": "coolapp",
  "tags": ["utility", "fun"],
  "description": "One sentence saying what it does.",
  "badge": ""
}
```

## Field notes

- name (required): human-friendly title
- subdomain (required): the XYZ AM subdomain (no .xyz.am)
- tags (required): lowercase keywords for filtering/search
- description (required): short, user-facing summary
- slug (optional): if different from subdomain
- url (optional): full URL if needed
- badge (optional): e.g. "official", "beta", "community" or empty

## What counts as an app?

- Anything that is:
- Hosted on an XYZ AM subdomain, or
- An official XYZ AM integration (browser extensions, etc.), or
- A community tool you want discoverable from XYZ AM.

## Contributing an app

- Fork this repo
- Edit apps.json and add your app to the array
- Open a pull request

Please:
- keep descriptions to 1 sentence
- use practical tags (e.g. utility, game, rss, developer)
- don’t add duplicates
- leave badge empty unless it’s official or you want a specific label

## Suggestions / changes

Open an issue if you want a new tag convention, schema changes, or automation hooks.
