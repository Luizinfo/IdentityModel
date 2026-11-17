# Changelog

## Unreleased

- Pin local builds and CI to .NET SDK 10.0.401 through global.json.
- Validate pull requests on Windows, Linux, and macOS without package publication.
- Use the patched SourceLink implementation supplied by the SDK instead of the vulnerable Microsoft.Build.Tasks.Git 8.0.0 dependency.

## 10.0.0

- Rebranded the NuGet package from `IdentityModel` to `ZinfoFramework.IdentityModel` as an independent continuation maintained by Luiz Antonio.
- Target framework is now `net10.0` only.
- Preserved the `IdentityModel` assembly name, namespaces, and public API surface.
- Updated package provenance, repository, documentation, support, and security metadata.

### Migration

Replace the package reference with `ZinfoFramework.IdentityModel` version `10.0.0`, upgrade the consumer to .NET 10, and retain existing `IdentityModel` namespace imports.
