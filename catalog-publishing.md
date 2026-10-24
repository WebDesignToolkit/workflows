# Publish a catalog snapshot

1. Make approved changes in catalog/data/resources.json and validate the catalog.
2. On an authorized workstation, run website/scripts/sync_catalog.py with local catalog path.
3. Inspect the website generated JSON diff; verify count and checksum.
4. Commit and push to website explicitly after review.
5. Verify the live website only after its actual deployment; do not claim automatic refresh.

The website never writes to the canonical catalog. No GitHub Actions.
