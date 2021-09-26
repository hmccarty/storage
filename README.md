A consistent file structure to maintain data across multiple machines.

Heavily based on the [datacurator-filetree](https://github.com/roboyoshi/datacurator-filetree/tree/master).

## Structure
- `apps/`: Full fledged applications or packaged software.
- `archive/`: Backups and miscellaneous files.
- `docs/`: General documents, usually PDFs.
- `pics/`: Any picture-based content.
- `repos/`: Git-based repositories.
- `projects/`: Collections of files related to specific and ongoing pursuits.
- `sounds/`: Any audio-based content.
- `vids/`: Any video-based content.

Most folders are nested by date:

`<folder>/<year>/<month>/<day>/<file>`

## Merging
The primary benefit is to enable easy merging between different filesystems.

If the same stucture exists on the same computer, they can combine files simply by running:

```bash
unison storage-desktop/ storage-laptop/
```
