# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.3.4] - 2020-05-26
### Fixed
- Because of the target OS, deltas weren't computed correctly.
- Delete files on backup that don't exist in the tracking directory.

## [0.3.3] - 2020-05-23
### Fixed
- Better formatting for the backup log.

## [0.3.2] - 2020-05-23
### Fixed
- Use options that improve rsync compression.

### Changed
- Made small updates to the README.

## [0.3.1] - 2020-05-23
### Added
- The directory for files and directores being tracked from backup.
- A basic README for the project.

## [0.3.0] - 2020-05-23
### Added
- A script to register files and directories to be backed up.

## [0.2.0] - 2020-05-23
### Added
- A script to setup the backup's destination.

## [0.1.0] - 2020-05-23
### Added
- Created proof of concept file backup tool.

[Unreleased]: https://github.com/adamtabrams/sink/compare/0.3.4...HEAD
[0.3.4]: https://github.com/adamtabrams/sink/compare/0.3.3...0.3.4
[0.3.3]: https://github.com/adamtabrams/sink/compare/0.3.2...0.3.3
[0.3.2]: https://github.com/adamtabrams/sink/compare/0.3.1...0.3.2
[0.3.1]: https://github.com/adamtabrams/sink/compare/0.3.0...0.3.1
[0.3.0]: https://github.com/adamtabrams/sink/compare/0.2.0...0.3.0
[0.2.0]: https://github.com/adamtabrams/sink/compare/0.1.0...0.2.0
[0.1.0]: https://github.com/adamtabrams/sink/releases/tag/0.1.0
