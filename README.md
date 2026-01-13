# gdl-arm

arm64 builds of [gallery-dl](https://github.com/mikf/gallery-dl).

## About

gallery-dl doesn't currently offer arm64 binaries. The intention behind this is for use
with [gdluxx](https://github.com/gdluxx/gdluxx), though it will work outside the gdluxx project as well.

If you don't know that you need this, you probably don't need this.

The binaries are built automatically following the
[official gallery-dl build process](https://github.com/mikf/gallery-dl/blob/master/scripts/pyinstaller.py).

## Build Schedule

Builds run automatically at **00:00, 06:00, 12:00, and 18:00 UTC** daily.

When a new gallery-dl release is detected, an arm64 binary is built and published as a github release with a matching
version tag.

### With gdluxx

[gdluxx](https://github.com/gdluxx/gdluxx) now auto detects host architecture. If an arm64 system is detected, the
binary from this repo will be downloaded. If x86 architecture is detected, the official gallery-dl is still downloaded.

## Version Compatibility

Release tags in this repository mirror the upstream gallery-dl tags (e.g.,
`v1.28.0`). Each release contains a single asset: `gallery-dl.bin`.

## Credits

- [gallery-dl](https://github.com/mikf/gallery-dl) by [mikf](https://github.com/mikf)
- Build process based on guidance from [gallery-dl#8774](https://github.com/mikf/gallery-dl/issues/8774)
