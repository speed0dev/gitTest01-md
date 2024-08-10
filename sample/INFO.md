# Github Action - Releases API

**Please note:** This repository is currently unmaintained by a team of developers at Github.

**Maintained Actions:***
* [elgohr/Github-Release-Action](https://github.com/elgohr/Github-Release-Action)

To reflect this state we've marked this repository as Archived.

## Usage
### Pre-requisites
Create a workflow

- 'tag_name' : The name of the tag for this release

```yaml
on:
  push:
    # Sequence of patterns matched against refs/tags
    tags:
      - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10

name: Create Release

jobs:
  build:
    name: Create Release
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v2
      - name: Create Release
        id: create_release
        uses: actions/create-release@v1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided by Actions, you do not need to create your own token
        with:
          tag_name: ${{ github.ref }}
          release_name: Release ${{ github.ref }}
          body: |
            Changes in this Release
            - First Change
            - Second Change
          draft: false
          prerelease: false
```

## License
The scripts and documentation in this project are released under the [MIT License](LICENSE)
