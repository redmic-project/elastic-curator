# Curator

## Restore

In order to restore Elasticsearch indices, you must create a new pipeline to deploy 'curator-restore' service.
Define these environment variables to configure manual pipeline:

* **DD_SNAPSHOT_RESTORE_NAME**: Snapshot source name to restore indices. Leave it empty to use last snapshot. Empty by default.
* **DD_SNAPSHOT_RESTORE_INDICES**: Name/expression to filter indices to restore. Accepts wildcards. Leave it empty to restore all indices. Default: `index.name`.
* **DD_SNAPSHOT_RESTORE_RENAME_PATTERN**: Expression to match indices names and prepare text groups to replace, in order to rename restored indices. Leave it empty to keep original names. Empty by default.
* **DD_SNAPSHOT_RESTORE_RENAME_REPLACEMENT**: Replacement for matched indices names, in order to rename restored indices. Default: `restored_<capture-group-1>`.

Then, you can run deploy task manually.
