# image-mirror

Unmodified, digest-identical copies of third-party container images, served from
`ghcr.io/alpha-affinity/mirror/*` so an upstream takedown cannot break the
consumers that pin them. The list lives in `.github/workflows/mirror.yml`.

| Image | Version | License | Corresponding Source | Upstream |
| --- | --- | --- | --- | --- |
| `mirror/silo` | `RELEASE.2026-09-16T00-00-00Z` | AGPL-3.0-or-later | [release `silo-RELEASE.2026-09-16T00-00-00Z`](https://github.com/alpha-affinity/image-mirror/releases/tag/silo-RELEASE.2026-09-16T00-00-00Z) (commit `2a4d514`) | [pgsty/silo](https://github.com/pgsty/silo) |

Each image is redistributed unmodified under its own license. The Corresponding
Source for every image served here is archived as an asset on this repository's
release `<name>-<version>`, taken at the exact commit recorded in the image's
`org.opencontainers.image.revision` label, so it stays available even if the
upstream project goes away. The mirror workflow archives it before publishing
and refuses to publish an image without it.

The silo image is built on Red Hat UBI, redistributed under the
[UBI EULA](https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI).
License texts for the bundled components ship inside the image under `/licenses/`.
