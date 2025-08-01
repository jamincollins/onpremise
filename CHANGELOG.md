# Changelog

## 25.7.0

### Various fixes & improvements

- feat: Swap `trace-view-v1` feature flag with `visibility-explore-view` (#3801) by @aldy505
- fix: set harakiri Django option to 30s (#3792) by @aldy505
- feat(images):Cutover images to ghcr (#3800) by @hubertdeng123
- docs: encourage community patches (#3794) by @aldy505
- feat: run EAP-related containers (#3778) by @aldy505
- feat(uptime): Enable uptime in self-hosted (#3787) by @evanpurkhiser
- feat: make `system.secret-key` configurable from environment variables (#3783) by @aldy505
- ci: run tests on arm64 (#3750) by @aldy505

## 25.6.2

### Various fixes & improvements

- fix: Increase timeout for flakey test (#3781) by @tobias-wilfert
- chore: provide detailed note for sentry endpoint settings (#3780) by @aldy505

## 25.6.1

### Various fixes & improvements

- fix(taskworker) Remove num-brokers (#3769) by @markstory
- feat: enable customization sentry DSN endpoint (#3747) by @yildizozgur
- ref(js-assets): Simplify how we call nginx container (#3761) by @BYK
- Revert "fix(vroom): Explicitly set PROFILES_DIR for upcoming change" (#3760) by @hubertdeng123
- fix(vroom): Explicitly set PROFILES_DIR for upcoming change (#3759) by @BYK

## 25.6.0

### Various fixes & improvements

- enable shell linter for more scripts (#3748) by @doc-sheet
- feat: migrate to arm64-compatible smtp image (#3746) by @ezhevita
- Introduce patches with external kafka (#3521) by @aldy505
- add shellcheck action to lint bash scripts (#3710) by @doc-sheet
- tests: Install version 2.x of Python SDK (#3745) by @sentrivana
- feat(features): enable continuous profiling (#3742) by @aldy505
- feat: Add taskbroker + worker + scheduler (#3738) by @markstory
- fix(profiles): Run the profile chunks consumer (#3739) by @phacops
- chore: prune removed feature flags on main repository (#3731) by @aldy505
- remove index workaround (#3730) by @asottile-sentry
- Make usage of Python SDK future proof (#3714) by @antonpirker

## 25.5.1

### Various fixes & improvements

- Add missing lib script to sentry-admin.sh (#3693) by @djakielski
- chore: cleanup obsolete feature flags (#3701) by @doc-sheet

## 25.5.0

### Various fixes & improvements

- build(deps): bump actions/create-github-app-token from 2.0.2 to 2.0.6 (#3690) by @dependabot
- Resolve datetime deprecation warnings (#3686) by @emmanuel-ferdman
- ref: remove SENTRY_USE_BIG_INTS (always True) (#3687) by @asottile-sentry

## 25.4.0

### Stand-alone Docker Compose Fixes

By: @aminvakil (#3658, #3654)

### Various fixes & improvements

- chore(relay): specify spool.enveloppe.max_backpressure_memory_percent configuration for handling relay's failing healthcheck (#3635) by @aldy505
- build(deps): bump actions/create-github-app-token from 1.12.0 to 2.0.2 (#3649) by @dependabot
- build(deps): bump actions/create-github-app-token from 1.11.7 to 1.12.0 (#3639) by @dependabot
- Minimum requirements for 'errors-only' profile (#3634) by @madest92
- build(deps): bump actions/create-github-app-token from 1.11.6 to 1.11.7 (#3632) by @dependabot
- feat(sentry): add dynamic sampling feature to config (#3631) by @aldy505
- docs(config): add example config for Google Auth (#3623) by @junsung-cho
- fix: js-sdk directory/file permission should be set correctly (#3616) by @aldy505
- feat(features): enable session replay canvas (#3619) by @aldy505

## 25.3.0

### Various fixes & improvements

- feat(features): enable trace view (#3617) by @aldy505
- feat: provide monitoring-related configurations (#3611) by @aldy505
- Enforce license compliance only on getsentry repository (#3606) by @aminvakil
- Fix unbound variable error in install script (#3601) by @brettdh
- Add --short to docker-compose version (#3605) by @aminvakil
- ref: Less complicated docker compose detection (#3604) by @BYK
- Use docker-compose if version is gte docker compose (#3595) by @aminvakil
- build(deps): bump actions/create-github-app-token from 1.11.3 to 1.11.6 (#3598) by @dependabot
- build(deps): bump getsentry/action-release from 1 to 3 (#3599) by @dependabot
- Bump docker-compose 2.33.1 (#3597) by @aminvakil
- refactor: move system.url-prefix under systems settings section (#3588) by @leeoocca

## 25.2.0

### Various fixes & improvements

- build(deps): bump actions/create-github-app-token from 1.11.2 to 1.11.3 (#3569) by @dependabot
- feat: merge `.env` and `.env.custom` file during installation (#3564) by @aldy505
- build(deps): bump actions/create-github-app-token from 1.11.1 to 1.11.2 (#3561) by @dependabot
- feat: Require both inputs to be set on action (#3554) by @BYK
- ref: Simpler and more accurate cache keys (#3553) by @BYK
- Hand off open-source to dev-infra (#3549) by @chadwhitacre
- ci: Remove obsolete `dcr up -w` from import test (#3544) by @BYK
- fix: github.action_path may not have trailing slash (#3547) by @BYK
- chore: Remove upgrade test (#3541) by @hubertdeng123
- fix: Use correct path for get compose action (#3539) by @hubertdeng123
- fix: Caching of sentry migrations should cover additional folders (#3542) by @hubertdeng123
- ci: Move self-contained action reference to master branch (#3538) by @BYK
- breaking: Upgrade min Compose version to 2.23.2 (#3535) by @BYK
- ci: Even better cache keys and granular caching (#3534) by @BYK
- test: Reorganize backup/restore tests for speed and reliability (#3537) by @BYK

## 25.1.0

### Various fixes & improvements

- ci: Use generic Docker volume cache action (#3524) by @BYK
- ci: Less volatile cache keys (#3522) by @BYK
- docs: include regular env file on wrap-up (#3523) by @aldy505
- ci: Faster and smarter backup/restore tests (#3516) by @BYK
- fix: Fix the new e2e action to be portable (#3520) by @BYK
- ci: Move e2e test action into the repo (#3519) by @BYK
- ci: Only test on compose 2.26 w/ customizations (#3506) by @BYK
- ci: Skip DB ops during install completely on cache hit (#3496) by @BYK
- chore: Remove everything zookeeper (#3499) by @hubertdeng123
- ci: Cache postgres volume after first migration (#3488) by @BYK
- fix: Remove the extra space in the log file names (#3212) by @melnele
- ref(snuba): Combine bootstrap & migrate for faster bootstrap (#3491) by @BYK
- ref(geoip): Remove geoipupdate from compose (#3490) by @BYK
- build(deps): bump actions/create-github-app-token from 1.11.0 to 1.11.1 (#3492) by @dependabot

## 24.12.1

### Various fixes & improvements

- chore: clearer message for errors-only mode (#3487) by @aldy505
- chore(relay): provide opt-in max_memory_percent config as workaround for failing healthcheck (#3486) by @aldy505
- fix(nginx): _assets should rewrite to _static/sentry/dist (#3483) by @BYK

## 24.12.0

- No documented changes.

## 24.11.2

### Various fixes & improvements

- fix(redis): Actually use custom config (#3459) by @BYK
- feat(release): Replace release bot with GH app (#3458) by @Jeffreyhung
- chore(issue-template): ask for machine specification and provide link to security policy (#3447) by @aldy505
- add sentry/backup.json to gitignore (#3450) by @niklassc7
- ref: remove suggested fix (#3446) by @aldy505

## 24.11.1

### Various fixes & improvements

- fix(redis): Use a safer eviction rule (#3432) by @BYK
- feat: add Redis configuration for improved memory management (#3427) by @Hassanzadeh-sd
- build(deps): bump codecov/codecov-action from 4 to 5 (#3429) by @dependabot

## 24.11.0

### Various fixes & improvements

- feat(healthcheck): Improve redis healthcheck (#3422) by @hubertdeng123
- fix: missing mime types and turning off autoindex for js-sdk endpoint (#3395) by @aldy505
- fix: Use js.sentry-cdn.com for JS SDK downloads (#3417) by @BYK
- fix(loader): provide js sdk assets from 4.x (#3415) by @aldy505
- Revert "Revert "ref(feedback): remove issue platform flags after releasing issue types"" (#3403) by @BYK
- Revert "ref(feedback): remove issue platform flags after releasing issue types" (#3402) by @BYK
- ref(feedback): remove issue platform flags after releasing issue types (#3397) by @aliu39
- fix(sentry-admin): Do not wait for command finish to display output (#3390) by @Makhonya

## 24.10.0

### Various fixes & improvements

- chore: Disable codecov for master/release branches (#3384) by @hubertdeng123
- chore: replace old URLs of the repo with the new docs (#3375) by @victorelec14
- ref: span normalization allowed host config (#3245) by @aldy505
- docs: explicitly specify `mail.use-{tls,ssl}` is mutually exclusive (#3368) by @aldy505
- ref: allow hosted js sdk bundles (#3365) by @aldy505
- fix(clickhouse): Allow nullable key (#3354) by @nikhars

## 24.9.0

### Various fixes & improvements

- docs: link to develop docs (#3307) by @joshuarli
- fix: more leeway for minimum RAM (#3290) by @joshuarli
- Mandate minimum requirements for ram/cpu (#3275) by @hubertdeng123
- ref(feedback): cleanup topic rollout option (#3276) by @aliu39
- Update release template (#3270) by @hubertdeng123

## 24.8.0

### Various fixes & improvements

- Migrate to zookeeper-less kafka  (#3263) by @hubertdeng123
- Revert "ref(feedback): cleanup topic rollout option" (#3262) by @aliu39
- ref(feedback): cleanup topic rollout option (#3256) by @aliu39
- Remove cdc and wal2json and use the default postgres entrypoint (#3260) by @beezz
- add `-euo pipefail` to enhance-image.example.sh (#3246) by @asottile-sentry
- remove python-dev (#3242) by @asottile-sentry
- feat: enable user feedback feature (#3193) by @aldy505
- Use CDN by default for JS SDK Loader (#3213) by @stayallive

## 24.7.1

### Various fixes & improvements

- Fix: errors only config flag (#3220) by @hubertdeng123
- Add errors only self-hosted infrastructure (#3190) by @hubertdeng123
- feat(generic-metrics): Add gauges to docker compose, re-try (#3177) by @ayirr7

## 24.7.0

### Various fixes & improvements

- Check postgres os before proceeding with install (#3197) by @hubertdeng123
- Update sentry-admin.sh to select its own working directory (#3184) by @theoriginalgri
- feat: add insights feature flags (#3152) by @aldy505
- feat(relay): Forward /api/0/relays/* to inner relays (#3144) by @iambriccardo

## 24.6.0

### Various fixes & improvements

- Use general kafka topic creation in self-hosted (#3121) by @hubertdeng123
- Use non-alpine postgres (#3116) by @hubertdeng123
- Bump Python SDK version used in tests (#3108) by @sentrivana

## 24.5.1

### Various fixes & improvements

- Update consumer flags (#3112) by @hubertdeng123
- feat: Add crons task consumers  (#3106) by @wedamija
- Update minimum docker compose requirement (#3078) by @JannKleen
- Different approach to editing permissions of docker volumes (#3084) by @hubertdeng123
- ref(spans): Add new feature flags needed (#3092) by @phacops
- chore: Add comment explaining the one liner in clickhouse config (#3085) by @hubertdeng123
- Fix install: use dynamic docker root dir instead of hardcoded one (#3064) by @boutetnico
- Typo in config.example.yml (#3063) by @luchaninov

## 24.5.0

### Various fixes & improvements

- fix: Make docker volume script respect compose project name (#3039) by @hubertdeng123
- remove ref to skip writes (#3041) by @john-z-yang
- Add clickhouse healthchecks to upgrade (#3024) by @hubertdeng123
- Upgrade clickhouse to 23.8 (#3009) by @hubertdeng123
- fix: use nginx realip module (#2977) by @oioki
- Add upgrade test (#3012) by @hubertdeng123
- Bump kafka and zookeeper versions (#2988) by @hubertdeng123

## 24.4.2

### Various fixes & improvements

- Edit test file name (#3002) by @hubertdeng123
- Revert "Sampling: Run e2e tests every 5 minutes" (#2999) by @hubertdeng123
- Fix master test failures (#3000) by @hubertdeng123
- Sampling: Run e2e tests every 5 minutes (#2994) by @hubertdeng123
- Tweak e2e test github action (#2987) by @hubertdeng123
- fix(performance): Add spans-first-ui flag to enable starfish/performance module views in ui (#2993) by @edwardgou-sentry
- Bump docker compose version in CI (#2980) by @hubertdeng123
- Upgrade postgres to 14.11 (#2975) by @mdtro
- Add workstation configuration (#2968) by @azaslavsky

## 24.4.1

### Various fixes & improvements

- chore(deps): bump memcached and redis to latest patch versions (#2973) by @mdtro
- Use docker compose exec to create additional kafka topics (#2904) by @saz
- Add example to docker compose version in problem report (#2959) by @edgariscoding
- Port last integration tests to python (#2966) by @hubertdeng123

## 24.4.0

### Various fixes & improvements

- Use python for e2e tests (#2953) by @hubertdeng123
- feat: adds group attributes consumer (#2927) by @scefali
- fix(spans): Adds organizations:standalone-span-ingestion flag to default config (#2936) by @edwardgou-sentry
- Bump ubuntu version for tests (#2923) by @hubertdeng123
- Write Customization tests in python (#2918) by @hubertdeng123
- feat(clickhouse): Added max_suspicious_broken_parts to the config.xml (#2853) by @victorelec14
- Port backup tests to python (#2907) by @hubertdeng123
- Fix defunct java processes (#2914) by @hubertdeng123
- Integration tests in python (#2892) by @hubertdeng123
- feat: run outcomes-billing consumer (#2909) by @lynnagara
- Remove duplicate feature flags (#2899) by @JannKleen

## 24.3.0

### Various fixes & improvements

- feat(spans): Ingest spans (#2861) by @phacops
- Integration test improvements (#2858) by @hubertdeng123
- increase postgres max_connections above 100 connections (#2740) by @erfantkerfan
- deps: bump maxmind/geoipupdate to 6.1.0 (#2859) by @victorelec14
- Enable proxy buffering in nginx (#2844) by @RexTim
- Add snuba rust consumers (#2831) by @hubertdeng123
- simplify if for open-ai-suggestion (#2732) by @LvckyAPI
- Upgrade to FSL-1.1 (#2835) by @chadwhitacre
- chore: provide clearer csrf url example (#2833) by @aldy505
- chore: Use django ORM to perform sql commands (#2827) by @hubertdeng123
- revert changes in 3067683f6c0e1c6dd9ceb72cb5155c1dbf3bf501 (#2829) by @hubertdeng123
- use rust consumers in self-hosted (3067683f) by @hubertdeng123

## 24.2.0

### Various fixes & improvements

- Bump nginx version (#2797) by @hubertdeng123
- build(deps): bump pre-commit/action from 3.0.0 to 3.0.1 (#2788) by @dependabot
- Tweak postgres indexing fix (#2792) by @hubertdeng123
- fix: DB migration script (#2779) by @hubertdeng123

## 24.1.2

### Various fixes & improvements

- Check memcached backend in Django (#2778) by @chadwhitacre
- Fix groupedmessage indexing error (#2777) by @hubertdeng123
- build(deps): bump actions/setup-python from 4 to 5 (#2644) by @dependabot
- feat: provide csrf settings information for sentry config (#2762) by @aldy505
- Fix apt config generation when http_proxy is set (#2725) (#2734) by @lemrouch

## 24.1.1

### Various fixes & improvements

- Revert "Move open ai key from env variables" (#2724) by @hubertdeng123
- Fix cache error self hosted (#2722) by @hubertdeng123

## 24.1.0

### Various fixes & improvements

- Enable crons (#2712) by @hubertdeng123
- Parameterize backup restore script (#2412) by @hubertdeng123
- Run tests only on getsentry repository (#2681) by @aminvakil
- Tweak the template now that we can see it (#2670) by @chadwhitacre
- Nginx client request body is buffered to a temporary file (#2630) by @zKoz210

## 23.12.1

### Various fixes & improvements

- Make a release issue template (#2666) by @chadwhitacre

## 23.12.0

### Various fixes & improvements

- test(backup): Use --no-prompt for backup tests (#2618) by @azaslavsky

## 23.11.2

- No documented changes.

## 23.11.1

### Various fixes & improvements

- feat: Add sentry-admin.sh tool (#2594) by @azaslavsky
- Patch for dev self-hosted environments (#2592) by @hubertdeng123
- Relicense under FSL-1.0-Apache-2.0 (#2586) by @chadwhitacre
- Bump minimum ram usage (#2585) by @hubertdeng123

## 23.11.0

### Various fixes & improvements

- feat: provide a toggle to enable discord integration (#2548) by @aldy505
- ref: fix a typo (#2556) by @asottile-sentry
- ref: use `git branch --show-current` instead of sed (#2550) by @asottile-sentry
- Remove sessions infra (#2514) by @hubertdeng123
- Upgrade Clickhouse to 21.8 (#2536) by @hubertdeng123
- [Snyk] Security upgrade debian from bullseye-slim to bookworm-20231009-slim (#2511) by @Indigi-managed
- snuba: Remove deprecated CLI arg (#2515) by @lynnagara

## 23.10.1

### Various fixes & improvements

- Revert "feat: upgrade to zookeeper-less kafka (#2445)" (#2500) by @hubertdeng123
- Add fast revert GH workflow (#2499) by @hubertdeng123
- build(deps): bump actions/checkout from 3 to 4 (#2493) by @dependabot
- configure dependabot (#2491) by @mdtro
- deps: bump nginx to 1.25.2 (#2490) by @mdtro
- feat: upgrade to zookeeper-less kafka (#2445) by @joshuarli
- Update outdated install option in README (#2440) by @hubertdeng123

## 23.10.0

### Various fixes & improvements

- Switch geoipupdate image to ghcr.io (#2442) by @hkraal
- Add system.url-prefix to config for visibility (#2426) by @hubertdeng123
- Remove CSPMiddleware since it is enabled by default in the upstream sentry (#2434) by @oioki
- Update nginx.conf (#2455) by @mwarkentin
- Update Redis container image to 6.2.13 (#2432) by @mencarellic

## 23.9.1

### Various fixes & improvements

- fix: e2e test jq bug (#2410) by @azaslavsky
- feat(backup): Support new backup script (#2407) by @azaslavsky
- Decrease frequency of e2e tests (#2383) by @hubertdeng123
- Reduce logs coming from clickhouse (#2382) by @hubertdeng123
- Increase frequency of e2e test runs (#2375) by @hubertdeng123
- Remove nginx content-disposition hack for safari (#2381) by @hubertdeng123
- Attempt to fix integration test flakiness (#2372) by @hubertdeng123
- change health check for kafka service (#2371) by @johnatannvmd
- Add metrics and generic metrics backend (#2355) by @hubertdeng123
- Bump self-hosted e2e action commit sha (#2369) by @hubertdeng123

## 23.8.0

### Various fixes & improvements

- Add issue platform infra (#2309) by @hubertdeng123

## 23.7.2

### Various fixes & improvements

- Ignore fixture-custom-ca-roots service in integration test (#2321) by @hubertdeng123
- Update GeoIpUpdate to v6.0.0 (#2287) by @victorelec14
- Bump healthcheck timeout (#2300) by @hubertdeng123

## 23.7.1

### Various fixes & improvements

- Resolve Safari Content-Disposition header bug (#2297) by @azaslavsky
- feat: vroom cleanup script that respects default retention days (#2211) by @aldy505

## 23.7.0

### Various fixes & improvements

- Remove nc -q option (#2275) by @hubertdeng123
- Move open ai key from env variables (#2274) by @hubertdeng123
- Fix command called in reset script (#2254) by @stayallive
- Remove stale-bot in self-hosted (#2255) by @hubertdeng123
- Update geoipupdate to 5.1.1 (#2236) by @williamdes

## 23.6.2

### Various fixes & improvements

- Update nginx to 1.25.1 (#2235) by @williamdes
- Fix error fingerprinting (#2237) by @chadwhitacre
- A couple unit testing improvements (#2238) by @chadwhitacre
- Fix #1684 (#2234) by @azaslavsky
- Update memcached to 1.6.21 (#2231) by @williamdes
- Update redis to 6.2.12 (#2230) by @williamdes
- ref: Move all consumers to unified consumer CLI (#2224) by @hubertdeng123
- Revert "ref: Move most consumers to unified consumer CLI" (#2223) by @hubertdeng123
- ref: Move most consumers to unified consumer CLI (#2203) by @untitaker
- Release 23.6.1 cleanup (#2209) by @hubertdeng123

## 23.6.1

### Various fixes & improvements

- Fix bump version script (#2207) by @hubertdeng123

## 23.6.0

### Various fixes & improvements

- Remove docker compose v1 (#2187) by @hubertdeng123
- ref(compose): Separate ingest consumers (#2193) by @jan-auer
- feat(profiling): Run profiling on self-hosted (#2154) by @phacops

## 23.5.2

- No documented changes.

## 23.5.1

### Various fixes & improvements

- fix(suggested-fix): key should be 'key', not 'token' (#2146) by @aldy505

## 23.5.0

### Various fixes & improvements

- Add no strict offset reset options to consumers (#2144) by @hubertdeng123
- Add settings for enabling CSP to config file (#2134) by @hubertdeng123
- feat: add suggested fix feature (#2115) by @aldy505
- adding ulimits for zookeeper, kafka, and web (#2123) by @jamincollins
- Uninstall Docker Compose v1 from CI so it's not used for tests (#2114) by @hubertdeng123
- Fixed docker compose issue in backup/restore (#2110) by @montaniasystemab
- Enable upstream keepalive (#2099) by @otbutz
- Bump commit sha for e2e test action (#2104) by @hubertdeng123
- Use docker compose exec to account for differences in container names for Postgres upgrade (#2096) by @hubertdeng123
- Change symbolicator to use CalVer for release (#2091) by @hubertdeng123

## 23.4.0

### Postgres 14 Upgrade

We've now included an upgrade from Postgres 9.6 to 14.5 that will automatically be run via the `./install.sh` script.

By: @hubertdeng123 (#2074)

### Various fixes & improvements

- Remove clean function testing line (#2082) by @hubertdeng123
- Fix command to get docker compose version in problem report template (#2080) by @hubertdeng123
- Tweak permissioning of backup file in backup script to read/write for all users (#2043) by @hubertdeng123
- Remove commit-batch-size parameter (#2058) by @hubertdeng123
- Support external sourcemaps bigger, than 1Mb (#2050) by @le0pard
- Add github setup instructions to config.example.yml (#2051) by @tm1000
- ref(snuba): Use snuba self-hosted settings (#2039) by @enochtangg

## 23.3.1

### Various fixes & improvements

- Bump Kafka version to keep up with SaaS (#2037) by @chadwhitacre
- Add Backup/restore scripts (#2029) by @hubertdeng123
- Add opt in error monitoring to reset and clean scripts (#2021) by @hubertdeng123

## 23.3.0

### Various fixes & improvements

- Remove ZooKeeper snapshot (#2020) by @dereckson
- feat(snuba): Add snuba sessions subscription service (#2006) by @klboke
- Add backup/restore integration tests (#2012) by @hubertdeng123
- ref(snuba): Remove snuba-cleanup, snuba-transactions-cleanup jobs (#2003) by @klboke
- ref(replays): Remove the session-replay-ui flag (#2010) by @ryan953
- Remove broken replay integration test (#2011) by @hubertdeng123
- Bump self-hosted-e2e-tests action commit sha (#2008) by @hubertdeng123
- Revert symbolicator tests (#2004) by @hubertdeng123
- post-process-forwarder: Update CLI command (#1999) by @lynnagara
- feat(replays): add replays to self hosted (#1990) by @JoshFerge
- Remove issue status helper automation (#1989) by @hubertdeng123
- Add proxy buffer size config to fix Bad Gateway (#1984) by @SCjona
- Reference paths relative to project root (#1800) by @spawnia
- Run close stale issues/PRs only on getsentry (#1969) by @aminvakil

## 23.2.0

### Various fixes & improvements

- Run lock issues/PRs only on getsentry (#1966) by @aminvakil
- Updates Redis to 6.2.10 (#1937) by @danielhartnell
- Handle missing example files gracefully (#1950) by @chadwhitacre
- Fix post-release.sh for `git pull` (#1938) by @BYK
- Manually change 23.1.1 to nightly (#1936) by @hubertdeng123

## 23.1.1

### Various fixes & improvements

- ci: Add test for symbolicator pipeline (#1916) by @ethanhs

## 23.1.0

### Various fixes & improvements

- ci: Check health of services after running integration tests and fix snuba-replacer (#1897) by @ethanhs
- Add wal2json debugging (#1906) by @chadwhitacre
- Pick up CI bugfix (#1905) by @chadwhitacre
- ref: Move jq build to error-handling.sh, and use proxy config (#1895) by @ethanhs
- fix(CI): use default curl retry mechanism for wal2json install (#1890) by @volokluev
- ref: Retry wal2json download in installer (#1881) by @ethanhs
- ci: Remove GCB and update Github Action SHA (#1880) by @ethanhs

## 22.12.0

### Various fixes & improvements

- Build each service image individually (#1858) by @ethanhs
- Set higher kafka healthcheck timeout and fix clickhouse timeout (#1855) by @ethanhs
- Add --skip-sse42-requirements to install.sh and enable SKIP_SSE42_REQUIREMENTS override (#1790) by @erinaceous
- Fix commit-log-topic parameter configuration problem (#1817) by @klboke
- Add .idea to .gitignore (#1803) by @spawnia
- Add USE_X_FORWARDED_HOST to example config (#1804) by @crinjes
- (fix): Fix contributor PR e2e tests (#1820) by @hubertdeng123

## 22.11.0

### Various fixes & improvements

- Fix jq usage (#1814) by @ethanhs
- Try adding end to end tests using new action (#1806) by @ethanhs
- Add context line, error msg to envelope (#1784) by @hubertdeng123
- Update to actions/checkoutv3 to address upcoming github deprecations (#1792) by @mattgauntseo-sentry
- ref: upgrade actions/setup-python to avoid set-output deprecation (#1789) by @asottile-sentry
- Enforce error reporting (#1777) by @hubertdeng123
- Upload end of log as breadcrumbs, use exceptions and stacktrace (#1775) by @ethanhs
- Fix sentry release for dogfood instance (#1768) by @hubertdeng123
- Add pre-commit config (#1738) by @ethanhs
- Do not send event on INT signal (#1773) by @hubertdeng123

## 22.10.0

### Various fixes & improvements

- Split post process forwarders (#1759) by @chadwhitacre
- Revert "Enforce error reporting for self-hosted" (#1755) by @hubertdeng123
- Enforce error reporting for self-hosted (#1753) by @hubertdeng123
- ref: Remove unused scripts and code (#1710) by @BYK
- Check to see if docker compose exists, else error out (#1733) by @hubertdeng123
- Fix minimum version requirements for docker and docker compose (#1732) by @hubertdeng123
- Factor out clean and use it in unit-test (#1731) by @chadwhitacre
- Reorganize unit test layout (#1729) by @hubertdeng123
- Request event ID in issue template (#1723) by @ethanhs
- Tag releases with sentry-cli (#1718) by @hubertdeng123
- Send full logs as an attachment to our dogfood instance (#1715) by @hubertdeng123

## 22.9.0

### Various fixes & improvements

- Fix traceback hash for error monitoring (#1700) by @hubertdeng123
- Add section about error monitoring to the README (#1699) by @ethanhs
- Switch from .reporterrors file to flag + envvar (#1697) by @chadwhitacre
- Rename flag to --skip-user-creation (#1696) by @chadwhitacre
- Default to not sending data to Sentry for now (#1695) by @chadwhitacre
- fix(e2e tests): Pull branch that initially triggers gcp build for PRs (#1694) by @hubertdeng123
- fix(e2e tests): Add .reporterrors file for GCP run of e2e tests (#1691) by @hubertdeng123
- Error monitoring of the self-hosted installer (#1679) by @ethanhs
- added docker commands in the description (#1673) by @victorelec14
- Use docker-compose 2.7.0 instead of 2.2.3 in CI (#1591) by @aminvakil

## 22.8.0

- No documented changes.

## 22.7.0

### Various fixes & improvements

- ref: use sort -V to check minimum versions (#1553) by @ethanhs
- Get more data from users in issue templates (#1497) by @aminvakil
- Add ARM support (#1538) by @chadwhitacre
- do not use gosu for snuba-transactions-cleanup and snuba-cleanup (#1564) by @goganchic
- ref: Replace regex with --short flag to get compose version (#1551) by @ethanhs
- Improve installation through proxy (#1543) by @goganchic
- Cleanup .env{,.custom} handling (#1539) by @chadwhitacre
- Bump nginx:1.22.0-alpine (#1506) by @aminvakil
- Run release a new version job only on getsentry (#1529) by @aminvakil

## 22.6.0

### Various fixes & improvements

- fix "services.web.healthcheck.retries must be a number" (#1482) by @yuval1986
- Add volume for nginx cache (#1511) by @glensc
- snuba: New subscriptions infrastructure rollout (#1507) by @lynnagara
- Ease modification of base image (#1479) by @spawnia

## 22.5.0

### Various fixes & improvements

- ref: reset user to root for installation (#1469) by @asottile-sentry
- Document From email display name (#1446) by @chadwhitacre
- Bring in CLA Lite (#1439) by @chadwhitacre
- fix: replace git.io links with redirect targets (#1430) by @asottile-sentry

## 22.4.0

### Various fixes & improvements

- Use better API key when available (#1408) by @chadwhitacre
- Use a custom action (#1407) by @chadwhitacre
- Add some debug logging (#1340) by @chadwhitacre
- meta(gha): Deploy workflow enforce-license-compliance.yml (#1388) by @chadwhitacre
- Turn off containers under old name as well (#1384) by @chadwhitacre

## 22.3.0

### Various fixes & improvements

- Run CI every night (#1334) by @aminvakil
- Docker-Compose: Avoid setting hostname to '' (#1365) by @glensc
- meta(gha): Deploy workflow enforce-license-compliance.yml (#1375) by @chadwhitacre
- ci: Change stale GitHub workflow to run once a day (#1371) by @kamilogorek
- ci: Temporary fix for interactive prompt on createuser (#1370) by @BYK
- meta(gha): Deploy workflow enforce-license-compliance.yml (#1347) by @chadwhitacre
- Add SaaS nudge to README (#1327) by @chadwhitacre

## 22.2.0

### Various fixes & improvements

- fix: unbound variable _group in reset/dc-detect-version script (#1283) (#1284) by @lovetodream
- Remove routing helper (#1323) by @chadwhitacre
- Bump nginx:1.21.6-alpine (#1319) by @aminvakil
- Add a cloudbuild.yaml for GCB (#1315) by @chadwhitacre
- Update set-up-and-migrate-database.sh (#1308) by @drmrbrewer
- Pull relay explicitly to avoid garbage in creds (#1301) by @chadwhitacre
- Improve logging of docker versions and relay creds (#1298) by @chadwhitacre
- Remove file again (#1299) by @chadwhitacre
- Clean up relay credentials generation (#1289) by @chadwhitacre
- Add CI compose version 1.29.2 / 2.0.1 / 2.2.3 (#1290) by @chadwhitacre
- Revert "Add CI compose version 1.29.2 / 2.0.1 / 2.2.3 (#1251)" (#1272) by @chadwhitacre
- Add CI compose version 1.29.2 / 2.0.1 / 2.2.3 (#1251) by @aminvakil

## 22.1.0

### Various fixes & improvements

- Make healthcheck variables configurable in .env (#1248) by @aminvakil
- Take some actions to avoid unhealthy containers (#1241) by @chadwhitacre
- Install: setup umask (#1222) by @glensc
- Deprecated /docker-entrypoint.sh call (#1218) by @marcinroman
- Bump nginx:1.21.5-alpine (#1230) by @aminvakil
- Fix reset.sh docker-compose call (#1215) by @aminvakil
- Set worker_processes to auto (#1207) by @aminvakil

## 21.12.0

### Support Docker Compose v2 (ongoing)

Self-hosted Sentry mostly works with Docker Compose v2 (in addition to v1 >= 1.28.0). There is [one more bug](https://github.com/getsentry/self-hosted/issues/1133) we are trying to squash.

By: @chadwhitacre (#1179)

### Prevent Component Drift

When a user runs the `install.sh` script, they get the latest version of the Sentry, Snuba, Relay and Symbolicator projects. However there is no guarantee they have pulled the latest `self-hosted` version first, and running an old one may cause problems. To mitigate this, we now perform a check during installation that the user is on the latest commit if they are on the `master` branch. You can disable this check with `--skip-commit-check`.

By: @chadwhitacre (#1191), @aminvakil (#1186)

### React to log4shell

Self-hosted Sentry is [not vulnerable](https://github.com/getsentry/self-hosted/issues/1196) to the [log4shell](https://log4shell.com/) vulnerability.

By: @chadwhitacre (#1203)

### Forum → Issues

In the interest of reducing sources of truth, providing better support, and restarting the fire of the self-hosted Sentry community, we [deprecated the Discourse forum in favor of GitHub Issues](https://github.com/getsentry/self-hosted/issues/1151).

By: @chadwhitacre (#1167, #1160, #1159)

### Rename onpremise to self-hosted (ongoing)

In the beginning we used the term "on-premise" and over time we introduced the term "self-hosted." In an effort to regain some consistency for both branding and developer mental overhead purposes, we are standardizing on the term "self-hosted." This release includes a fair portion of the work towards this across multiple repos, hopefully a future release will include the remainder. Some orphaned containers / volumes / networks are [expected](https://github.com/getsentry/self-hosted/pull/1169&#35;discussion_r756401917). You may clean them up with `docker-compose down --remove-orphans`.

By: @chadwhitacre (#1169)

### Add support for custom DotEnv file

There are several ways to [configure self-hosted Sentry](https://develop.sentry.dev/self-hosted/&#35;configuration) and one of them is the `.env` file. In this release we add support for a `.env.custom` file that is git-ignored to make it easier for you to override keys configured this way with custom values. Thanks to @Sebi94nbg for the contribution!

By: @Sebi94nbg (#1113)

### Various fixes & improvements

- Revert "Rename onpremise to self-hosted" (5495fe2e) by @chadwhitacre
- Rename onpremise to self-hosted (9ad05d87) by @chadwhitacre

## 21.11.0

### Various fixes & improvements

- Fix #1079 - bug in reset.sh (#1134) by @chadwhitacre
- ci: Enable parallel tests again, increase timeouts (#1125) by @BYK
- fix: Hide compose errors during version check (#1124) by @BYK
- build: Omit nightly bump commit from changelog (#1120) by @BYK
- build: Set master version to nightly (d3e77857)

## 21.10.0

### Support for Docker Compose v2 (ongoing)

You asked for it and you did it! Sentry self-hosted now can work with Docker Compose v2 thanks to our community's contributions.

PRs: #1116

### Various fixes & improvements

- docs: simplify Linux `sudo` instructions in README (#1096)
- build: Set master version to nightly (58874cf9)

## 21.9.0

- fix(healthcheck): Increase retries to 5 (#1072)
- fix(requirements): Make compose version check bw-compatible (#1068)
- ci: Test with the required minimum docker-compose (#1066)
  Run tests using docker-compose `1.28.0` instead of latest
- fix(clickhouse): Use correct HTTP port for healthcheck (#1069)
  Fixes the regular `Unexpected packet` errors in Clickhouse

## 21.8.0

- feat: Support custom CA roots ([#27062](https://github.com/getsentry/sentry/pull/27062)), see the [docs](https://develop.sentry.dev/self-hosted/custom-ca-roots/) for more details.
- fix: Fix `curl` image to version 7.77.0
- upgrade: docker-compose version to 1.29.2
- feat: Leverage health checks for depends_on

## 21.7.0

- No documented changes.

## 21.6.3

- No documented changes.

## 21.6.2

- BREAKING CHANGE: The frontend bundle will be loaded asynchronously (via [#25744](https://github.com/getsentry/sentry/pull/25744)). This is a breaking change that can affect custom plugins that access certain globals in the django template. Please see https://forum.sentry.io/t/breaking-frontend-changes-for-custom-plugins/14184 for more information.

## 21.6.1

- No documented changes.

## 21.6.0

- feat: Add healthchecks for redis, memcached and postgres (#975)
