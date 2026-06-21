# rapaf-assets

Static media for the RAPAF / ФВСАР site ([new.rapaf.ru](https://new.rapaf.ru)), served via the
free [jsDelivr](https://www.jsdelivr.com/) GitHub CDN so the application repo stays lean.

## Galleries

Migrated from the legacy WordPress site (rapaf.ru, Envira Gallery) before that host is
decommissioned. Originals (`link` field) downloaded where available, otherwise the largest
surviving size.

- `galleries/<slug>/NN.jpg` — images, numbered in original gallery order.
- `galleries.json` — manifest: per gallery `slug`, `title` (RU), `count`, and per image
  `file`, `caption`, `origUrl` (source on old site), `cdn` (jsDelivr URL), dimensions.

**CDN URL pattern:**

```
https://cdn.jsdelivr.net/gh/pvsmolyakov-svg/rapaf-assets@main/galleries/<slug>/<file>
```

33 galleries, 220 images. See `LOST_IMAGES.txt` for 31 images whose source files were already
deleted from the old server (galleries `kfs-samara`, `forum-nsar` fully lost; `kfs-ufa` partial)
and could not be recovered (not in Wayback Machine either).
