# fixe-media-assets

Public delivery host for Fixe Media's own social assets.

Buffer has no upload endpoint, so every asset needs a public URL. This repo is
that URL. Files are served from `raw.githubusercontent.com`.

## Layout

    YYYY-MM/<post id>/<file>

Filenames: `F###_slug_PLATFORM_asset.ext`

- `F###` Post ID from the Notion Content Calendar
- `PLATFORM` one of `ALL`, `IG`, `FB`
- `asset` `a`, `b`, `c` for carousel slides, `reel` for video

Carousel slides are lettered, never numbered. Bare digits sort 1, 10, 2, 3 and
break slide order silently.

## Rules

- Finished social assets only. This repo is public.
- Fixe Media's own content only. Client work lives in that client's repo.
- Never contracts, credentials, invoices or anything not cleared to publish.
- Deleting a file does not erase it. Git keeps the blob. Treat anything pushed
  as permanently public.
- This is a delivery mechanism, not an archive. The content folder on the Mac is
  the source of truth.

Full pipeline: `Fixe-Buffer-Scheduling-Runbook.md` in the FIXE MEDIA SMM project.
