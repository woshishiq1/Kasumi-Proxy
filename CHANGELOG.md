## v0.4.10 — 2026-11-09

### Core updates

- xray-core: `v26.10.31` → `v26.11.9`

## v0.4.9 — 2026-11-02

### Core updates

- xray-core: `v26.3.27` → `v26.10.31`
- sing-box: `v1.14.3` → `v1.14.4`

### Changes

- [`ec37307`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ec37307) fix(backend): tear down a data path whose core died
- [`5a53c45`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5a53c45) fix(frontend): wrap setting row control under title when it does not fit
- [`e256b8a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e256b8a) docs(desktop): distinguish pkexec and sudo authorization
- [`1acf7f2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1acf7f2) fix(desktop): discover installed capped helpers for AppImage
- [`8409992`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8409992) fix(core): reject service-only loopback observation targets
- [`54f6bdf`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/54f6bdf) fix(core): omit inert provider burst ping labels with a warning
- [`f7c2580`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f7c2580) fix(core): reject non-canonical hyphen regexes and mixed service loopback candidates
- [`1d2ada0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1d2ada0) fix(core): enforce Go-compatible regex AST grammar and permit loopback balancer members
- [`a4cfcac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a4cfcac) feat(core): support leastLoad balancer strategy costs
- [`9fb666e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9fb666e) fix(core): strip burstObservatory connectivity diagnostic with warning
- [`c943f3c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c943f3c) fix(core): drop a stateless balancer fallback that Xray cannot start
- [`ecedb5a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ecedb5a) fix(core): accept provider routing rules without a type
- [`ddf3488`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ddf3488) fix(core): reject provider proxySettings without a tag
- [`d735ddb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d735ddb) fix(core): treat a null or empty dialerProxy as no hop
- [`3100314`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3100314) fix(core): reject string balancer strategies and doubled dialer hops
- [`ffa7734`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ffa7734) docs: match provider import stages to the sanitizer
- [`3413dac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3413dac) test(core): observe routing records in the provider recursion check
- [`62ac7c9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/62ac7c9) fix(core): classify every Xray rule condition and reject nested chain aliases
- [`b1a8ac7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b1a8ac7) docs: document provider Xray exit fragment linker architecture
- [`a0cad1e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a0cad1e) test(core): add unit and real-Xray tests for provider fragments
- [`670c45f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/670c45f) feat(subs): report omitted provider settings and incompatible config errors
- [`e008137`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e008137) feat(core): link provider Xray profiles as exit fragments without recursion
- [`b27b13e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b27b13e) fix(ci): stage geodata in release workflow before core-compat check
- [`4e14641`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4e14641) fix(core): account for every built case in the core-validation gate
- [`8acb2a7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8acb2a7) fix(core): generate configs accepted by Xray 26.10 and sing-box 1.14
- [`0e694ba`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0e694ba) fix(desktop): fail setup on bypass failure and clean legacy route state
- [`98053b0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/98053b0) feat(desktop): report Windows tun byte counters from GetIfEntry2
- [`344984e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/344984e) fix(desktop): strip UTF-8 BOM from powershell and preserve on-link defaults
- [`39f7370`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/39f7370) fix(desktop): skip routes with unreadable interface metrics and bind uplink by index
- [`c49539b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c49539b) fix(desktop): select default route via GetIpForwardTable2
- [`74226f7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/74226f7) fix(desktop): drop stale route-parser test and use then_some
- [`2cb922e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2cb922e) fix(desktop): take the Windows uplink from one route lookup
- [`5e51cbd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5e51cbd) fix(desktop): emit UTF-8 from the powershell helper
- [`4b55708`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4b55708) fix(desktop): read the Windows uplink adapter alias natively
- [`a592454`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a592454) fix(jobs): preserve failure reason when probe temporary log is blank
- [`86885f6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/86885f6) fix(core): place the proxy-select alias rule ahead of user rules
- [`f425a7b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f425a7b) fix(jobs): probe a custom profile through its default path
- [`e4f8545`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e4f8545) fix(core): hand the proxy tag to the profile's default target
- [`9f74419`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9f74419) fix(core): drop the balancer fallbackTag xray cannot resolve
- [`4bdac91`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4bdac91) feat(core): resolve a custom profile's default traffic target
- [`f33c508`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f33c508) fix(singbox): keep loopback relays reachable under auto_detect_interface
- [`b20861b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b20861b) fix(jobs): own a test's log slot from start to finish
- [`a7c8d54`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a7c8d54) fix(jobs): keep the reason a test never started
- [`0f38e7d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0f38e7d) fix(jobs): run probe cores without the user's routing rules
- [`d2a9829`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d2a9829) fix(android): bound rule-deletion loop in apply_listener_return
- [`4ebdf19`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4ebdf19) fix(android): route tun kernel-listener replies back to the tun
- [`a64ecec`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a64ecec) fix(settings): stack sing-box fragment method setting row to avoid control overflow (#402)
- [`0892158`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0892158) feat(domain): unify subscription filter regex, url security and block templates in backend (#401)
- [`991357d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/991357d) fix(desktop): keep custom-protocol out of default features for CI and dev
- [`8613002`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8613002) fix(desktop): enable custom-protocol feature for embedded frontend assets
- [`d8933c5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d8933c5) feat(domain): unify asset validation, routing rule parsing and core preset policy in backend (#399)
- [`e14d241`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e14d241) feat(routes): implement backend route packaging, sharing and package import (#398)
- [`1783b09`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1783b09) feat(editor): implement backend profile validation and protocol switching (#397)
- [`2427c5f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2427c5f) feat(lifecycle): implement unified startup readiness check and remove frontend logic leak (#396)
- [`de886cf`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/de886cf) fix(lifecycle): address review findings for asset presence, negative selectors, and exact matching
- [`9db4333`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9db4333) fix(frontend): include process, package and source IP in rule summary
- [`b7e7824`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b7e7824) fix(lifecycle): block startup and require geo assets when used in config
- [`fb7ee33`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fb7ee33) fix(copr): instantiate concrete version into spec during make srpm
- [`deb9dc6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/deb9dc6) fix(copr): avoid macro recursion when parsing spec without explicit version
- [`9a9eb86`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9a9eb86) fix(copr): address review findings for spec arch, capabilities, and makefile
- [`e0ec8d1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e0ec8d1) feat(singbox): support dynamic ECH via query_server_name
- [`38b1767`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/38b1767) fix(frontend): preserve locate target through filter updates before scrolling
- [`7e74199`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7e74199) fix(frontend): ensure locate scroll executes and centers smoothly
- [`e4cd98f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e4cd98f) feat(frontend): navigate and scroll to active profile from overview
- [`6ee1e86`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6ee1e86) fix(core): match static-host names case-insensitively in sing-box DNS
- [`e197777`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e197777) fix(core): bootstrap sing-box DNS servers through static hosts
- [`4bea104`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4bea104) docs: say a Linux desktop identifies as Incy desktop too
- [`21e1feb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/21e1feb) feat(backend): take both desktop HWIDs from happ-sub's rules
- [`8ecdfaa`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8ecdfaa) feat(core): describe a desktop raw and let happ-sub format it per client
- [`5e080e3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5e080e3) fix(backend): tune test core configs for the platform
- [`054f126`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/054f126) fix(log): write each record on one line
- [`0755112`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0755112) fix(desktop): refuse to start a bridged core that could not be marked
- [`87995df`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/87995df) feat(core): send Happ desktop's full locale on Linux
- [`892a72d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/892a72d) fix(desktop): keep a Linux bridged data path across an uplink change
- [`e1eb8e5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e1eb8e5) feat(core): mark the outbounds a bind would bind
- [`dc87108`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/dc87108) docs: say a Linux desktop identifies as Happ desktop
- [`dcf22a5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/dcf22a5) feat(desktop): describe a Linux machine as Happ desktop does
- [`e43f53d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e43f53d) feat(backend): send the machine id as Happ desktop does on Linux
- [`ef5dbfd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ef5dbfd) feat(core): send Happ desktop's request from a Linux desktop
- [`137fbd9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/137fbd9) fix(desktop): describe the real device in subscription requests
- [`b81796b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b81796b) fix(desktop): open links and watch for resume through the helper too
- [`01a49ac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/01a49ac) test(desktop): check that RemotePlatform answers uplink changes as DesktopPlatform
- [`7609598`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7609598) fix(desktop): ask the local platform whether an uplink change restarts
- [`006cdb3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/006cdb3) fix(backend): decide on an uplink change under the lifecycle lock
- [`ddff548`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ddff548) fix(desktop): rebuild only a bridged data path when the uplink changes
- [`4c5c634`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4c5c634) fix(frontend): let a running core be stopped or restarted while connecting
- [`2208e33`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2208e33) fix(backend): keep the status when a refresh re-creates the running profile
- [`785c761`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/785c761) fix(daemon): answer a request it cannot read
- [`c093d6a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c093d6a) fix(desktop): gate unused log imports on target os
- [`4995c30`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4995c30) fix(backend): scope kasumi_log import to Windows job submodule
- [`ae0dff1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ae0dff1) fix(log): append semantics for child logs, recursive field redaction and safe shell lock
- [`7bd0ce6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7bd0ce6) fix(security): sanitize shell arguments on failure and redact fields in logger
- [`7ec2b41`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7ec2b41) fix(log): address review feedback on rotation, redaction, filters and i18n
- [`05e39b5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/05e39b5) fix(frontend): wait for a command as long as the daemon is alive
- [`d5ab5f4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d5ab5f4) feat(daemon): send a heartbeat on every WebUI connection
- [`aa2905d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/aa2905d) fix(backend): end every fetch within one budget
- [`a52af5a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a52af5a) feat(frontend): record what the socket drops, now that it can drop
- [`2cc08c4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2cc08c4) docs(log): say where the records come from, and correct what the UI is pushed
- [`2db8b38`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2db8b38) feat(backend): trim logs on a timer and cut them on record boundaries
- [`79f0ce6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/79f0ce6) feat(daemon): record what the Android data path did, and what it could not run
- [`6ffd494`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6ffd494) feat(backend): tell "no file" apart from "cannot read it"
- [`dafc74a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/dafc74a) feat(backend): keep the geo conversion and the core spawn from failing quietly
- [`8f2934f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8f2934f) feat(backend): say what the data path is doing, and why it stopped
- [`9a197ac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9a197ac) test(backend): decide the log fallback off the shared buffer
- [`21492f8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/21492f8) fix(module): keep the sourced logger visible to shellcheck
- [`ed2cb4c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ed2cb4c) docs(log): describe the UI's own records
- [`0ad371b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0ad371b) feat(frontend): record what the UI swallows
- [`ed92ff0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ed92ff0) feat(backend): show the in-memory tail when the app log has nothing
- [`b2ff459`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b2ff459) test(log): keep ad-hoc printing out of the tree
- [`80dfcaf`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/80dfcaf) feat(module): let the module's own scripts record what they did
- [`46db930`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/46db930) feat(frontend): offer the app log level next to the core one
- [`bdba046`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bdba046) feat(state): let the user pick the verbosity of the app's own log
- [`4390899`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4390899) feat(log): default our own areas to debug, dependencies to info
- [`5343a44`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5343a44) feat(log): let a noisy dependency be pinned below the level filter
- [`e83b72a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e83b72a) fix(sub): keep the subscription link out of the fetch failure log
- [`ff78b83`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ff78b83) feat(log): redact URLs that appear inside error chains
- [`4aae95c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4aae95c) feat(log): one record format for every Kasumi process
- [`ca604ee`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ca604ee) fix(frontend): let a closing socket settle only what it owns
- [`0b951e9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0b951e9) fix(backend): keep the geo flag when stopping the core fails
- [`cfeac21`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cfeac21) fix(backend): write geo data and decide the pending restart under one lock
- [`0424a49`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0424a49) fix(frontend): stop warning that geo updates restart the connection
- [`6dc3a73`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6dc3a73) fix(backend): mark the restart pending after a manual geo download too
- [`3d5776c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3d5776c) fix(frontend): tell the user new geo data waits for a restart
- [`c8ff4f6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c8ff4f6) fix(backend): mark the restart pending when geo data changes
- [`c26f02c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c26f02c) fix(frontend): drop a pending reconnect once nobody listens
- [`58526dd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/58526dd) fix(frontend): keep reconnecting the daemon socket until it answers
- [`db38e74`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/db38e74) fix(android): drop socket marks from Xray configs
- [`b20ead4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b20ead4) fix(android): respawn a dead uplink monitor no faster than the poll
- [`0724bf9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0724bf9) fix(android): poll instead of respawning an ip without monitor support
- [`f6eb628`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f6eb628) fix(android): drop the shell-era RFC1918 rules from the external tun path
- [`a006ecc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a006ecc) fix(android): follow Android's default network and drop the mark rule
- [`0238534`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0238534) fix(android): keep the data path running across an uplink switch
- [`681781f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/681781f) test(core): check generated Xray rules for a condition in the core sweep
- [`3630154`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3630154) fix(core): leave out a rule whose domains and IPs all parse to nothing
- [`09e7a44`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/09e7a44) fix(frontend): ask for a condition before saving a routing rule
- [`64909ef`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/64909ef) fix(core): leave out Xray rules with no condition
- [`b8ce38a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b8ce38a) fix(frontend): drop the unverified note from Incy's identity
- [`d13412b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d13412b) fix(deps): bump happ-sub to a99ec83 for Incy's HWID prefix
- [`8ad9928`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8ad9928) docs: mention fetching subscriptions as Incy
- [`9f67b33`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9f67b33) feat(frontend): choose Happ or Incy per subscription
- [`d075f41`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d075f41) feat(core): fetch a subscription as Incy
- [`c7820f6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c7820f6) build(deps): bump happ-sub to acd9aef
- [`9e53846`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9e53846) build(deps): bump happ-sub to c08b41b
- [`da24259`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/da24259) docs: list incy://crypt1 among the imported links
- [`c423bd4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c423bd4) feat(frontend): name an Incy subscription after its provider
- [`77b5fee`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/77b5fee) feat(core): import Incy's incy://crypt1 subscription links
- [`bc34506`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bc34506) build(deps): bump happ-sub to 7672c07 for incy://crypt1
- [`b83ebc9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b83ebc9) feat(frontend): warn when a rule's target loses settings on sing-box
- [`0b7be16`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0b7be16) feat(core): list the xray-only settings sing-box would drop from a profile
- [`2e41dc3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2e41dc3) fix(frontend): show long hosts in full on a narrow outbound field
- [`2d03757`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2d03757) fix(frontend): let a long app bar title wrap before it is cut
- [`0a565ff`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0a565ff) fix(frontend): mark chain hops that clash on core as unavailable
- [`89126b7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/89126b7) feat(frontend): warn on rules whose target the active core can't build
- [`4941f96`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4941f96) feat(core): report why a core can't build a rule's target profile
- [`72b2bb7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/72b2bb7) fix(android): let the phone's IPv6 replies reach tethered clients
- [`f2711af`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f2711af) fix(core): refuse custom Xray configs that skip the certificate check
- [`b1da215`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b1da215) fix(desktop): drop the old engine marker at boot
- [`582a957`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/582a957) fix(desktop): stop the tun helper gracefully
- [`cef618e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cef618e) fix(desktop): sweep sing-box's IPv6 auto_route rules after an unclean exit
- [`bec6204`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bec6204) fix(android): stop tun helpers gracefully and sweep their orphaned rules
- [`d9cb44b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d9cb44b) feat(backend): find the sing-box tun rules a killed helper leaves behind
- [`06e3d1d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/06e3d1d) fix(backend): report the ports the running data path listens on
- [`ef820de`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ef820de) feat(core): record the ports a data path listens on
- [`e4e87c3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e4e87c3) fix(android): route the app filter the plan was resolved with
- [`d813816`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d813816) fix(core): ask for a restart when the routing in front of a helper changes
- [`f96d946`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f96d946) fix(android): watch the force-proxy tun's helper too
- [`59cf2a7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/59cf2a7) test(desktop): start and the watchdog expect the same helper
- [`e30004c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e30004c) feat(desktop): send the data-path plan to the privileged helper
- [`ad531f8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ad531f8) test(android): start and the watchdog expect the same helpers
- [`e6c0b99`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e6c0b99) test(backend): the platform starts from the baseline's plan
- [`b614160`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b614160) test(core): plan, config and state agree for every combination
- [`20ad9dc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/20ad9dc) feat(core): add the data-path plan
- [`839a39e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/839a39e) feat(core): record the helpers a data path runs
- [`10a3e40`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/10a3e40) fix(android): bridge the force-proxy tun into the force inbound's port
- [`993624b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/993624b) fix(android): bring up the sing-box sidecar for an xray core
- [`6cc9fae`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6cc9fae) feat(core): export the defaults a new subscription starts with
- [`f5f03c9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f5f03c9) feat(frontend): open the profile editor on a link pasted in the Add sheet
- [`e5e3b87`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e5e3b87) fix(frontend): carry the Add sheet's options into the subscription editor
- [`9ab1db0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9ab1db0) fix(frontend): let a sheet dismissed while sliding in finish closing
- [`bec5f0c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bec5f0c) fix(frontend): open the subscription editor with the URL typed in the Add sheet
- [`d201570`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d201570) fix(core): don't offer a routing profile that carries no rules
- [`7a7c45f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7a7c45f) fix(android): refuse tethered clients' IPv6 DNS to the phone
- [`396d93f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/396d93f) fix(android): pin tethered traffic ahead of the BPF offload programs
- [`a25bdae`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a25bdae) test(desktop): drive the helper pipe loop from two GUIs
- [`790aaa6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/790aaa6) fix(desktop): serve only the Windows session that started the service
- [`c848c1a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c848c1a) feat(desktop): add the session rule for the helper service
- [`ec77c84`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ec77c84) feat(frontend): name rule and route targets apart, and flag deleted ones
- [`32e0c5f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/32e0c5f) feat(frontend): pick a profile from a searchable full-height sheet
- [`28b2bf4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/28b2bf4) feat(frontend): name profiles apart where they are referenced
- [`63f0a12`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/63f0a12) fix(backend): sweep retained test logs when profiles are dropped and on start
- [`d5f719f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d5f719f) fix(daemon): make the status CLI report the running daemon's state
- [`5cd572b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5cd572b) fix(backend): answer a Status request with the probe-refined state
- [`a22d73f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a22d73f) fix(frontend): lay out subscription cards the same way at any width
- [`f390414`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f390414) fix(frontend): show subscription traffic in the UI font and locale
- [`74dc480`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/74dc480) fix(frontend): give app bar subtitles their own full-width row
- [`97431f9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/97431f9) fix(scripts): resolve the release zip path before entering module/
- [`93af940`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/93af940) test(desktop): cover the Windows DNS guard and its lack of persistent state
- [`b6ab865`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b6ab865) fix(desktop): block DNS outside the Windows tun while the helper lives
- [`9193c85`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9193c85) fix(desktop): give the Windows tun its own resolver with an xray core
- [`e2163fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e2163fe) feat(core): add the resolver address a Windows tun advertises
- [`89c5d64`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/89c5d64) fix(desktop): link the app manifest into Windows test binaries
- [`f63098d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f63098d) feat(frontend): explain a core forced or blocked by a chain hop
- [`75135e3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/75135e3) feat(backend): report the hop that pins a profile's core
- [`f790c2f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f790c2f) fix(core): run a proxy chain on the core its hops need
- [`513798f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/513798f) test(desktop): refuse a pre-handshake helper over a real socket
- [`d237fe9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d237fe9) feat(frontend): explain an outdated helper on startup
- [`6c5daf8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6c5daf8) feat(desktop): report an outdated helper to the UI
- [`14b7524`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/14b7524) feat(desktop): version the privileged helper handshake
- [`8664982`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8664982) fix(frontend): mark catch-all rules from the backend's answer
- [`d6b8399`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d6b8399) feat(backend): answer which routing rules catch everything
- [`f7deb46`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f7deb46) feat(core): tell whether a built rule matches every connection
- [`5feb05a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5feb05a) feat(desktop): pin the IPv6 uplink source for sing-box
- [`9f34f88`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9f34f88) feat(frontend): hide protocols the device can't run in the editor
- [`a234f46`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a234f46) fix(backend): withhold protocols the device can't run
- [`60382a8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/60382a8) test(core): check a share-link corpus against the real cores
- [`a726786`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a726786) feat(frontend): say why an insecure profile can't start
- [`03e64d6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/03e64d6) fix(core): run unpinned insecure TLS on sing-box, refuse it on xray
- [`bbc7afd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bbc7afd) fix(core): leave the removed trojan flow out of xray configs
- [`b136e55`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b136e55) feat(frontend): pin a profile to the default route in the editor
- [`25a42d5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/25a42d5) feat(core): let the default route pin a profile against its group
- [`9f3b13e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9f3b13e) feat(frontend): show a local port clash in Settings
- [`fdd61e5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fdd61e5) fix(backend): refuse a settings write that makes ports collide
- [`b2096a2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b2096a2) fix(core): detect local listeners set to one port
- [`23dccc7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/23dccc7) fix(frontend): say that a backup merge skips what is already here
- [`a5e8cff`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a5e8cff) fix(core): skip backup items already here when merging
- [`3772a41`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3772a41) fix(frontend): say that TCP ping targets a chain's first hop
- [`4577726`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4577726) fix(desktop): tcp-ping over the uplink while a tun is up
- [`4607b72`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4607b72) fix(backend): tcp-ping the chain hop the device dials
- [`1649ce5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1649ce5) fix(backend): start the tun engine with the baseline's tuning
- [`764bbfd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/764bbfd) fix(core): count external tun tuning as a core config change
- [`77904dd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/77904dd) test(android): cover the xtables.lock detection and retry decision
- [`cb3f699`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cb3f699) test(backend): cover job-object reaping on Windows
- [`fe39d53`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fe39d53) fix(android): retry a sing-box start that lost the xtables.lock race
- [`67dac2a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/67dac2a) fix(backend): reap Windows children with a kill-on-close job object
- [`a320ee6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a320ee6) fix(backend): bound the in-memory subscription cookie jar
- [`089e5e9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/089e5e9) style(desktop): collapse the nested if in the service uninstall
- [`732ccd8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/732ccd8) feat(frontend): say what a routing link imported as a route does
- [`780a6cd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/780a6cd) fix(frontend): count only real share links in the mock bridge
- [`a62643e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a62643e) fix(frontend): name a typed happ:// subscription after what it resolves to
- [`f582966`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f582966) fix(frontend): tell links from broken JSON in the backup and rule imports
- [`d5ddf6b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d5ddf6b) fix(backend): write subscription request headers in title case
- [`5d4e072`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5d4e072) fix(frontend): send subscription edits with the copy they started from
- [`a5bfd08`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a5bfd08) fix(core): apply only the settings a subscription edit changed
- [`bfb2d48`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bfb2d48) fix(core): keep fetch results when a subscription is saved
- [`bed47bd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bed47bd) feat(core): add a SetSubError intent for failures the UI detects
- [`55f5940`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/55f5940) feat(frontend): take happ://routing links in the route import sheet
- [`5093dcb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5093dcb) feat(core): import a Happ routing profile as a route of its own
- [`6e59a60`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6e59a60) fix(core): let every Shadowsocks cipher run on Xray on plain TCP
- [`b3d1b93`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b3d1b93) test(core): validate Xray cipher spellings on both pinned cores
- [`5818860`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5818860) fix(core): let Xray-spelled Shadowsocks ciphers run on sing-box
- [`a8de778`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a8de778) test(backend): make the port-lease test independent of other processes
- [`fb13b80`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fb13b80) fix(frontend): say how many backup profiles were left out
- [`00276b2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/00276b2) feat(backend): count skipped profiles when restoring a backup
- [`2003c3d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2003c3d) fix(backend): read app-state.json through the migrations everywhere
- [`33e42b5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/33e42b5) fix(desktop): generate enum-keyed maps as partial Zod records
- [`e85f6e0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e85f6e0) fix(frontend): keep the mock bridge from restoring unmigrated profiles
- [`72d3e62`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/72d3e62) fix(frontend): let a backup's older profiles reach the migrations
- [`381ea93`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/381ea93) test(core): restore a backup that still has flat v0 profiles
- [`f7b8173`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f7b8173) fix(backend): stamp the current schema version on every state write
- [`815cc89`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/815cc89) test(core): pin a sing-box tailscale endpoint as a skipped server
- [`3a9b2a9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3a9b2a9) fix(frontend): say which sing-box outbounds the warning counts
- [`991ed48`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/991ed48) fix(core): warn only about sing-box servers that can't be imported
- [`c070516`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c070516) feat(backend): offer HTTP/2 to subscription servers over ALPN
- [`84f5d17`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/84f5d17) fix(core): keep the REALITY pick of an active provider config
- [`c0511c8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c0511c8) fix(core): bind xray dns outbounds to the uplink in bridged mode
- [`a7d89ee`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a7d89ee) test(core): validate bridged uplink binds against the real cores
- [`46b68b3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/46b68b3) fix(core): bind every server outbound to the uplink in bridged mode
- [`b573365`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b573365) fix(frontend): confirm withdrawing provider configs and remove them
- [`a3a1222`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a3a1222) fix(core): drop provider configs when their permission is withdrawn
- [`6d3f6fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6d3f6fe) fix(backend): name the profile an on-demand probe measured
- [`ad75b5a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ad75b5a) fix(backend): report a ping only for the profile it measured
- [`3208db3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3208db3) test(backend): make the failed tcp_ping probe network-independent
- [`eddf3bb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/eddf3bb) fix(frontend): start new VLESS, VMess and HTTP profiles without TLS
- [`790837e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/790837e) fix(core): run Shadowsocks over QUIC only on a core that supports it
- [`4bef647`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4bef647) fix(frontend): refuse a newer-schema backup before stopping the service
- [`b9857dc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b9857dc) feat(frontend): stamp the schema version on exported backups
- [`5442208`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5442208) fix(core): migrate imported backups like stored state
- [`30b0cea`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/30b0cea) fix(frontend): read happ:// links in the subscription URL field
- [`a673611`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a673611) fix(core): switch off TLS on stored plain Shadowsocks profiles
- [`cac8269`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cac8269) fix(frontend): keep TLS off when the editor switches to Shadowsocks
- [`e433c74`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e433c74) fix(core): keep plain Shadowsocks links without TLS
- [`835208d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/835208d) docs: describe the Happ support in one place
- [`1dc5204`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1dc5204) feat(frontend): show encrypted subscription links with a Reveal action
- [`b243f70`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b243f70) feat(frontend): read happ:// links in the add sheet
- [`0d16f3f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0d16f3f) feat(frontend): add resolveImportInput and revealSubscriptionUrl
- [`1378abc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1378abc) feat(backend): add ResolveImportInput and RevealSubscriptionUrl
- [`c916853`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c916853) feat(backend): decrypt encrypted subscription links at fetch time
- [`918c41a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/918c41a) feat(frontend): explain an encrypted link that does not decrypt
- [`72cf9a6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/72cf9a6) feat(core): resolve happ:// links and encrypted subscription URLs
- [`561972a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/561972a) build(deps): enable happ-sub URL decryption with the built-in keys
- [`2913599`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2913599) docs: mention JSON subscription bodies
- [`26410a4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/26410a4) feat(frontend): review provider JSON configs and mark them in the list
- [`7a7b89d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7a7b89d) feat(backend): ask before importing a provider's Xray configs
- [`c1aed0f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c1aed0f) feat(core): decompose sing-box subscription bodies into typed profiles
- [`5ebf94b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5ebf94b) feat(core): import Xray JSON subscription bodies after consent
- [`b8121de`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b8121de) feat(core): keep provider Custom profiles across refreshes
- [`db96084`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/db96084) feat(frontend): show the tethering offload warning under its switch
- [`a328257`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a328257) feat(android): warn while tethering offload still bypasses the proxy
- [`ab6ddad`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ab6ddad) fix(android): reinstall tether routes after the downstream is recreated
- [`df51e2a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/df51e2a) fix(android): hold off tethering offload while tethered traffic is proxied
- [`bad08bb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bad08bb) fix(android): detect tethering downstreams from Android's own rules
- [`48e875d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/48e875d) feat(android): proxy hotspot and tethering clients
- [`593ca0a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/593ca0a) docs: mention the review of provider-proposed changes
- [`c97a817`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c97a817) feat(frontend): review provider-proposed changes per subscription
- [`b48860b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b48860b) feat(backend): offer provider changes on fetch, use accepted fallback
- [`f9391e4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f9391e4) feat(backend): honour accepted provider User-Agent keys
- [`b4343f1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b4343f1) feat(core): propose provider changes and apply them only on consent
- [`5428871`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5428871) docs: mention the Happ-style request identity
- [`0fa7c2c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0fa7c2c) feat(frontend): edit the request identity per subscription and in Settings
- [`3aa1415`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3aa1415) feat(frontend): add resolveRequestIdentity to the bridge
- [`3f70245`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3f70245) feat(desktop): report device facts and the machine id
- [`c3c9077`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c3c9077) feat(daemon): read the Android SSAID key and device facts
- [`98bf9d1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/98bf9d1) feat(backend): send Happ's request identity on subscription fetches
- [`cbb5e32`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cbb5e32) feat(core): resolve the subscription request identity via happ-sub
- [`2bdbad1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2bdbad1) docs: mention Happ-compatible subscriptions
- [`e8ad245`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e8ad245) feat(frontend): show provider info on subscription cards
- [`0948c75`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0948c75) fix(core): keep REALITY sni/sid of the active profile across refreshes
- [`39264bc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/39264bc) feat(backend): open provider links
- [`ba575d5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ba575d5) feat(backend): apply provider meta on subscription updates
- [`c42f7cb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c42f7cb) feat(core): migrate state to v2
- [`88de447`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/88de447) feat(core): provider info and schedule from subscription meta
- [`489f6ca`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/489f6ca) build(deps): bump happ-sub to 62642b3
- [`15b4988`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/15b4988) feat(frontend): show provider Custom profiles read-only
- [`38d6bf9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/38d6bf9) feat(core): build provider configs into Kasumi's skeleton
- [`4199c5a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4199c5a) feat(core): sanitise provider Xray configs
- [`ec40142`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ec40142) feat(core): mark Custom profiles by origin
- [`4448778`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4448778) feat(backend): route subscriptions through happ-sub
- [`934671c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/934671c) feat(backend): return status and headers from net::fetch
- [`2890dae`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2890dae) feat(core): ingest subscription responses through happ-sub
- [`bdbbbc1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bdbbbc1) fix(core): drop Happ serverDescription from share-link names
- [`afeeb9f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/afeeb9f) fix(core): parse bare IPv6 hosts in share links

## v0.4.8 — 2026-10-12

### Core updates

- sing-box: `v1.14.2` → `v1.14.3`

### Changes

- [`54b7e85`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/54b7e85) feat(frontend): answer routing edits with an explicit restart verdict (#294)
- [`5c2bdc1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5c2bdc1) fix(frontend): mute switched-off blocks in the route graph (#293)
- [`79a632e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/79a632e) fix(frontend): tuck background sheets away while another sheet is on top (#292)
- [`c92a8a7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c92a8a7) fix(frontend): keep semantic colors in text and fill roles (#291)
- [`90aa523`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/90aa523) fix(frontend): tone the restart banner into the warn container palette (#289)
- [`83d5cdf`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/83d5cdf) fix(frontend): give the overview route chip its own line (#288)
- [`2712d51`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2712d51) fix(frontend): resolve the graph proxy outbound to the selected profile node
- [`ccb76ab`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ccb76ab) fix(frontend): show the selected profile on the graph proxy outbound
- [`61d3c9e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/61d3c9e) fix(frontend): list profiles in route pickers the way the Profiles screen does (#287)
- [`a22ac4f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a22ac4f) feat(frontend): routes built from shared rule blocks
- [`b12efcd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b12efcd) feat(core): rule blocks and per-profile routes
- [`f30fc52`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f30fc52) fix(frontend): Back closes the top sheet or dialog
- [`af260b1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/af260b1) fix(frontend): add new routing rules above a rule that catches everything
- [`77902a8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/77902a8) fix(frontend): word speed tests, failed installs and the backup box right
- [`27153db`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/27153db) fix(frontend): validate resource files and keep each one re-downloadable
- [`0286241`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0286241) fix(frontend): say what failed instead of showing a bare error
- [`b20efe0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b20efe0) fix(frontend): keep the Profiles filter, sort and search across tabs
- [`3ebfbae`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3ebfbae) fix(frontend): stop offering settings that do nothing here
- [`893e893`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/893e893) fix(frontend): a real first-run state on Profiles, no empty headings
- [`f924af6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f924af6) fix(frontend): give switches, fields and close buttons accessible names
- [`d899323`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d899323) fix(frontend): turn the Overview dead ends into ways forward
- [`986d4f7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/986d4f7) fix(frontend): show a subscription updating, and run it once
- [`caa864f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/caa864f) feat(frontend): say "restart to apply" in Settings too
- [`dcee0c5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/dcee0c5) fix(backup): back up rules, resource files and hand-made profiles
- [`25760ea`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/25760ea) fix(frontend): save settings fields on blur and never fail a write silently
- [`efa3e88`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/efa3e88) feat(frontend): select all or a whole group in bulk mode
- [`1924723`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1924723) fix(frontend): keep unsaved profile edits and blank profiles out
- [`d271c5e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d271c5e) fix(frontend): ask before actions that can't be undone
- [`e67a75c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e67a75c) fix(frontend): add into the group being looked at
- [`37c538d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/37c538d) feat(frontend): one Add sheet that sorts out what is pasted
- [`e757da4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e757da4) feat(frontend): create a group right where one is picked
- [`4f460a5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4f460a5) fix(core): keep subscriptions and profiles pointing at a live group
- [`7a919b9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7a919b9) feat(desktop): list launcher apps for the app filter
- [`3a4b431`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3a4b431) feat(core): route desktop apps in the app filter by process
- [`5925546`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5925546) fix(android): keep apps outside the proxy off its ports and its tun
- [`89e9615`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/89e9615) fix(desktop): send system DNS through the tun with an xray core
- [`5ec4a7b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5ec4a7b) feat(core): xray config helpers for DNS through a tun
- [`5d143f6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5d143f6) fix(desktop): keep the LAN out of the sing-box tun on Linux
- [`425fd7b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/425fd7b) fix(frontend): word the startup toggles for desktop
- [`e0f2446`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e0f2446) fix(desktop): start with the system through the launcher, in the tray
- [`c8b6176`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c8b6176) feat(frontend): keep the active ping fresh and re-check it on tap
- [`a6a6958`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a6a6958) feat(backend): check connectivity once a minute and report its latency

## v0.4.7 — 2026-09-29

### Changes

- [`26e1b38`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/26e1b38) fix(desktop): ship kasumi-helper as a bundled bin, not a sidecar
- [`790fdd2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/790fdd2) build(desktop): run codegen as an example, not a bin
- [`de7a7e2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/de7a7e2) docs(readme): add screenshots of the desktop and Android UI
- [`9e3ac41`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9e3ac41) fix(frontend): give routing rules their own card
- [`5a3ba16`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5a3ba16) fix(frontend): make routing rules usable on a phone-width screen

## v0.4.6 — 2026-09-29

### Core updates

- sing-box: `v1.14.0` → `v1.14.2`

### Changes

- [`e9d7432`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e9d7432) fix(android): stop strict-route carve-out from blackholing tethered clients
- [`58b6d2b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/58b6d2b) docs(agents): drop the Nix-only workflow and stale references
- [`6dcce29`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6dcce29) docs: trim README, split build and Nix guides out
- [`516c6f9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/516c6f9) fix(frontend): hide the restart cue while a start or stop is running
- [`e9b2fad`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e9b2fad) fix(backend): don't flag a pending restart over a restart in flight
- [`223486a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/223486a) feat(settings): process, app and source-address fields in the rule editor
- [`86a1706`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/86a1706) feat(core): match routing rules by process, Android app and source address
- [`6daba66`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6daba66) feat(core): choose how sing-box fragments the TLS handshake
- [`a90100a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a90100a) feat(editor): pick the profile to connect through
- [`38880df`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/38880df) feat(core): proxy chains through another profile
- [`a6fd50e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a6fd50e) feat(backend): keep a sing-box cache file across core restarts
- [`72bffb0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/72bffb0) feat(core): offer the mixed sing-box tun stack
- [`ca2d368`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ca2d368) fix(core): use every remote DNS server on sing-box, not just the first
- [`e5e6fc8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e5e6fc8) TUN engine settings driven by Rust: each engine shows the fields it reads
- [`ea4ac81`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ea4ac81) frontend: TUN engine matrix and one type scale for rows, hints and labels
- [`f8f824f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f8f824f) frontend: settings as categories, segmented controls, searchable selects
- [`be43bbe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/be43bbe) feat(settings): asset auto-update controls
- [`5a8ee20`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5a8ee20) feat(backend): headless geosite/geoip auto-update
- [`69f6786`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/69f6786) fix(frontend): render newline-joined list settings in a textarea
- [`fc1d743`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fc1d743) fix(core): keep the wireguard address list non-empty
- [`a839c86`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a839c86) feat(frontend): parse list settings one-per-line and add hints
- [`952daac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/952daac) feat(core): parse list fields on newline or comma
- [`744a230`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/744a230) feat(frontend): expose TUN exclude-CIDRs in the TUN engine settings
- [`93a7e32`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/93a7e32) feat(desktop): merge user exclude-CIDRs into the tun bypass
- [`1635327`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1635327) feat(core): add TUN exclude-CIDR setting
- [`903bc66`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/903bc66) feat(core): match DNS responses instead of legacy address filters
- [`4c7e0e4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4c7e0e4) test(core): list every legacy-DNS offender in the config harness
- [`c41caf1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c41caf1) fix(core): keep fake-DNS sing-box configs off response-matched DNS fields
- [`fed29b0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fed29b0) feat(core): generate the routing-mode option list from Rust
- [`d09b349`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d09b349) fix(tray): don't panic when the bundled icon won't decode
- [`5270909`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5270909) fix(tray): surface pending-restart in the tooltip
- [`d1406f2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d1406f2) feat(tray): routing switch, live tooltip/icon, ping in recent list
- [`f658431`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f658431) feat(frontend): call out a catch-all that only repeats the final fallback
- [`28a893f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/28a893f) feat(frontend): warn about catch-all rules in the routing list
- [`b4124ee`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b4124ee) feat(frontend): detect routing rules that match every connection
- [`daf7e70`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/daf7e70) fix(frontend): drop the duplicate restart button from the pending-restart banner

## v0.4.4 — 2026-08-03

### Core updates

- sing-box: `v1.13.14` → `v1.13.15`

### Changes

- [`49dc58f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/49dc58f) fix(desktop): propagate boot_init dir-creation errors
- [`0beef3c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0beef3c) fix(desktop): stop mutating the process-global umask in privhelper serve
- [`8b73874`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8b73874) fix(desktop): let settings stay editable while the proxy is running
- [`4789239`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4789239) feat(core): DataPathState document + read/write helpers
- [`a12e8ea`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a12e8ea) test(desktop): drop env mutation from path-dependent tests
- [`9fdcba8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9fdcba8) feat(frontend): pending-restart banner on the overview
- [`f2b20a0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f2b20a0) feat(backend): flag a running data path stale after settings mutations
- [`37f0aa3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/37f0aa3) feat(core): pendingRestart status flag + mutation-effect decision
- [`a878c4c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a878c4c) feat(desktop): skip the privileged helper in non-tun proxy modes
- [`04643a7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/04643a7) fix(desktop): hand helper-created runtime files to the GUI owner
- [`5617db8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5617db8) feat(desktop): make the PAC port a local-ports setting
- [`2463bb2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2463bb2) feat(desktop): snapshot and restore the OS proxy around system/pac
- [`157ee72`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/157ee72) feat(desktop): serve a PAC in pac mode
- [`af5f1e2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/af5f1e2) feat(desktop): set the OS proxy in system mode
- [`49196c3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/49196c3) feat(desktop): run a proxy-only data path + mode selector
- [`7839739`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7839739) feat(core): add proxyMode setting (tun/proxy-only/system/pac)
- [`64286d3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/64286d3) fix(desktop): tunnel root traffic on Linux; escape the core by fwmark
- [`91ea0b2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/91ea0b2) fix(core): make tun uid-0 exclusion a platform decision, not builder policy
- [`0063db2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0063db2) fix(tun): drive tun2socks through its YAML config

## v0.4.3 — 2026-07-13

### Core updates

- tun2socks: `v2.6.0` → `v2.7.0`

### Changes

- [`a735813`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a735813) Revert "feat(nix): Force use zsh in devshell"
- [`d68ee13`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d68ee13) build(nix): single-source rustfmt's edition from Cargo.toml
- [`cd8824e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cd8824e) build(nix): single-source the Rust toolchain via rust-toolchain.toml
- [`d215fc4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d215fc4) fix(nix): exclude generated bun.nix from treefmt
- [`8d8d3cf`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8d8d3cf) feat(nix): Force use zsh in devshell
- [`4c96f90`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4c96f90) test(core): guard TS<->Rust core-resolution parity with generated fixtures
- [`5e0c423`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5e0c423) fix(profiles): route plain/(x)chacha20-poly1305 shadowsocks to the xray tag
- [`38c4050`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/38c4050) feat(tun): sing-box as an external TUN engine for xray (sidecar bridge)
- [`11767e3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/11767e3) feat(settings): hev TUN engine option + tuning controls
- [`45dd592`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/45dd592) build(binaries): fetch hev-socks5-tunnel for desktop and android
- [`b988269`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b988269) feat(backend,desktop,daemon): launch the hev TUN engine
- [`518c9a7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/518c9a7) feat(core): hev-socks5-tunnel config builder + external-tun tuning
- [`db8c066`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/db8c066) fix(desktop): wrap raw-pointer deref in unsafe block (edition 2024)
- [`b51760a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b51760a) feat(settings): TUN engine settings section
- [`7ee2f5d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7ee2f5d) feat(core,desktop,daemon): wire TUN engine into the data path
- [`cdf3078`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cdf3078) fix(android): surface tun2socks spawn failure instead of swallowing it
- [`2401db9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2401db9) feat(core): per-core TUN engine selection (abstraction)
- [`c8c43f2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c8c43f2) fix(android): defer local-port guard until core is up

## v0.4.2 — 2026-06-29

### Core updates

- sing-box: `v1.13.13` → `v1.13.14`

### Changes

- [`7bd10f7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7bd10f7) fix(desktop): include xray dns.servers in the bypass CIDR set
- [`4c04ed5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4c04ed5) fix(desktop): lift data-path caps into the helper's ambient set; one spawn path
- [`5aa72f1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5aa72f1) test(core): expand validation matrix with per-field builder branches
- [`c5faf9b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c5faf9b) fix(desktop): grant the active core CAP_NET_ADMIN under the caps-only helper
- [`7907be5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7907be5) feat(desktop): build rpm bundle
- [`1bf3b2e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1bf3b2e) fix(singbox): PEM-wrap ECH config
- [`da607f7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/da607f7) fix(profiles): delete unreachable by id, keep test status
- [`244f276`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/244f276) fix(ui): close select on overlay click, not pointerdown
- [`3cfa31d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3cfa31d) feat(profiles): open the test-core log behind a failed result
- [`2d0542e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2d0542e) feat(backend): retain failed test-core logs per profile
- [`4f1c4eb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4f1c4eb) fix(desktop): keep the windows resume watcher future Send
- [`da61579`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/da61579) fix(desktop): correct windows-sys power handle out-param type
- [`c6baa53`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c6baa53) feat(desktop): signal system resume to the service
- [`437a9a8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/437a9a8) feat(backend): restart the data-path on system resume
- [`8b28674`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8b28674) fix(backend): wait for the core to be reaped after SIGKILL
- [`eb0946d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/eb0946d) fix(desktop): sweep orphaned sing-box auto_route rules on stop/start
- [`60e747c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/60e747c) fix(subs): replace native time picker with an in-house clock-dial
- [`eeef7f9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/eeef7f9) fix(frontend): stop batch ping/speed test from no-oping on a stale bridge cache
- [`4664f22`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4664f22) feat(logs): always reverse log order — newest lines on top
- [`479ab01`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/479ab01) fix(core): expand dedup key to full serialized profile minus bookkeeping
- [`5dd2f6f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5dd2f6f) fix(frontend): use Iconify-format SVGs for lan/wifi_off/stars icons
- [`3844188`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3844188) feat(core): intent-based AppState mutation + active-id fixup
- [`d092287`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d092287) fix(frontend): keep FAB scroll clearance in the desktop layout
- [`908a6fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/908a6fe) fix(frontend): drop the obsolete list-row icon translateZ(0) hack
- [`5c6e442`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5c6e442) fix(frontend): inline icon SVGs so webkit2gtk stops rendering squares
- [`23efdec`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/23efdec) fix(desktop): pin the uplink source address so the tun-escape bind survives multi-homing
- [`2f689c2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2f689c2) fix(core): set ws Host to the server domain when the profile leaves it empty
- [`3bd4294`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3bd4294) fix(desktop): reap the data-path core when the helper dies
- [`fb1c4cc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fb1c4cc) feat(core): accept DNS URL schemes (DoH/DoT/DoQ) in sing-box config
- [`51d2d06`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/51d2d06) fix(nix): set tauri app version from appVersion
- [`b14d3e0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b14d3e0) fix(nix): run install hooks so the .desktop entry is copied
- [`3b624da`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3b624da) fix(ui): blur number inputs on wheel scroll
- [`22acc54`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/22acc54) fix(core): keep force-in off a custom http_port
- [`233a47c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/233a47c) feat(backend): route proxied fetches through force-in, not socks-in
- [`f753647`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f753647) feat(core): always-on force-in inbound that bypasses geo routing
- [`50c90a9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/50c90a9) fix(desktop): honor KASUMI_HELPER_BIN over the NixOS wrapper
- [`a0afc81`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a0afc81) fix(desktop): bind core egress outbounds to uplink to break geo-direct TUN loop
- [`05e3815`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/05e3815) test(core): add a settings/routing matrix to core_validation
- [`9c04b7a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9c04b7a) test(core): drop byte-exact golden config fixtures
- [`3fb4c22`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3fb4c22) fix(desktop): write app log to datadir/daemon.log for the in-app viewer
- [`5d0d913`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5d0d913) fix(backend): surface subscription fetch cause, drop redundant URL
- [`d6e7270`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d6e7270) build(nix): source cores from the catalog, drop the geodat2srs clone app
- [`67fca8d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/67fca8d) build(cores): unify the fetch scripts behind a shared cores.json catalog
- [`754d9e6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/754d9e6) fix(desktop): build and bundle geodat2srs for rule_set .srs generation
- [`1c8e77c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1c8e77c) feat(nix): grant the helper caps by default, drop the opt-in + polkit path
- [`2472d44`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2472d44) fix(backend): gate the pre_exec spawn imports to cfg(unix)
- [`b53cc1b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b53cc1b) style(desktop): rustfmt the stack, clarify the run_dir comment
- [`ff73fb2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ff73fb2) feat(nix): add a security.wrappers caps option for the helper
- [`2a40404`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2a40404) feat(desktop): setcap the helper from the deb postinstall
- [`ab45d2c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ab45d2c) feat(desktop): grant helper caps via a one-time pkexec setcap
- [`99a84b9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/99a84b9) feat(desktop): grant test cores an ambient CAP_NET_RAW across exec
- [`48cf9d9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/48cf9d9) feat(desktop): seed inheritable CAP_NET_RAW + switch the bind gate to a real cap check
- [`f61ccb5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f61ccb5) feat(backend): add a pre_exec spawn seam for the forked child
- [`6a8c9b8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6a8c9b8) feat(desktop): drop the helper's bounding set to least-privilege caps
- [`e51085c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e51085c) build(desktop): add the caps crate for Linux least-privilege
- [`4f77603`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4f77603) fix(desktop): bind test cores to the uplink instead of per-test routes
- [`bd9c271`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bd9c271) fix(nix): inject product version into Tauri config
- [`2ca61d7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2ca61d7) feat(frontend): sync service state to tray, route start/stop actions
- [`95d547d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/95d547d) feat(desktop): conditional tray menu — Start/Stop/Restart by proxy state
- [`da17020`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/da17020) feat(desktop): native file picker for backup & routing import/export
- [`ab4adf5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ab4adf5) feat(desktop): tray quick-switch and restart
- [`00a8775`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/00a8775) feat(desktop): use the native clipboard with a web fallback
- [`57974e8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/57974e8) fix(frontend): animate the side rail when an overlay opens
- [`c9fe024`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c9fe024) fix(desktop): report runtime version in app_version
- [`4a81d70`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4a81d70) fix(desktop): defer the data-path bring-up off the setup thread
- [`9455b47`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9455b47) feat(desktop): file logging for the GUI and the privileged helper
- [`da0dca0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/da0dca0) fix(desktop): drop the duplicate tray icon from the config
- [`2a50851`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/2a50851) feat(module): add action/webui icons
- [`f8f3dec`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f8f3dec) feat(module): clean uninstall via `kasumi-proxy stop`
- [`680ed14`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/680ed14) test(desktop): cover quote_arg backslash/quote escaping
- [`e484dba`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e484dba) fix(desktop): quote elevated helper args per CommandLineToArgvW
- [`ce9ea38`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ce9ea38) feat(desktop): portable Windows runs the helper transiently, not as a service
- [`83dc5d2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/83dc5d2) build(windows): register the data-path service from the NSIS installer
- [`57ef65b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/57ef65b) feat(desktop): Windows data-path runs in a LocalSystem service
- [`f4d728e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f4d728e) fix(desktop): harden helper socket perms, drop dead unlink
- [`fd3d366`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fd3d366) feat(nix): opt-in passwordless elevation scoped to the helper
- [`c3217f4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c3217f4) build: ship kasumi-helper in every package channel
- [`1651d38`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1651d38) feat(desktop): GUI runs unprivileged, spawns the root helper (Linux)
- [`d332a4c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d332a4c) feat(desktop): privilege helper binary, elevated spawn + socket perms
- [`bb54bbd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bb54bbd) feat(desktop): RemotePlatform — GUI-side Platform over the helper
- [`3d0df60`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/3d0df60) feat(desktop): privsep server dispatcher + client transport
- [`cd0a3a6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cd0a3a6) feat(desktop): privilege-separation wire protocol
- [`d613233`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d613233) feat(nix): add a programs.kasumi-proxy NixOS module
- [`4ddd1de`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4ddd1de) fix(desktop): forward iproute2 to the elevated Linux data-path on NixOS
- [`6749982`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6749982) fix(nix): give the @2x icon a legal store-path name
- [`6f30d0c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6f30d0c) feat(nix): make kasumi-desktop a proper installable package
- [`20c745e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/20c745e) feat(flake): declare the Cachix cache as a substituter in nixConfig
- [`c9f6a9e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c9f6a9e) docs(readme): document the Cachix binary cache for local builds
- [`9ec1d0d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9ec1d0d) test(core): validate generated configs against real xray/sing-box
- [`bfb006f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/bfb006f) test(backend): cover pid_matches_any candidate scan
- [`0ec3efe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0ec3efe) test(core): cover migrate intermediate-shape retag and version clamp
- [`0859d9a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0859d9a) test(desktop): cover bypass-CIDR aggregation over literal servers
- [`c83bad4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c83bad4) test(backend): cover proxy-required fetch, port leasing, tun2 cleanup
- [`7a9f35f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7a9f35f) test(core): cover config_shared, forced-core branches, sub-apply helpers
- [`f8508da`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f8508da) build(cores): ship libcronet next to sing-box for the naive outbound
- [`27501ca`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/27501ca) fix(singbox): drop uTLS from the naive outbound
- [`c88f201`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c88f201) fix(core): route xray-only shadowsocks ciphers to xray
- [`4dd2fd1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4dd2fd1) feat(profiles): explain why a group can't be deleted
- [`f77a855`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f77a855) feat(settings): drop redundant current-core row from diagnostics
- [`ccbe82f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ccbe82f) feat(settings): surface installed core versions and TUN in diagnostics
- [`281d759`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/281d759) fix(ui): keep inline Escape edits from closing their sheet
- [`5c80afc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5c80afc) feat(ui): dismiss sheets and dialogs on Escape
- [`adab839`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/adab839) feat(subscriptions): unify add entry points and enrich bulk import
- [`a81e74d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a81e74d) feat(frontend): cross-platform Material select dropdown
- [`0044ee2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0044ee2) docs(readme): match portable zip names to the unified scheme
- [`99949cd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/99949cd) feat(ui): animate search field expand and FAB entrance
- [`4834ea7`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4834ea7) feat(ui): pop ping/speed results in when a test finishes
- [`a7415f2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a7415f2) fix(ui): keep the select-box arrow visible on focus
- [`9973558`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9973558) feat(ui): show toasts as a dismissible queue
- [`31102c4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/31102c4) fix(ui): animate the toast on dismiss instead of vanishing

## v0.4.1 — 2026-06-22

### Changes

- [`faf9069`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/faf9069) fix(profiles): stop group icons resizing on drag-drop
- [`5329240`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5329240) fix(desktop): fully collapse the side rail when hidden
- [`aa9cd08`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/aa9cd08) fix(profiles): keep delete dialogs mounted so they animate out
- [`32ba106`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/32ba106) fix(ui): animate dialog exit instead of unmounting instantly
- [`97a6ac0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/97a6ac0) fix(ui): animate bottom sheet on close instead of popping out
- [`038bb5b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/038bb5b) fix(ui): track sheet swipe on window so mouse drag works on desktop
- [`f164a28`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f164a28) feat(ui): swipe down to dismiss bottom sheets
- [`64727a9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/64727a9) fix(desktop): hide side rail while a bottom sheet is open
- [`b81be5c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b81be5c) fix(ci): detect changed areas from merge-base, not base..head
- [`503ba49`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/503ba49) fix(i18n): pluralize count-bearing strings via plural() helper
- [`4ff51a4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4ff51a4) feat(profiles): reorder groups via drag-and-drop
- [`6b15472`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6b15472) feat(subscriptions): per-subscription copy URL
- [`0af325c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0af325c) feat(subscriptions): import subscriptions from clipboard
- [`62dc8c3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/62dc8c3) feat(subscriptions): export subscriptions to clipboard
- [`a5e5c86`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a5e5c86) fix(ci): don't sign updater artifacts in nightly
- [`b207492`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b207492) test(core): init socks-auth test settings via struct update
- [`f0f08bb`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f0f08bb) feat(settings): wire up three dropped UI strings
- [`0f562b9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0f562b9) feat(settings): SOCKS/HTTP inbound authentication
- [`1fa5c28`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/1fa5c28) docs: refresh the PR template for the Rust/Tauri stack
- [`883ed7b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/883ed7b) feat(frontend): app version + auto-update controls in Settings
- [`84ac7e0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/84ac7e0) feat(desktop): wire the updater plugin + bundle signing config
- [`b997d03`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b997d03) docs: document the Linux portable zip
- [`9ca0b63`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9ca0b63) feat(desktop): honour a portable.dat marker on Linux
- [`0cb3c93`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0cb3c93) docs: Windows desktop install instructions
- [`9f8fa71`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9f8fa71) fix(frontend): use the standard card surface for quick actions
- [`81c983d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/81c983d) fix(frontend): lower the snackbar on desktop
- [`20ead8d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/20ead8d) fix(desktop): native backslash paths on Windows
- [`f9eece6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f9eece6) fix(desktop): keep the inherited env on Windows so cores can use Winsock
- [`91a8e2b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/91a8e2b) fix(desktop): bundle the app, not the codegen bin (default-run)
- [`fc6b4ef`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fc6b4ef) fix(desktop): suppress console windows when spawning on Windows
- [`489ed79`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/489ed79) docs: add Windows to the platform badge
- [`40174a8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/40174a8) fix(desktop): only the xray path needs wintun.dll on disk
- [`af03cbe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/af03cbe) build(desktop): bundle wintun.dll for the Windows target
- [`7bb5c72`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7bb5c72) feat(desktop): Windows Platform (wintun tun + route/netsh routing)
- [`a6ec99a`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a6ec99a) feat(backend): make tun2socks fwmark optional
- [`67c098e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/67c098e) feat(backend): portable process identity (POSIX + Windows)
- [`e4db159`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e4db159) fix(core): drop uTLS from hysteria2/tuic sing-box outbounds
- [`104819b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/104819b) docs: publish the AppImage release signing public key

## v0.4.0 — 2026-06-20

### Cross-platform: Rust backend + Tauri desktop

Base migration off the original Bash backend (with its React WebUI) to a Rust
workspace (`kasumi-core` / `kasumi-backend` / `kasumi-daemon`), with two thin
shells over one shared `Service`:

- **Android** — the same KSU/Magisk/APatch module, now a Rust `kasumi-proxy`
  daemon (axum HTTP webroot + token-gated typed WS).
- **Linux desktop (new)** — a Tauri 2 app owning the data path with a real TUN:
  system tray + minimize-to-tray, autostart, single-instance, and window-state.

Highlights:

- Nested `Profile` model; the frontend runs on TypeScript bindings + Zod schemas
  + runtime defaults **generated from the Rust types** — one source of truth, no
  hand-duplicated values.
- Versioned on-disk migrations (flat → nested) — existing installs keep their
  profiles (verified on a 324-profile device dump).
- Truthful **5-state status** (`stopped / connecting / connected / noInternet /
  failed`) via an end-to-end probe; per-profile diagnostics stream as they finish.
- Desktop installers (deb / appimage / nsis / msi) bundle the cores;
  `nix build .#kasumi-desktop` is self-contained.

---

## v0.3.4 — 2026-06-10

### Changes

- [`042437c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/042437c) fix(store): restart active profile only when its config changes
- [`948f58f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/948f58f) feat(settings): add toggle to allow non-localhost proxy access (#43)
- [`7eaf0fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7eaf0fe) fix(store): use daemon fetch timestamp for subscription lastUpdated (#42)
- [`65c19fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/65c19fe) fix: preserve profiles manually moved from subscription group on update (#41)
- [`277b192`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/277b192) fix(overview): show the engine that is actually running
- [`20b5bf2`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/20b5bf2) fix(module): report the running core's engine in status
- [`33dcac1`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/33dcac1) fix(editor): pin the engine selector to the forced core
- [`8facd2f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8facd2f) fix(singbox): emit sniff + hijack-dns route rules
- [`99d2964`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/99d2964) fix(core): run xray-style custom gRPC paths on xray only
- [`a366c25`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a366c25) feat(subscriptions): consume auto-update cache while the UI stays open
- [`6f7edc3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6f7edc3) fix(service): open sub-wake pipe read-write to unblock auto-update daemon
- [`cc51296`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/cc51296) fix(service): rename reserved awk variable breaking subscription listing
- [`6d208cc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6d208cc) feat(settings): add dedup on sub update toggle (#36)
- [`9b3be55`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9b3be55) fix(profiles): scope ping, selectBest, removeUnreachable, and removeDuplicates to current group (#35)
- [`ef3f65e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ef3f65e) fix(profiles): sort offline profiles (ping=-1) to bottom when sorting by ping (#34)
- [`4e4cd86`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4e4cd86) fix(storage): persist large state via native file I/O, split profiles.json (#33)
- [`0ad455d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0ad455d) fix(schema): tolerate invalid profiles/settings and report skipped on import (#32)
- [`e24283d`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/e24283d) fix(hydrate): show UI before slow asset/status I/O (#31)
- [`8f124ae`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8f124ae) fix(schema): drop grpc from TRANSPORT_NEEDS_PATH (#30)
- [`c58e18e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c58e18e) fix(schema): accept non-RFC-variant UUIDs via explicit hex regex (#29)
- [`fb855ef`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fb855ef) fix(i18n): drop profiles count from backup summary
- [`f306939`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f306939) fix(backup): validate imported backup against schema in mock bridge
- [`5e10e32`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/5e10e32) fix(backup): preserve current profiles when importing backup in replace mode
- [`d733789`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d733789) feat(backup): remove profile export from backup JSON
- [`c4b56bd`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/c4b56bd) fix(schema): make profiles optional in AppStateSchema for backup compatibility
- [`72341dc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/72341dc) feat(subscriptions): per-subscription download mode (auto/proxy/direct)
- [`4f34c5b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4f34c5b) fix(assets): restore download_asset_impl lost in helper refactor (#26)
- [`0a5b4a0`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0a5b4a0) fix(assets): restore download_asset_impl lost in helper refactor
- [`4d5e143`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4d5e143) fix(profiles): stream batch ping/speed results progressively (#25)
- [`f75e862`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/f75e862) feat(ui): add spinner for in-progress tests and red '—' for failures in profile rows (#24)
- [`75f31a3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/75f31a3) fix(install): ship bin/utils.sh in the module package (#22)
- [`a114c60`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a114c60) fix(schema): accept non-RFC-variant UUIDs for vless/vmess (#20)
- [`6546e9e`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6546e9e) feat(subscriptions): wake sub-update daemon on upsertSub
- [`9af73fe`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/9af73fe) feat(service): replace 1-min polling with event-driven sub-update scheduling

## v0.3.3 — 2026-06-08

### Changes

- [`059fe75`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/059fe75) fix(share): preserve full profile name when fragment contains spaces (#17)
- [`4b07317`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/4b07317) fix(service): point xray asset dir at DATADIR
- [`62865b5`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/62865b5) fix(service): avoid SC2015 in sub auto-update guard
- [`52a3c45`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/52a3c45) feat(service): subscription auto-update daemon + proxyctl sub-cache commands
- [`de4f8ac`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/de4f8ac) feat(subscriptions): consume backend auto-update cache on hydrate
- [`347457b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/347457b) feat(subscriptions): edit interval as HH:MM time picker
- [`afb5a6b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/afb5a6b) feat(schema): version state by module version, migrate sub interval to minutes (#12)
- [`6f0bbd9`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6f0bbd9) fix(subscriptions): auto-derive allowInsecure, warn on plain HTTP
- [`7135713`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/7135713) fix(subscriptions): drop duplicate enable toggle in edit sheet
- [`6c06f29`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/6c06f29) fix(subscriptions): show date and time of last update
- [`51132b8`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/51132b8) i18n: use action verb for add-profile FAB across locales
- [`91e2733`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/91e2733) fix(profiles): keep FAB clear of last row, fix ru label
- [`d31b93c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/d31b93c) fix(profiles): reset ping/speed stats on clone
- [`b4acddc`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/b4acddc) docs(readme): add status badges
- [`8754a91`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8754a91) fix(deps): remove unused styling deps
- [`8aba4b3`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/8aba4b3) fix(ui): extract shared btn-reset utility class
- [`a747a9b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/a747a9b) fix(editor): drop unsafe Profile/ProfileView double casts
- [`ac36cee`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/ac36cee) fix(config): reuse splitCsv in sing-box generator
- [`46b2d2b`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/46b2d2b) feat(subscriptions): inline new group in edit sheet
- [`66df59f`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/66df59f) feat(profiles): group management sheet
- [`fe266d6`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/fe266d6) feat(store): delete group removes its profiles
- [`0eea5c4`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/0eea5c4) fix(overview): hide activity card when feed is empty
- [`52d380c`](https://github.com/loss-and-quick/Kasumi-Proxy/commit/52d380c) fix(changelog): link commit hashes to GitHub in CHANGELOG.md

## v0.3.2 — 2026-06-07

### Changes

- e4cdcc1 feat(store): add pushActivity to upsertProfile + test coverage for all activity events
- 9fa8f76 feat(i18n): add activity.profileSaved to all 8 locales
- e60e3f4 feat(store): add pushActivity to speedTestAll/removeUnreachable/removeDuplicates/downloadAsset
- aff1b28 feat(i18n): add speedTest/unreachable/duplicates/asset activity keys to all 8 locales
- 150d3bf feat(overview): replace hardcoded recent array with live activity feed + relative timestamps
- 5e6aec3 feat(store): wire ActivityService into useAppStore — recentActivity slice + pushActivity on key actions
- ae06fed feat(i18n): add activity event keys + time.now/ago to all 8 locales
- 6e383bd feat(activity): add ActivityService — capped in-memory event feed
- 15bebde fix(changelog): strip quotes from core versions, exclude ci/chore commits, require non-empty OLD for core update entries
- 5b39c7d fix(ci): strip quotes from pinned version parse in changelog

## v0.3.1 — 2026-06-07

### Fixes

- **Real ping no longer returns -1 for all profiles when run in batch.**
  Concurrent `realPingAll` workers all received the same SOCKS port from
  `freePort` (TOCTOU — the test core binds asynchronously after `*Start`
  returns). Replaced per-worker `freePort` with a single `freePorts` call
  that allocates a distinct port block per worker from one snapshot.
  `freePort` removed from `kasumi-proxyctl`; `freePorts <start> <count>
  [<span>]` is the new API.

## v0.3.0 — 2026-06-07

### Fixes

- **WebUI no longer freezes during tests.** A KernelSU `ksu.exec` call blocks the
  WebView renderer for the whole duration of the shell command, so running a test
  (core warmup + a curl of up to 15s) inside one exec hung the entire UI. RealPing,
  SpeedTest and TCPing now run as background jobs — a quick `*Start` spawns the work
  and returns, the UI polls a quick `*Status` every 250ms — so no exec blocks the
  renderer for more than ~250ms.
- TCPing/RealPing job files are keyed per request, so concurrent runs no longer race
  on a shared temp file, and the backgrounded test cores are reniced to lowest
  priority so they don't compete with the UI.

### Features

- While any test (TCPing/RealPing/SpeedTest) is in progress, all test actions are
  disabled in the ping and profile sheets — not just the matching one.
- Config-affecting settings sections are disabled while the proxy is running.

## v0.2.0 — 2026-06-07

