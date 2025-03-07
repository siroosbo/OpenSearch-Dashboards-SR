# CHANGELOG

Inspired from [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)

## [Unreleased]

### 💥 Breaking Changes

### Deprecations

### 🛡 Security

- [CVE-2022-37599] Bump loader-utils from `2.0.3` to `2.0.4` ([#3031](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3031)). Backwards-compatible fixes included in v2.6.0 and v1.3.7 releases.
- [CVE-2022-37603] Bump loader-utils from `2.0.3` to `2.0.4` ([#3031](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3031)). Backwards-compatible fixes included in v2.6.0 and v1.3.7 releases.
- [WS-2021-0638] Bump mocha from `7.2.0` to `10.1.0` ([#2711](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2711))
- Bump `joi` to v14 to avoid the possibility of prototype poisoning in a nested dependency ([#3952](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3952))

### 📈 Features/Enhancements

- Add plugin manifest config to define OpenSearch plugin dependency and verify if it is installed on the cluster ([#3116](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3116))
- Replace re2 with RegExp in timeline and add unit tests ([#3908](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3908))
- Hide any output from use_node checking for Node compatibility ([#4237](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4237))
- Add category option within groups for context menus ([#4144](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4144))
- [Saved Object Service] Add Repository Factory Provider ([#4149](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4149))
- [Multiple DataSource] Backend support for adding sample data ([#4268](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4268))

### 🐛 Bug Fixes

- [Chore] Update deprecated url methods (url.parse(), url.format()) ([#2910](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2910))
- Cleanup unused url ([#3847](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3847))

### 🚞 Infrastructure

- Re-enable CI workflows for feature branches ([#2908](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2908))
- Upgrade yarn version to be compatible with @opensearch-project/opensearch ([#3443](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3443))
- Add an achievement badger to the PR ([#3721](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3721))
- Upgrade the backport workflow ([#4343](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4343))

### 📝 Documentation

- [Doc] Add COMMUNICATIONS.md with info about Slack, forum, office hours ([#3837](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3837))
- [Saved Object Service] Adds design doc for new Saved Object Service Interface for Custom Repository [#3954](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3954)
- Add plugin development section in DEVELOPER_GUIDE.md ([#778](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3989))

### 🛠 Maintenance

- Removes `minimatch` manual resolution ([#3019](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3019))
- Upgrade `vega-lite` dependency from `4.17.0` to `^5.6.0` ([#3076](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3076)). Backwards-compatible version included in v2.5.0 release.
- Bump `js-yaml` from `3.14.0` to `4.1.0` ([#3770](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3770))
- Adding @ZilongX and @Flyingliuhub as maintainers. ([#4137](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4137))
- Add new MAINTAINERS to CODEOWNERS file. ([#4199](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4199))

### 🪛 Refactoring

- [Console] Remove unused ul element and its custom styling ([#3993](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3993))
- Fix EUI/OUI type errors ([#3798](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3798))
- Remove unused Sass in `tile_map` plugin ([#4110](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4110))
- [Table Visualization] Remove custom styling for text-align:center in favor of OUI utility class. ([#4164](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4164))
- Replace the use of `bluebird` in `saved_objects` plugin ([#4026](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4026))
- [Vis Colors] Update default color in TSVB to use `ouiPaletteColorBlind()[0]`([#4363](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4363))

### 🔩 Tests

## [2.8.0 - 2023-06-06](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.8.0)

### Deprecations

- Remove timeline application ([#3971](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3971))

### 🛡 Security

- [CVE-2023-2251] Bump `yaml` to `2.2.2` ([#3947](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3947))

### 📈 Features/Enhancements

- [Multiple Datasource] Support Amazon OpenSearch Serverless ([#3957](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3957))
- Add support for Node.js >=14.20.1 <19 ([#4071](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4071))
- Bundle Node.js 14 as a fallback for operating systems that cannot run Node.js 18 ([#4151](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4151))
- Enhance grouping for context menus ([#3924](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3924))

### 🐛 Bug Fixes

- [BUG] Fix bottom bar visibility using createPortal ([#3978](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3978))
- [Dashboards Listing] Fix listing limit to utilize `savedObjects:listingLimit` instead of `savedObjects:perPage` ([#4021](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4021))

### 🚞 Infrastructure

- Install chrome driver for functional tests from path set by environment variable `TEST_BROWSER_BINARY_PATH`([#3997](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3997))
- Add threshold to code coverage config to prevent workflow failures ([#4040](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4040))
- [CI] Skip checksum verification on OpenSearch snapshot for cypress tests ([#4188](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4188))

### 📝 Documentation

### 🛠 Maintenance

- Use `exec` in the CLI shell scripts to prevent new process creation ([#3955](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3955))

### 🪛 Refactoring

### 🔩 Tests

## [1.3.10 - 2023-05-18](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.7.0)

### 🛡 Security

- [CVE-2020-15366][1.x] Bump ajv from 4.11.8 to 6.12.6 ([#4035](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4035))
- [CVE-2022-48285][1.x] Bump jszip from 3.7.1 to 3.10.1 ([#4011](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4011))
- [CVE-2021-35065][1.x] Bump glob-parent from 6.0.0 to 6.0.2 ([#4005](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4005))
- [CVE-2022-25851][1.x] Bump jpeg-js from 0.4.1 to 0.4.4 ([#3860](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3860))
- [CVE-2022-25858][1.x] Bump terser from 4.8.0 to 4.8.1 ([#3786](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3786))
- [CVE-2021-23490][1.x] Bump parse-link-header from 1.0.1 to 2.0.0 ([#3820](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3820))
- [CVE-2021-3765][1.x] Bump validator from 8.2.0 to 13.9.0 ([#3753](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3753))
- [CVE-2022-25758][1.x] Bump scss-tokenizer from 0.3.0 to 0.4.3 ([#3789](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3789))
- [CVE-2021-3803][1.x] Bump nth-check from 1.0.2 to 2.0.1 ([#3745](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3745))
- Bump highlight.js from 9.18.5 to 10.7.3 to solve security concerns （[#4062](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4062))

### 📈 Features/Enhancements

- Add tooltip to help icon ([#3872](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3872))

### 🐛 Bug Fixes

### 📝 Documentation

- Update jest documentation links ([#3939](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3939))

### 🛠 Maintenance

- Add threshold to code coverage changes for project ([#4050](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4050))
- Temporarily hardcode chromedriver to 112.0.0 to enable all ftr tests ([#4039](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/4039))
- Update MAINTAINERS.md and CODEOWNERS ([#3938](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3938))
- Add opensearch-dashboards-docker-dev to .gitignore ([#3781](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3781))

### 🪛 Refactoring

### 🔩 Tests

## [2.7.0 - 2023-05-02](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.7.0)

### Deprecations

### 🛡 Security

- [CVE-2023-26486] Bump vega from `5.22.1` to `5.23.0` ([#3533](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3533))
- [CVE-2023-26487] Bump vega from `5.22.1` to `5.23.0` ([#3533](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3533))
- [CVE-2023-0842] Bump xml2js from `0.4.23` to `0.5.0` ([#3842](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3842))
- [Multi DataSource] Add private IP blocking validation on server side ([#3912](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3912))

### 📈 Features/Enhancements

- Add satisfaction survey link to help menu ([#3676](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3676))
- Add `osd-xsrf` header to all requests that incorrectly used `node-version` to satisfy XSRF protection ([#3643](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3643))
- [Dashboard] Add Dashboards-list integrations for Plugins ([#3090](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3090) )
- [Data] Add geo shape filter field ([#3605](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3605))
- [Doc Links] Add downgrade logic for branch in DocLinkService ([#3483](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3483))
- [Monaco editor] Add json worker support ([#3424](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3424))
- [Multiple DataSource] Allow create and distinguish index pattern with same name but from different datasources ([#3604](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3604))
- [Multiple DataSource] Integrate multiple datasource with dev tool console ([#3754](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3754))
- [Notifications] Add id to toast api for deduplication ([#3752](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3752))
- [UI] Add support for comma delimiters in the global filter bar ([#3686](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3686))
- [UI] Indicate that IE is no longer supported ([#3641](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3641))
- [Vega] Add Filter custom label for opensearchDashboardsAddFilter ([#3640](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3640))
- [VisBuilder] Add metric to metric, bucket to bucket aggregation persistence ([#3495](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3495))
- [VisBuilder] Add UI actions handler ([#3732](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3732))
- [VisBuilder] Add persistence to visualizations inner state ([#3751](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3751))

### 🐛 Bug Fixes

- Clean up and rebuild `@osd/pm` ([#3570](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3570))
- Omit adding the `osd-version` header when the Fetch request is to an external origin ([#3643](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3643))
- [Console] Fix/update documentation links in Dev Tools console ([#3724](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3724))
- [Console] Fix dev tool console autocomplete not loading issue ([#3775](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3775))
- [Console] Fix dev tool console run command with query parameter error ([#3813](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3813))
- [Table Visualization] Fix table rendering empty unused space ([#3797](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3797))
- [Table Visualization] Fix data table not adjusting height on the initial load ([#3816](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3816))
- [Timeline] Fix y-axis label color in dark mode ([#3698](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3698))
- [TSVB] Fix undefined serial diff aggregation documentation link ([#3503](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3503))
- [UI] Add clarifying tooltips to header navigation icons ([#3626](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3626))
- [VisBuilder] Fix multiple warnings thrown on page load ([#3732](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3732))
- [VisBuilder] Fix Firefox legend selection issue ([#3732](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3732))
- [VisBuilder] Fix type errors ([#3732](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3732))
- [VisBuilder] Fix indexpattern selection in filter bar ([#3751](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3751))

### 🚞 Infrastructure

- Use mirrors to download Node.js binaries to escape sporadic 404 errors ([#3619](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3619))
- [CI] Update NOTICE file, add validation to GitHub CI ([#3051](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3051))
- [CI] Reduce redundancy by using matrix strategy on Windows and Linux workflows ([#3514](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3514))
- [Darwin] Add support for Darwin for running OpenSearch snapshots with `yarn opensearch snapshot` ([#3537](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3537))

### 📝 Documentation

- Correct copyright date range of NOTICE file and notice generator ([#3308](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3308))
- Simplify the in-code instructions for upgrading `re2` ([#3328](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3328))
- [Doc] Improve DEVELOPER_GUIDE to make first time setup quicker and easier ([#3421](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3421))
- [Doc] Update DEVELOPER_GUIDE with added manual bootstrap timeout solution and max virtual memory error solution with docker ([#3764](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3764))
- [Doc] Add second command to install yarn step in DEVELOPER_GUIDE ([#3633](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3633))
- [Doc] Add docker dev set up instruction ([#3444](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3444))
- [Doc] Add docker files and instructions for debugging Selenium functional tests ([#3747](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3747))
- [Doc] Update SECURITY with instructions for nested dependencies and backporting ([#3497](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3497))
- [TSVB] Fix typo in TSVB README ([#3518](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3518))
- [UI Actions] Improve UI actions explorer ([#3614](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3614))

### 🛠 Maintenance

- Relax the Node.js requirement to `^14.20.1` ([#3463](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3463))
- Bump the version of Node.js installed by `nvm` to `14.21.3` ([#3463](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3463))
- Allow selecting the Node.js binary using `NODE_HOME` and `OSD_NODE_HOME` ([#3508](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3508))
- Remove the unused `renovate.json5` file ([#3489](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3489))
- Bump `styled-components` from `5.3.5` to `5.3.9` ([#3678](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3678))
- [Timeline] Update default expressions from `.es(*)` to `.opensearch(*)`. ([#2720](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2720))

### 🪛 Refactoring

- Remove automatic addition of `osd-version` header to requests outside of OpenSearch Dashboards ([#3643](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3643))
- [Console] Replace jQuery usage in console plugin with native methods ([#3733](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3733))
- [Doc Links] Clean up docs_link_service organization so that strings are in the right categories. ([#3685](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3685))
- [I18n] Fix Listr type errors and error handlers ([#3629](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3629))
- [Multiple DataSource] Refactor dev tool console to use opensearch-js client to send requests ([#3544](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3544))
- [Multiple DataSource] Present the authentication type choices in a drop-down ([#3693](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3693))
- [Table Visualization] Move format table, consolidate types and add unit tests ([#3397](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3397))

### 🔩 Tests

- Update caniuse to `1.0.30001460` to fix failed integration tests ([#3538](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3538))
- [Tests] Fix unit tests for `get_keystore` ([#3854](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3854))

## [1.3.9 - 2023-04-04](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/1.3.9)

### 🛡 Security

- [CVE-2022-2499] Resolve qs from 6.5.2 and 6.7.0 to 6.11.0 in 1.x ([#3451](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3451))
- [CVE-2020-36632] [REQUIRES PLUGIN VALIDATION] Bump flat from 4.1.1 to 5.0.2 ([#3539](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3539)). To the best of our knowledge, this is a non-breaking change, but if your plugin relies on `mocha` tests, validate that they still work correctly (and plan to migrate them to `jest` [in preparation for `mocha` deprecation](https://github.com/opensearch-project/OpenSearch-Dashboards/issues/1572).
- [CVE-2023-25653] Bump node-jose to 2.2.0 ([#3445](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3445))
- [CVE-2021-23807] Bump jsonpointer from 4.1.0 to 5.0.1 ([#3535](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3535))
- [CVE-2021-23424] Bump ansi-html from 0.0.7 to 0.0.8 ([#3536](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3536))
- [CVE-2022-24999] Bump express from 4.17.1 to 4.18.2 ([#3542](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3542))

### 📈 Features/Enhancements

- [I18n] Register ru, ru-RU locale ([#2817](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2817))

### 🐛 Bug Fixes

- [TSVB] Fix the link to "serial differencing aggregation" documentation ([#3503](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3503))

### 📝 Documentation

- [TSVB] Fix a spelling error in the README file ([#3518](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3518))
- Simplify the in-code instructions for upgrading `re2` ([#3328](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3328))
- [Doc] Improve DEVELOPER_GUIDE to make first time setup quicker and easier ([#3421](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3421))

### 🛠 Maintenance

- Update MAINTAINERS.md formatting and maintainer list ([#3338](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3338))
- Remove `github-checks-reporter`, an unused dependency ([#3126](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3126))
- [Version] Increment to 1.3.9 ([#3375](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3375))
- Remove the unused `renovate.json5` file ([3489](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3489))

## [2.6.0 - 2023-02-28](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.6.0)

### Deprecations

- [CVE-2020-36632] [REQUIRES PLUGIN VALIDATION] Bump flat from `4.1.1` to `5.0.2` ([#3419](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3419)). To the best of our knowledge, this is a non-breaking change, but if your plugin relies on `mocha` tests, validate that they still work correctly (and plan to migrate them to `jest` [in preparation for `mocha` deprecation](https://github.com/opensearch-project/OpenSearch-Dashboards/issues/1572).

### 🛡 Security

- [CVE-2022-37599] Bump loader-utils from `2.0.3` to `2.0.4` ([#3318](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3318))
- [CVE-2022-37603] Bump loader-utils from `2.0.3` to `2.0.4` ([#3318](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3318))
- [CVE-2022-25860] Bump simple-git from `3.15.1` to `3.16.0` ([#3345](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3345))
- [CVE-2022-25881] Resolve http-cache-semantics from `4.1.0` to `4.1.1` ([#3409](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3409))
- [Security] Bump hapi/statehood from `7.0.3` to `7.0.4` ([#3411](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3411))
- [CVE-2023-25166] Bump formula from `3.0.0` to `3.0.1` ([#3416](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3416))
- [CVE-2020-36632] [REQUIRES PLUGIN VALIDATION] Bump flat from `4.1.1` to `5.0.2` ([#3419](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3419)). To the best of our knowledge, this is a non-breaking change, but if your plugin relies on `mocha` tests, validate that they still work correctly (and plan to migrate them to `jest` [in preparation for `mocha` deprecation](https://github.com/opensearch-project/OpenSearch-Dashboards/issues/1572).
- [CVE-2023-25653] Bump node-jose from `2.1.1` to `2.2.0` ([#3445](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3445))
- [CVE-2022-24999] Resolve qs from `6.5.3` to `6.11.0` ([#3450](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3450))
- [CVE-2022-25758] Bump node-sass from `6.0.1` to `7.0.3` and sass-loader from `10.2.1` to `10.4.1` to bump scss-tokenizer from `0.2.3` to `0.4.3` ([#3455](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3455))
- [CVE-2020-24025] Bump node-sass from `6.0.1` to `7.0.3` ([#3455](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3455))

### 📈 Features/Enhancements

- Add disablePrototypePoisoningProtection configuration to prevent JS client from erroring when cluster utilizes JS reserved words ([#2992](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2992))
- [Multiple DataSource] Add support for SigV4 authentication ([#3058](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3058))
- [Multiple DataSource] Refactor test connection to support SigV4 auth type ([#3456](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3456))

### 🐛 Bug Fixes

- [Search Telemetry] Fix search telemetry's observable object that won't be GC-ed([#3390](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3390))
- [Region Maps] Add ui setting to configure custom vector map's size parameter([#3399](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3399))

### 🚞 Infrastructure

- Fix detection of Chrome's version on Darwin during CI ([#3296](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3296))

### 📝 Documentation

- [Docs] Fix documentation link for date math ([#3207](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3207))

### 🛠 Maintenance

- Bump `re2` and `supertest` ([#3018](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3018))
- Upgrade vega-tooltip to `0.30.0` to support custom tooltips ([#3359](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3359))
- Allow relaxing the Node.js runtime version requirement ([#3402](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3402))
- Make build scripts find and use the latest version of Node.js that satisfies `engines.node` ([#3467](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3467))
- Add `@opensearch-project/opensearch@^2.x` as dependency aliased as `@opensearch-project/opensearch-next` ([#3469](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3469))

### 🪛 Refactoring

### 🔩 Tests

- [BWC Tests] Add BWC tests for `2.6.0` ([#3356](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3356))
- Prevent primitive linting limitations from being applied to unit tests found under `src/setup_node_env` ([#3403](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3403))

## [1.3.8 - 2023-02-15](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/1.3.8)

### 🛡 Security

- [CVE-2022-25901] Bump supertest from 2.0.5 to 2.0.12 ([#3326](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3326))
- [CVE-2022-25860] Bump simple-git from 3.15.1 to 3.16.0 ([#3345](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3345))
- [CVE-2022-46175] Bump json5 version from 1.0.1 and 2.2.1 to 1.0.2 and 2.2.3 ([#3201](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3201))
- [CVE-2022-25912] Bump simple-git from 3.4.0 to 3.15.0 ([#3036](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3036))
- Bump decode-uri-component from 0.2.0 to 0.2.2 ([#3009](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3009))

### 🐛 Bug Fixes

- [BUG] Fixes misleading embeddable plugin error message ([#3043](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3043))
- [BUG] Trim trailing slashes before checking no-restricted-path rule ([#3020](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3020))

### 🚞 Infrastructure

- Lock workflow tests to Chrome and ChromeDriver 107 as the last combination that run on Node.js v10 ([#3299](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3299))
- Update yarn timeout for GitHub workflow on Windows ([#3118](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3118))
- Add Windows CI to the GitHub workflow ([#2966](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2966))

### 📝 Documentation

- Fix documentation link for date math ([#3207](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3207))

### 🔩 Tests

- [BWC] Updates to BWC tests ([#1190](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/1190))
- Automates chromedriver version selection for tests ([#2990](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2990))

## [2.5.0 - 2023-01-25](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.5.0)

### 🛡 Security

- Introduce guidelines for reporting vulnerable dependencies ([#2674](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2674))
- Bump decode-uri-component from 0.2.0 to 0.2.2 ([3009](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3009))
- [CVE-2022-25912] Bump simple-git from 3.4.0 to 3.15.0 ([#3036](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3036))
- [CVE-2022-35256] Bump node version from 14.20.0 to 14.20.1 [#3166](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3166))
- [CVE-2022-46175] Bump json5 version from 1.0.1 and 2.2.1 to 1.0.2 and 2.2.3 ([#3201](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3201))

### 📈 Features/Enhancements

- [CLI] Enhance `yarn opensearch snapshot` to facilitate installing plugins on an OpenSearch cluster ([#2734](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2734))
- [I18n] Register ru, ru-RU locale ([#2817](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2817))
- [Multi DataSource] Introduce validation of new or modified connections to external data sources ([#2973](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2973), [#3110](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3110))
- [VisBuilder] Create global data persistence for VisBuilder ([#2896](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2896))
- [VisBuilder] Introduce Redux store persistence ([#3088](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3088))
- [VisBuilder] Enable persistence for app filter and query without using state containers ([#3100](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3100))
- [Data] Make the newly created configurations get added to beginning of the `aggConfig` array when using `createAggConfig` ([#3160](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3160))
- [Optimizer] Increase the amount of time an optimizer worker is provided to exit before throwing an error ([#3193](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3193))

### 🐛 Bug Fixes

- Upgrade the `del` library to fix a race condition on macOS ([#2847](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2873))
- [Table Visualization] Fix a problem with table visualizations that prevented URLs from being rendered correctly ([#2918](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2918))
- [Embeddable] Fix a misleading error message ([#3043](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3043))
- Fix rendering issues when the obsolete `v8 (beta)` theme was carried over by an upgrade ([#3045](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3045))
- [Multi Datasource] Replace the mock URL in tests ([#3099](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3099))
- [CI] Increase Yarn's timeout for installing dependencies in workflows ([#3118](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3118))
- [VisBuilder] Fix an issue that caused a crash when certain filters were added to a table visualization ([#3210](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3210))
- [VisBuilder] Fix errors throws when pipeline aggregations, like cumulative sum, were used in VisBuilder ([#3137](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3137))
- [Region Maps] Fix the problem of join fields being unusable ([#3213](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3213))
- [Multi DataSource] Update test connection button text ([#3247](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3247))

### 🚞 Infrastructure

- Bump the version of the `2.x` branch to 2.5.0 ([#2884](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2884))
- [CI] Create workflows that test and build on Windows ([#2966](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2966))
- [CI] Automate ChromeDriver installation for running functional tests ([#2990](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2990))
- Create the Release Notes for the 1.3.7 release ([#3066](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3066))
- [CI] Improve workflows by retaining Yarn's cache folder ([#3194](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3194))

### 📝 Documentation

- Publish the release runbook ([#2533](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2533))
- Document the capabilities of the Charts plugin and its current usage ([#2695](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2695))
- Document the correct version selection switch in `@osd/plugin-helpers` ([#2810](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2810))
- Document the global query persistence ([#3001](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3001))
- Document data persistence for plugins ([#3081](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3081))

### 🪛 Refactoring

- [VisBuilder] Extend the use of i18n ([#2867](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2867))
- [Console] Switch to using `core.http` when calling OSD APIs in console ([#3080](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3080))
- [Table Visualization] Refactor table visualization using React and DataGrid component ([#2863](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2863))

### 🛠 Maintenance

- Remove an unused dependency on `github-checks-reporter` ([#3126](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3126))
- Introduce `vega-lite@5`, aliased as `vega-lite-next` ([#3151](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3151))

### 🔩 Tests

- Enable retrying of flaky tests ([#2967](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2967))
- Enhance cross-platform testing of plugin installation on cluster snapshots ([#2994](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2994))
- [Tests] Bump `chromedriver` to v107 ([#3017](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3017))
- [CI] Disable the execution of the Build and Test workflow when the changes are limited to the docs folder ([#3197](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3197))
- Correct the linting logic for `no-restricted-path` to ignore trailing slashes ([#3020](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3020))
- [VisBuilder] Create unit tests for field utilities ([#3211](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3211))

## [2.4.1 - 2022-12-14](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.4.1)

### 🐛 Bug Fixes

- Update `leaflet-vega` and fixed its usage ([#3005](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3005))

### 🔩 Tests

- Correct the linting logic for `no-restricted-path` to ignore trailing slashes ([#3020](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3020))

## [1.3.7 - 2022-12-14](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/1.3.7)

### 🛡 Security

- [CVE-2022-0144] Bump shelljs from 0.8.4 to 0.8.5 ([#2511](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2511))
- [Legacy Maps Plugin] Prevent reverse-tabnabbing ([#2540](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2540))
- [CVE-2022-3517] Bump minimatch from 3.0.4 to 3.0.5 and [IBM X-Force ID: 220063] unset-value from 1.0.1 to 2.0.1 ([#2640](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2640))
- [CVE-2022-0155] Bump follow-redirects to 1.15.2 ([#2653](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2653))
- [CVE-2022-0536] Bump follow-redirects to 1.15.2 ([#2653](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2653))
- [CVE-2021-24033] Remove storybook package ([#2660](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2660))
- [CVE-2021-42740] Remove storybook package ([#2660](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2660))
- [CVE-2022-23647] Bump prismjs to 1.29.0 ([#2668](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2668))
- [CVE-2022-37599] Bump loader-utils to 2.0.4 ([#2995](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2995))
- [CVE-2022-37603] Bump loader-utils to 2.0.4 ([#2995](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2995))

### 📈 Features/Enhancements

- [Windows] Facilitate building and running OSD and plugins on Windows platforms ([#2601](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2601))
- [Windows] Add helper functions to work around the differences of platforms ([#2681](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2681))
- [Windows] Add `@osd/cross-platform` package to standardize path handling across platforms ([#2703](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2703))

### 🐛 Bug Fixes

- [Chore] Visualize link fix [#2395](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2395)
- [BUG] Fix suggestion list cutoff issue ([#2607](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2607))
- Remove Leftover X Pack references ([#2638](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2638))
- Bump `del` version to fix MacOS race condition ([#2847](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2873))
- Temporary workaround for task-kill exceptions on Windows when it is passed a pid for a process that is already dead ([#2842](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2842))
- [Build] Fixed "Last Access Time" not being set by `scanCopy` on Windows ([#2964](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2964))
- Update `leaflet-vega` and fix its usage ([#3005](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/3005))

### 🚞 Infrastructure

- Update backport custom branch name to utilize head template ([#2766](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2766))

### 📝 Documentation

- Add the release runbook to RELEASING.md ([#2533](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2533))
- Security-CVEs fixes guidelines [#2674](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2674)
- Correct README and help command of osd-plugin-helpers ([#2810](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2810))

### 🛠 Maintenance

- Increment version to 1.3.7 [#2528](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2528)

### 🔩 Tests

- Bump `chromedriver` to 106 to fix function test fail issue [#2514](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2514)
- Fix incorrect validation of time values in JUnit Reporter ([#2965](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2965))

## [2.4.0 - 2022-11-15](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/2.4.0)

### 🛡 Security

- Bump percy-agent to use non-beta version ([#2415](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2415))
- Use a forced CSP-compliant interpreter with Vega visualizations ([#2352](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2352))
- [CVE-2022-33987] Bump makelogs to remove dependency on got ([#2801](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2801))
- [CVE-2022-33987] Upgrade geckodriver to 3.0.2 ([#2166](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2166))
- [CVE-2022-3517] Bump minimatch to 3.0.5 and [IBM X-Force ID: 220063] unset-value to 2.0.1 ([#2640](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2640))
- [CVE-2022-37601] Bump loader-utils to 2.0.3 ([#2706](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2706))
- [GMS-2022-4708] Resolve sub-dependent d3-color version and potential security issue ([#2454](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2454))
- [Legacy Maps] Prevent reverse-tabnabbing ([#2540](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2540))
- [WS-2022-0284] [WS-2022-0280] Bump moment-timezone from 0.5.34 to 0.5.37 ([#2361](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2361))
- [Multi DataSource] Prevent spell-checking the password fields ([#2818](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2818))

### 📈 Features/Enhancements

- Add extension point in saved object management to register namespaces and show filter ([#2656](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2656))
- Add updated_at column to Saved Objects' tables ([#1218](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/1218))
- Change the links in the visualize plugin to use `href` rather than `onClick` ([#2395](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2395))
- Improve Discover field summaries ([#2391](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2391))
- Remove Add Integration button ([#2723](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2723))
- [Multi DataSource] Add data source column into index pattern table ([#2542](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2542))
- [Multi DataSource] Add data source config to opensearch-dashboards-docker ([#2557](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2557))
- [Multi DataSource] Add data source signing support ([#2510](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2510))
- [Multi DataSource] Add experimental callout for index pattern section ([#2523](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2523))
- [Multi DataSource] Address UX comments on Data source list and create page ([#2625](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2625))
- [Multi DataSource] Apply get indices error handling in step index pattern ([#2652](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2652))
- [Multi DataSource] Display error toast for create index pattern with data source ([#2506](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2506))
- [Multi DataSource] Make text content dynamically translated & update unit tests ([#2570](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2570))
- [Multi DataSource] Support legacy client for data source ([#2204](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2204))
- [Multi DataSource] UX enhancement on Data source management creation page ([#2051](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2501))
- [Multi DataSource] UX enhancement on Data source management stack ([#2521](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2521))
- [Multi DataSource] UX enhancement on Index Pattern management stack ([#2505](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2505))([#2527](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2527))
- [Multi DataSource] UX enhancement on Update stored password modal for Data source management stack ([#2532](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2532))
- [Plugin Helpers] Facilitate version changes ([#2398](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2398))
- [VisBuilder] Add an experimental table visualization in vis builder ([#2705](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2705))
- [VisBuilder] Add field summary popovers ([#2682](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2682))
- [VisBuilder] Add index pattern info when loading embeddable ([#2363](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2363))
- [VisBuilder] Add state validation before dispatching and loading ([#2351](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2351))
- [VisBuilder] Change VisBuilder flag for docker config ([#2804](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2804))
- [VisBuilder] Change classname prefix wiz to vb ([#2581](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2581/files))
- [VisBuilder] Change save object type, wizard id and name to visBuilder ([#2673](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2673))
- [VisBuilder] Change wizard to vis_builder in file names and paths ([#2587](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2587))
- [VisBuilder] Create a new wizard directly on a dashboard ([#2384](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2384))
- [VisBuilder] Edit wizard directly on dashboard ([#2508](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2508))
- [VisBuilder] Enable VisBuilder by default ([#2725](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2725))
- [VisBuilder] Rename wizard on save modal and visualization table ([#2645](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2645))
- [VisBuilder] Rename wizard to visBuilder in class name, type name and function name ([#2639](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2639))
- [VisBuilder] Rename wizard to visBuilder in i18n id and formatted message id ([#2635](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2635))
- [Windows] Add cross-platform helpers ([#2681](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2681))
- [Windows] Consume `@osd/cross-platform` package to standardize path handling across platforms ([#2703](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2703))
- [Windows] Facilitate building and running OSD and plugins on Windows platforms ([#2601](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2601))

### 🐛 Bug Fixes

- Fix management app breadcrumb error ([#2344](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2344))
- Fix suggestion list cutoff issue ([#2607](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2607))
- Remove Leftover X Pack references ([#2638](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2638))
- [Multi DataSource] Add data source param to low-level search call in Discover ([#2431](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2431))
- [Multi DataSource] Address UX comments on Edit Data source page ([#2629](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2629))
- [Multi DataSource] Address UX comments on index pattern management stack ([#2611](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2611))
- [Multi DataSource] Enhance data source error handling ([#2661](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2661))
- [Multi DataSource] Skip data source view in index pattern step when default is chosen ([#2574](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2574))
- [Multi DataSource] Update default audit log path ([#2793](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2793))
- [Save Object Aggregation View] Fix for export all after scroll count response changed ([#2696](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2696))
- [VisBuilder] Add additional aggregation parameters to Vislib charts (Bar, Line and Area) ([#2610](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2610))
- [VisBuilder] Add missing test subject property of `DisabledVisualization` ([#2610](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2610))
- [VisBuilder] Fix Date Histogram auto bounds showing per 0 millisecond ([#2632](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2632))
- [VisBuilder] Fix Histogram updating bounds when date range updates ([#2632](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2632))
- [VisBuilder] Fix auto bounds for time-series bar chart visualization ([2401](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2401))
- [VisBuilder] Fix broken UX after switching index pattern while editing an aggregation ([#2632](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2632))
- [VisBuilder] Fix rendering issues with time series for new chart types ([#2309](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2309))
- [VisBuilder] Fix the missing `Last Updated` timestamp in visualization list ([#2628](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2628))
- [VisBuilder] Fix visualization shift when editing an aggregation ([2401](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2401))
- [VisBuilder] Rename "Histogram" to "Bar" in visualization type picker ([2401](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2401))
- [Table Visualization] Fix an issue preventing sorting the first column ([#2828](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2828))
- Temporary workaround for task-kill exceptions on Windows when it is passed a pid for a process that is already dead ([#2842](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2842))

### 🚞 Infrastructure

- Add CHANGELOG.md and related workflows ([#2414](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2414))
- Update WhiteSource scans to ignore Backward Compatibility artifacts in `cypress` ([#2408](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2408))
- [CI] Add Backward Compatibility tests for 2.4.0 ([#2393](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2393))
- [CI] Add path ignore for markdown files ([#2312](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2312))
- [CI] Prevent backport workflow from running on unmerged PRs ([#2746](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2746))
- [CI] Run functional test repo as workflow ([#2503](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2503))
- [CI] Update backport custom branch name ([#2766](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2766))
- [CI] Update backport workflow to ignore changelog conflicts ([#2729](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2729))

### 📝 Documentation

- Add CHANGELOG.md and Release Notes for 2.4.0 ([#2809](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2809))
- Add README.md for `dataSource` and `dataSourceManagement` plugins ([#2448](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2448))
- Add README.md for saving index pattern relationship ([#2276](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2276))
- Remove a repeated "to" from the README.md file ([#2403](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2403))
- Update functional testing information in TESTING.md ([#2492](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2492))
- [Multi DataSource] Add design documents of multiple data source feature [#2538](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2538)
- [Multi DataSource] Add sample configuration for multi data source to the yml template ([#2428](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2428))
- [Multi DataSource] Tweak multiple data source design doc ([#2724](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2724))
- [Multi DataSource] Update MD data source documentation link ([#2693](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2693))

### 🔩 Tests

- Update caniuse to fix failed integration tests ([#2322](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2322))
- [Multi DataSource] Add unit test coverage for Update Data source management stack ([#2567](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2567))
- [VisBuilder] Enable VisBuilder cypress tests ([#2728](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2728))

### 🛠 Maintenance

- Add @zengyan-amazon as a maintainer ([#2419](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2419))
- Increment from 2.3 to 2.4. ([#2295](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2295))
- Add CHANGELOG.md for 2.4.0 ([#2809](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2809))

## [1.3.6 - 2022-10-06](https://github.com/opensearch-project/OpenSearch-Dashboards/releases/tag/1.3.6)

### 🛡 Security

- [CVE-2021-3807] Resolves ansi-regex to v5.0.1 ([#2425](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2425))
- [CVE-2022-23713] Handle invalid query, index and date in vega charts filter handlers ([#1932](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/1932))
- Use a forced CSP-compliant interpreter with Vega visualizations ([#2352](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2352))
- Bump moment-timezone from 0.5.34 to 0.5.37 ([#2361](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2361))

### 📈 Features/Enhancements

- Custom healthcheck with filters ([#2232](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2232), [#2277](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2277)). To configure see example in [config/opensearch_dashboards.yml](https://github.com/opensearch-project/OpenSearch-Dashboards/blob/6e2ec97459ae179c86201c611ce744c2c24ce150/config/opensearch_dashboards.yml#L44-L46)

### 🚞 Infrastructure

- Add CHANGELOG.md and related workflows ([#2414](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2414))
- Extends plugin-helpers to be used for automating version changes ([#2398](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2398),[#2486](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2486))

### 🛠 Maintenance

- Version Increment to 1.3.6 ([#2420](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2420))

### 🔩 Tests

- Update caniuse to fix failed integration tests ([#2322](https://github.com/opensearch-project/OpenSearch-Dashboards/pull/2322))
