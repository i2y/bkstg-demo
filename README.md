# bkstg-demo

Demo catalog repository for [bkstg](https://github.com/i2y/bkstg) - Mini IDP.

## Contents

- `catalogs/components/` - Sample service components
- `catalogs/apis/` - API definitions
- `catalogs/resources/` - Infrastructure resources
- `catalogs/systems/` - System groupings
- `catalogs/domains/` - Business domains
- `catalogs/users/` - Team members
- `catalogs/groups/` - Teams
- `catalogs/locations/` - External catalog references
- `catalogs/scorecards/` - Score and rank definitions
- `catalogs/history/` - Score/rank history

## External Location

This demo includes a Location entity that references [bkstg-demo-external](https://github.com/i2y/bkstg-demo-external) repository, demonstrating multi-repository catalog aggregation.

## Usage

1. Install bkstg
2. Create `bkstg.yaml`:

```yaml
version: 1
sources:
  - name: demo
    type: github
    owner: i2y
    repo: bkstg-demo
    branch: main
    path: catalogs
    enabled: true
    sync_enabled: false
    auto_commit: false
```

3. Run `uv run bkstg`

## License

MIT
