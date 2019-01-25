# Curator

## Restore

In order to restore Elasticsearch indices, you must create a new pipeline to deploy 'curator-restore' service.
Define these environment variables to configure manual pipeline:

* **SNAPSHOT_RESTORE_NAME**: Snapshot source name to restore indices. Leave it empty to use last snapshot.
* **SNAPSHOT_RESTORE_INDICES**: Name/expression to filter indices to restore. Accepts wildcards.

Then, you can run deploy task manually.
