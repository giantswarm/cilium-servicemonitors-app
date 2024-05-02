# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Change ownership from `phoenix` to `cabbage`.
- Use the app-build-suite.

## [0.1.2] - 2023-07-26

### Changed

- Drop metrics with high cardinality.
- Increase scrape interval to 60s.

## [0.1.1] - 2023-05-16

### Added

- Add overridability to the servicemonitors relabelings and metric_relabelings sections.

## [0.1.0] - 2023-05-15

### Added

- Allow disabling service monitors via helm value `disabled`.

### Fixed

- Fix helm template filenames to match actual content.

## [0.0.2] - 2023-02-24

### Changed

- Add labels to servicemonitors

## [0.0.1] - 2023-02-24

### Added

- Create ServiceMonitors to scrape Cilium


[Unreleased]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.1.2...HEAD
[0.1.2]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.0.2...v0.1.0
[0.0.2]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/cilium-servicemonitors-app/compare/v0.0.0...v0.0.1
