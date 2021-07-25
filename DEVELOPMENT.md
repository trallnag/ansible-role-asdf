# Development

## How to release a new version?

1. Make sure that the changelog contains an entry for the new version. The
   formatting must exacly match the schema.
2. Create a tag that satisfies the expression `*.*.*`.
3. Push. From here the pipeline will pick it up, import the new version to
   Ansible Galaxy and create a GitHub Release.

## What to do before releasing the first version?

1. Manually add the role via Ansible Galaxy Web UI.
2. Make sure `GALAXY_API_KEY` is set.
