# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Run the sync script automatically on Renovate vendir branches and push the result for review.
- Add a check which fails a pull request if the sync script was not run.
- Add shared helpers file to sync dir.

### Changed

- Create the vendir update issue as the `giantswarm-project-automation` GitHub App instead of architectbot's `ISSUE_AUTOMATION` token (giantswarm/giantswarm#38800).
- Use the `giantswarm-release` GitHub App instead of the taylorbot personal access token to push sync commits.
- Disable Helm image reference verification in CI config.
- Revert 'Disable Helm image reference verification in CI config'.
- Stop overriding appVersion in chart metadata.
- Add Github action to create an issue in `giantswarm/giantswarm` for Team Rocket on vendir updates.
- Update architect to v10.13.0 (giantswarm/kube-vip-app#89)
- Update architect to v10.13.2 (giantswarm/kube-vip-app#90)
- Update architect to v10.13.4 (giantswarm/kube-vip-app#92)
- Use Linux tools to manipulate chart label instead of an inscrutable Perl command.
- Update architect to v10.14.8 (giantswarm/kube-vip-app#97)
- Update architect to v10.14.10 (giantswarm/kube-vip-app#102)
- Update actions/create-github-app-token to v3.3.0 (giantswarm/kube-vip-app#107)
- Update architect to v10.14.18 (giantswarm/kube-vip-app#108)
- Update architect to v10.15.1 (giantswarm/kube-vip-app#109)
- Update architect to v10.16.3 (giantswarm/kube-vip-app#110)
- Update architect to v10.16.6 (giantswarm/kube-vip-app#114)
- Update architect to v10.16.7 (giantswarm/kube-vip-app#115)

### Fixed

- The `helm.sh/chart` label is valid for long chart versions: the 63-character cut trims the whole trailing run of `-`, `.` and `_`.
- Move manual edit of daemonset manifest to a patch file.
- Fix changelog generation script.

## [0.3.0] - 2026-03-03

### Changed

- Improve Chart.yaml metadata and management.
- PolicyException: Use Kyverno-native API instead of Giant Swarm abstraction.
- DaemonSet: Ensure leading `v` when defaulting to `.Chart.AppVersion`.

## [0.2.0] - 2025-02-25

### Changed

- Push to default catalogs.

## [0.1.0] - 2025-02-20

### Added

- Initial release which tracks upstream version `0.8.4`.

[Unreleased]: https://github.com/giantswarm/kube-vip-app/compare/v0.3.0...HEAD
[0.3.0]: https://github.com/giantswarm/kube-vip-app/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/giantswarm/kube-vip-app/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/kube-vip-app/compare/v0.1.0...v0.1.0
[0.1.0]: https://github.com/giantswarm/kube-vip-app/releases/tag/v0.1.0
