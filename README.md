# Schelde crossing data

Ferry timetables for the *Snel over de Schelde* app, rebuilt daily from the
operators' own published schedules and republished here only when something
actually changes.

**This repository is generated.** Every file is overwritten on each publish,
so changes made here by hand will be lost. The scraper, its tests and the
workflow that writes this live in a separate private repository.

| File | Size |
| --- | --- |
| [`v1/sint_anna_ferry.json`](v1/sint_anna_ferry.json) | 6,698 bytes |
| [`v1/waterbus.json`](v1/waterbus.json) | 66,511 bytes |
| [`v1/index.json`](v1/index.json) | manifest |

Served over GitHub Pages with `ETag`, so a conditional request costs nothing
when the data has not changed.

The schema version is in the path. Anything published under
`v1/` keeps that shape for good; an incompatible change would
appear under `v2/` instead, so existing app installs never
break.

The commit history of this repository is a log of every timetable change that
has reached users, each one referencing the commit it was built from.

## Provenance

Data belongs to its operators: [De Waterbus](https://dewaterbus.be/) and
[Agentschap MDK](https://www.agentschapmdk.be/). It is reproduced here
unmodified, for use by one app. Refer to the operators for anything
authoritative — a timetable here can be up to a day behind theirs.

Last built 2026-09-07T19:28:45Z from commit
`caa7b6cf779e`.
