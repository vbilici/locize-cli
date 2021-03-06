# locize-cli change log

All notable changes to this project will be documented in this file.

Project versioning adheres to [Semantic Versioning](http://semver.org/).
Change log format is based on [Keep a Changelog](http://keepachangelog.com/).


## [7.0.3](https://github.com/locize/locize-cli/compare/v7.0.2...v7.0.3) - 2020-02-05

- update android-string-resource dependency


## [7.0.2](https://github.com/locize/locize-cli/compare/v7.0.1...v7.0.2) - 2020-02-05

- update dependencies


## [7.0.1](https://github.com/locize/locize-cli/compare/v7.0.0...v7.0.1) - 2020-01-16

- alert if project not found


## [7.0.0](https://github.com/locize/locize-cli/compare/v6.0.8...v7.0.0) - 2020-01-06

- change default api endpoint to new api.locize.app domain


## [6.0.8](https://github.com/locize/locize-cli/compare/v6.0.7...v6.0.8) - 2019-11-07

- fix for edge case for msgctxt used with non i18next


## [6.0.7](https://github.com/locize/locize-cli/compare/v6.0.6...v6.0.7) - 2019-09-27

- try to also "import" context information


## [6.0.6](https://github.com/locize/locize-cli/compare/v6.0.5...v6.0.6) - 2019-09-26

- fallback for xliff files


## [6.0.5](https://github.com/locize/locize-cli/compare/v6.0.4...v6.0.5) - 2019-09-09

- fix file ending for strings resources


## [6.0.4](https://github.com/locize/locize-cli/compare/v6.0.3...v6.0.4) - 2019-09-09

- fix file ending for strings resources


## [6.0.3](https://github.com/locize/locize-cli/compare/v6.0.2...v6.0.3) - 2019-08-26

- locize sync: ability to handle multiple subfolders in path-mask


## [6.0.2](https://github.com/locize/locize-cli/compare/v6.0.1...v6.0.2) - 2019-08-24

- offer binaries for linux, macos and windows


## [6.0.1](https://github.com/locize/locize-cli/compare/v6.0.0...v6.0.1) - 2019-08-24

- locize sync/download: use path.sep instead of / (for windows users)


## 6.0.0

- locize sync/download: introduced --path-mask={{language}}/{{namespace}}


## 5.1.0

- locize rm: omitting the language argument will remove the key from all languages


## 5.0.0

- [BREAKING] gettext format: handle it closer to basic gettext format keeping msgid, msgid_plural when converting po -> json (locize UI) -> po
- for i18next use format po_i18next or gettext_i18next (gettext, po will be focused on non i18next cases)

## 4.8.3

- gettext format: don't assume i18next -> handle just plurals for non gettext_i18next format

## 4.8.2

- locize get: ability to get multiple keys

## 4.8.1

- gettext format: check if it's i18next format

## 4.8.0

- introduce (Java-)properties format

## 4.7.9

- update dependencies

## 4.7.8

- optimize convert to yaml-rails (check if should unflatten first)

## 4.7.7

- update dependencies

## 4.7.6

- sync and migrate: ignore "Unnecessary Request" advice

## 4.7.5

- xliff: file extenstion xlf

## 4.7.4

- xliff: added a first fallback for angular format

## 4.7.3

- locize sync: optimize csv multiline handling

## 4.7.1

- locize sync: fix --skip-delete parameter #24

## 4.7.0

- locize sync: introduce --skip-delete parameter #24

## 4.6.3

- optimize log message for remove key
- make sure download path exists

## 4.6.1

- filter namespaces based on options when reference-language-only is false (#21 #22) thanks to [Joe Holdcroft](https://github.com/joeholdcroft)

## 4.6.0

- introduce format command

## 4.5.5

- update dependencies

## 4.5.4

- locize sync: make it a bit safer #19

## 4.5.3

- locize sync: fix edge case comparison when local key and remote key are empty

## 4.5.2

- locize sync: fix callback in case of error

## 4.5.1

- added support for nested laravel format

## 4.5.0

- introduce language and namespace argument for sync command

## 4.4.2

- update dependencies

## 4.4.1

- update dependencies

## 4.4.0

- introduce laravel format

## 4.3.4

- fix strange error handling #16

## 4.3.3

- retry post call once on gateway timeout

## 4.3.2

- fix sync command when project/version is empty

## 4.3.1

- add possibility to download multiple namespaces in all languages

## 4.3.0

- add possibility to download only a dedicated namespace in all languages

## 4.2.3

- throttle the update requests in the sync command

## 4.2.1

- paged update for sync command

## 4.2.0

- introduce "reference-language-only" argument for sync command
- introduce "compare-modification-time" argument for sync command

## 4.1.0

- looking for the config file in the current directory first

## 4.0.1

- handle edge case for fluent format
- update deps

## 4.0.0

- refactoring of sync and download command
- introduce tmx format
- po files now get correct date values

## 3.15.0

- introduce --language-folder-prefix parameter for sync command

## 3.14.2

- catch edge case when file has no content

## 3.14.1

- ignore comments for fluent format
- update deps

## 3.14.0

- support fluent format

## 3.13.4

- fix gettext format

## 3.13.3

- fix yaml-rails format

## 3.13.2

- fix yaml-rails format nesting

## 3.13.1

- fix yaml-rails format

## 3.13.0

- support yaml-rails format

## 3.12.1

- do not delete hidden folders

## 3.12.0

- introduce delete-namespace

## 3.11.0

- introduce --update-values flag for sync command

## 3.10.0

- support for private published files

## 3.9.6

- support for HTML strings for Android #4

## 3.9.5

- fix a bug when adding and removing keys with the same sync call (keys are not added anymore to all languages)

## 3.9.4

- fix -c argument
- possibility to define env vars

## 3.9.3

- fix exit code on error in bin too

## 3.9.2

- fix exit code on error

## 3.9.1

- fix return of job object

## 3.9.0

- wait for async action for copy & publish version completes

## 3.8.0

- copy version
- publish version

## 3.7.3

- update dependencies

## 3.7.2

- update dependencies

## 3.7.1

- make sure we get a non-cached version of available languages request

## 3.7.0

- introduce sync command

## 3.6.0

- download resources as strings format

## 3.5.0

- download resources as gettext po format

## 3.4.3

- add defaults for download (when calling programmatically)

## 3.4.2

- update android-string-resource dependency

## 3.4.1

- ensure data is flatted for add

## 3.4.0

- add possibility to skip-empty namespaces

## 3.3.1

- sort keys for flat json export

## 3.3.0

- add additional csv format option for download

## 3.2.3

- update android-string-resource dependency

## 3.2.2

- update xliff dependency

## 3.2.1

- optimize error message handling

## 3.2.0

- migrate has a new option --replace

## 3.1.0

- download resources in different formats (json, flat, xliff2, xliff12, android)

## 3.0.1

- fixes path cleaning for non linux systems

## 3.0.0

- download now does not provide projectId and version (if called with version param) - so downloaded structure is more useful to i18next
- download now appends fileextension .json to the json files

## 1+2.x.x

- initial versions
