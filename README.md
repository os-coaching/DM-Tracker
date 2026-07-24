# DM Outreach Tracker

Personal Instagram DM outreach pipeline. Single self-contained `index.html`, no build step, no dependencies.

## Running it

Either open `index.html` directly, or visit the GitHub Pages URL.

## Data

Everything lives in `localStorage` under the key `dm_tracker_v1`. Nothing is sent anywhere and there is no server.

That means data is **per browser and per origin**. The copy you open from your hard drive and the copy on the Pages URL do not share data, and neither do your laptop and your phone. Use **Export JSON** on one and **Import JSON** on the other to move a pipeline across.

Countdowns are recomputed from stored timestamps on every tick, so they survive refreshes, closed tabs and restarts.

## Pipeline

| Tab | Holds |
| --- | --- |
| Leads | First DM sent, waiting on a reply. Day 3 follow-up, day 7 meme, then archive. |
| Leads That Respond | In conversation. Stage dropdown, notes, park (21 days), dead. Clients pinned at the bottom. |
| Leads That Don't | Archived. Revive moves them back to Control Q. |
| Script | The full DM script as checkpoints, every line copy-to-clipboard. |

## Backups

`localStorage` is wiped if you clear browsing data for the site. Export a JSON backup regularly.
