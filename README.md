# ZinfoFramework.IdentityModel

> [!IMPORTANT]
> This repository and package are an independent continuation of the historical IdentityModel project, maintained by Luiz Antonio under the ZinfoFramework name. They are not endorsed by, sponsored by, or operationally maintained by the original upstream authors or Duende Software.

ZinfoFramework.IdentityModel is a .NET library for claims-based identity, OAuth 2.0, and OpenID Connect. It provides request and response types, HTTP extension methods, protocol constants, and convenience APIs for common identity operations.

## Package identity and compatibility

| Historical package | Current package |
| --- | --- |
| `IdentityModel` | `ZinfoFramework.IdentityModel` |

Install version 10.0.0:

```shell
dotnet add package ZinfoFramework.IdentityModel --version 10.0.0
```

This release targets **.NET 10 only** (`net10.0`). The assembly name remains `IdentityModel`, and existing namespaces such as `IdentityModel`, `IdentityModel.Client`, and `IdentityModel.Jwk` are preserved.

## Breaking changes and migration

- Replace the NuGet package reference from `IdentityModel` to `ZinfoFramework.IdentityModel`.
- Upgrade the consuming project to `net10.0` or a compatible future target framework.
- Do not change existing `using IdentityModel...` directives or assembly references; the namespaces and assembly name are intentionally unchanged.
- Review the [changelog](https://github.com/Luizinfo/IdentityModel/blob/main/CHANGELOG.md) before upgrading.

## Project resources

- [Repository](https://github.com/Luizinfo/IdentityModel)
- [Issues](https://github.com/Luizinfo/IdentityModel/issues)
- [Contributing](https://github.com/Luizinfo/IdentityModel/blob/main/CONTRIBUTING.md)
- [Security policy](https://github.com/Luizinfo/IdentityModel/blob/main/SECURITY.md)
- [Support](https://github.com/Luizinfo/IdentityModel/blob/main/SUPPORT.md)
- [Changelog](https://github.com/Luizinfo/IdentityModel/blob/main/CHANGELOG.md)
- [Apache 2.0 license](https://github.com/Luizinfo/IdentityModel/blob/main/LICENSE)
- [Attribution and provenance notice](https://github.com/Luizinfo/IdentityModel/blob/main/NOTICE.md)

## Historical provenance and credits

This continuation derives from the original [IdentityModel/IdentityModel repository](https://github.com/IdentityModel/IdentityModel). Historical credit belongs to Brock Allen, Dominick Baier, and the original contributors. Links and package names associated with that upstream project, including later Duende packages, are historical references only and are not support or migration destinations for this continuation. See [NOTICE.md](https://github.com/Luizinfo/IdentityModel/blob/main/NOTICE.md) for the full distinction between current package authorship and historical authorship.

## Build and pull-request validation

Install the exact .NET SDK **10.0.401** selected by `global.json`. Run `./build.ps1` on Windows or `./build.sh` on Linux/macOS from the repository root. The default build compiles the solution, runs its tests, and creates local validation packages; it also validates trimming. CI installs the same SDK from `global.json` and checks Windows, Linux, and macOS Intel (macos-26-intel). It runs for pull requests and correction/release branches without publishing packages.

Unreleased build changes do not replace the existing NuGet release. A future publication requires a new package version and validation of the final artifacts.
