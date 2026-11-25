# friendly-pup

Two single-page sites, one folder each. Plain HTML and CSS, no build step.

| Folder | Domain | What it is |
| --- | --- | --- |
| `billfugina/` | billfugina.com | Professional page: who Bill is, what he builds, links to his apps |
| `dogspots/` | dogspots.com | Personal page: a hello, the same app links, a link to billfugina.com |

## Deploying on Vercel

Two Vercel projects, both connected to this repo:

1. New project, import this repo, set **Root Directory** to `billfugina`, framework preset **Other**, no build command.
2. Same again with Root Directory `dogspots`.
3. In each project's Git settings, turn on skipping deployments when nothing in its root directory changed, so an edit to one page doesn't redeploy the other.
4. Add the domain (and its `www`) to its project. DNS steps are in the switch-over plan.

## Editing

Each page is one `index.html` and one `styles.css`. Look for `TODO` comments for the spots that need Bill's input (app addresses, photos).

## Preview locally

```
npx serve billfugina
npx serve dogspots
```
