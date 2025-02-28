[![GitHub issues](https://img.shields.io/github/issues/yokoffing/NextDNS-Config)](https://github.com/yokoffing/NextDNS-Config/issues)
[![GitHub closed issues](https://badgen.net/github/closed-issues/yokoffing/NextDNS-Config?color=green)](https://github.com/yokoffing/NextDNS-Config/issues?q=is%3Aissue+is%3Aclosed)
![GitHub repo size](https://img.shields.io/github/repo-size/yokoffing/NextDNS-Config)
![GitHub](https://img.shields.io/github/license/yokoffing/NextDNS-Config?color=blue)
![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-green)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/yokoffing/NextDNS-Config)
![GitHub last commit](https://img.shields.io/github/last-commit/yokoffing/NextDNS-Config)
![GitHub Maintained](https://img.shields.io/badge/maintained-yes-green)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyokoffing%2FNextDNS-Config&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

***
# Guidelines :bookmark:
1) Prevent overblocking by utilizing the [law of diminishing returns](https://pmctraining.com/site/wp-content/uploads/2018/04/Law-of-Diminishing-Returns-CHART.png) (e.g., using [sane](https://www.privacyguides.org/basics/threat-modeling/), quality [blocklists](https://github.com/yokoffing/NextDNS-Config#blocklists-1); allowing most [TLDs](https://github.com/yokoffing/NextDNS-Config#block-top-level-domains-tlds-1-2-3-4-5); etc.).
2) Pass the [girlfriend test](https://www.urbandictionary.com/define.php?term=Grandma%20Test) with few exceptions. These deviations are documented throughout the guide.

***

## Create your account

Sign up for NextDNS [here](https://nextdns.io/?from=xujj63g5)!

***

# Security :policeman:

Security settings protect your data from harm, theft, and unauthorized use.<sup>*^[why does this matter?](https://thenewoil.org/why.html)*</sup>

### Threat Intelligence Feeds <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/security/threat-intelligence-feeds.json)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Use Threat Intelligence Feeds
### AI-Driven Threat Detection
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable AI-Driven Threat Detection
### Google Safe Browsing <sup><sup> [1](https://user-images.githubusercontent.com/11689349/107696360-d8dde800-6c7f-11eb-9882-cccc8d2065c5.jpg) [2](https://safebrowsing.google.com/safebrowsing/report_general/) [3](https://the8-bit.com/apple-proxies-google-safe-browsing-privacy/) [4](https://github.com/brave/brave-browser/wiki/Deviations-from-Chromium-(features-we-disable-or-remove)#services-we-proxy-through-brave-servers) </sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Google Safe Browsing
### Cryptojacking Protection <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/security/cryptojacking.json)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Cryptojacking Protection
### DNS Rebinding Protection <sup><sup>[1](https://help.nextdns.io/t/35hmval/what-is-dns-rebinding-protection) [2](https://www.reddit.com/r/nextdns/comments/t0ne8r/does_dns_rebinding_protection_block_remote_access/?context=3)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg)  Enable DNS Rebinding Protection
### IDN Homograph Attacks Protection
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Homograph Attacks Protection
### Typosquatting Protection <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/security/typosquatting/protected-domains)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Typosquatting Protection
### Domain Generation Algorithms (DGAs) Protection
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable DGA Protection
### Block Newly Registered Domains (NRDs) <sup><sup>[1](https://www.malwarebytes.com/glossary/phishing) [2](https://old.reddit.com/r/uBlockOrigin/comments/w64sqt/comment/ihboutk/?context=3) [3](https://www.boldgrid.com/instagram-influencer-accounts-are-being-hacked-phishing-attacks/) </sup></sup>
:warning: Blocking NRDs may cause [false positives](https://csrc.nist.gov/glossary/term/false_positive) [occasionally](https://old.reddit.com/r/InternetIsBeautiful/comments/w2wdro/comment/iguvg8y/?context=3). Be selective when adding NRDs to your allowlist; and, if you do, **NEVER** give [sensitive information](https://www.egnyte.com/guides/governance/sensitive-information) to a NRD. *If you plan to [set-and-forget](https://glosbe.com/en/en/set-and-forget) your configuration, disable this setting.*
<br><br>![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Block Newly Registered Domains (NRDs)
### Block Dynamic DNS Hostnames <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/security/ddns/suffixes) [2](https://twitter.com/NextDNS/status/1541740963760144386?cxt=HHwWhIC8iZ7PruUqAAAA) [3](https://www.phishing.org/what-is-phishing) </sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Block Dynamic DNS Hostnames
### Block Parked Domains <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/security/parked-domains-cname)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Block Parked Domains
### Block Top-Level Domains (TLDs) <sup><sup>[1](https://webtribunal.net/blog/tld-statistics/) [2](https://www.spamhaus.org/statistics/tlds/) [3](https://www.bleepingcomputer.com/news/security/verified-twitter-accounts-hacked-to-send-fake-suspension-notices/) [4](https://github.com/iam-py-test/my_filters_001/blob/main/enhanced_protection.txt) [5](https://github.com/DandelionSprout/adfilt/blob/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt) [6](https://github.com/DandelionSprout/adfilt/issues/659#issuecomment-1284845803) </sup></sup>
:warning: Blocking [TLDs](https://www.geeksforgeeks.org/components-of-a-url/) may cause [false positives](https://csrc.nist.gov/glossary/term/false_positive) since this feature blocks both site nagviations and subrequests. However, the entries below should allow for everyday browsing while offering protection against commonly abused TLDs.

```
.buzz
.cricket
.discount
.gdn
.loan
.loans
.ooo
.sbs
.wang
```

:stop_sign: Below are additional TLDs you may block, but you may need to [allowlist](https://github.com/yokoffing/NextDNS-Config#allowlist-white_check_mark) sites on occasion. *If you plan to [set-and-forget](https://glosbe.com/en/en/set-and-forget) your configuration, skip this setting.*

<details>

```
.work
.fit
.surf
.asia
.tokyo
.monster
---
.agency
.associates
.bid
.cam
.casa
.cf
.ci
.cyou
.fun
.ga
.gq
.link
.live
.ml
.icu
.rest
.shop
.webcam
.win
```

</details>

:memo: If you would rather block TLDs with an adblocker (e.g., easier to troubleshoot breakage), add the first two filterlists [here](https://github.com/yokoffing/filterlists#security).

### Block Child Sexual Abuse Material
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Block Child Sexual Abuse Material

***

# Privacy :lock:
Privacy features limit the amount of data that companies can collect about you. Privacy is a [spectrum](https://blog.thenewoil.org/the-privacy-myth-binary-vs-spectrum). What you need varies on your [threat model](https://thenewoil.org/threatmodel.html), interest, and skillset.<sup>^[*why should I care? I have nothing to hide*](https://aeon.co/essays/privacy-matters-because-it-empowers-us-all)</sup>

### Blocklists <sup><sup>[1](https://github.com/nextdns/metadata/tree/master/privacy/blocklists)</sup></sup>

Blocklists are community generated lists that block ads and [trackers](https://www.freecodecamp.org/news/what-you-should-know-about-web-tracking-and-how-it-affects-your-online-privacy-42935355525/). Filters can be categorized into five tiers of coverage:
1) **None**: no breakage; NextDNS still protects against malicious threats (à la [security settings](https://github.com/yokoffing/NextDNS-Config#security-cop)) but will allow ads and trackers
2) **Basic**: rare breakage; prioritizes functionality over blocking; *very* forgiving
3) **Balanced**: minimal breakage; largely [set-and-forget](https://glosbe.com/en/en/set-and-forget) but you may need to allowlist occasionally to [unsubscribe from junk email](https://old.reddit.com/r/nextdns/comments/y3zmhb/new_on_nextdns_and_im_loving_it_any_advices_about/ish8dla/?context=1)
4) **Strict**: moderate breakage; prioritizes privacy over user experience; must [manage your allowlist](https://github.com/yokoffing/NextDNS-Config#allowlist-white_check_mark) regularly
5) **Aggressive**: excessive breakage; use on a separate profile to [lockdown single-purpose devices](https://old.reddit.com/r/nextdns/comments/uqap3n/comment/i8q8alf/?context=3)

We recommend you select the minimum number of useful lists. Here are the suggested blocklists for each category:

|     Basic     |    Balanced   |    Strict    |     Aggressive     |
|:-------------:|:-------------:|:------------:|:------------------:|
| 1Hosts (mini) | 1Hosts (Lite) | 1Hosts (Pro) |    1Hosts (Xtra)   |
|               |      oisd     |     oisd     |     Goodbye Ads    |

:bulb: The **Balanced** tier is recommended for everyday browsing, based on my testing and user feedback.<sup>[1](https://old.reddit.com/r/nextdns/comments/s2gzc5/oisd_vs_1hostsminiliteproxtra/hsgmp5n/) [2](https://old.reddit.com/r/nextdns/comments/xoyyw2/nextdns_as_a_set_it_and_forget_it_solution/iq1k6tx/) [3](https://www.reddit.com/r/nextdns/comments/vuon2a/comment/iffd682/) [4](https://old.reddit.com/r/nextdns/comments/vn8olr/please_could_someone_recommend_me_a_good/ie5meel/?context=2) [5](https://www.reddit.com/r/nextdns/comments/yryq3c/comment/ivwr8tp/?context=3) </sup>

:question: You may wonder why other lists are not utilized. This is because many list maintainers:
* do not remove [false positives](https://csrc.nist.gov/glossary/term/false_positive) and/or are no longer active <sup>[1](https://github.com/lightswitch05/hosts/issues/356) [2](https://github.com/EnergizedProtection/block/issues/916) [3](https://github.com/notracking/hosts-blocklists/issues/815#issuecomment-1317556798)</sup>
* already aggregate common blocklists into their own list (Easylist/Fanboy, AdGuard, Steven Black, etc.) <sup>[1](https://github.com/badmojr/1Hosts/blob/master/-data/lists/assets.txt) [2](https://oisd.nl/includedlists/full/0) [3](https://github.com/notracking/hosts-blocklists/blob/master/SOURCES.md) [4](https://github.com/StevenBlack/hosts#sources-of-hosts-data-unified-in-this-variant) [5](https://github.com/EnergizedProtection/block#packs-2)</sup>
* offer no meaningful additional coverage when compared with the chart combinations above <sup>[1](https://www.reddit.com/r/nextdns/comments/ys3s1s/comment/ivxdcd2/?context=3)</sup>

### Native Tracking Protection <sup><sup>[1](https://github.com/nextdns/metadata/tree/master/privacy/native)</sup></sup>

Add all the device brands that you use. There's no advantage in adding brands you don't have; however, there’s no disadvantage in adding unused brands, either.

<details>

	Xiaomi
	Huawei
	Samsung
	Amazon Alexa
	Windows
	Apple
	Roku
	Sonos

</details>

### Block Disguised Third-Party Trackers <sup><sup>[1](https://github.com/nextdns/cname-cloaking-blocklist/blob/master/domains) [2](https://medium.com/nextdns/cname-cloaking-the-dangerous-disguise-of-third-party-trackers-195205dc522a) [3](https://arxiv.org/pdf/2102.09301.pdf) [4](https://tma.ifip.org/2020/wp-content/uploads/sites/9/2020/06/tma2020-camera-paper66.pdf) </sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Block Disguised Third-Party Trackers

### Allow Affiliate & Tracking Links <sup><sup>[1](https://github.com/nextdns/metadata/blob/master/privacy/affiliate-tracking-domains) [2](https://twitter.com/NextDNS/status/1539229377560461312) </sup></sup>
:bulb: Your IP address will automatically be hidden (via [TCP](https://www.educba.com/what-is-tcp-ip/) [proxying](https://en.wikipedia.org/wiki/Proxy_server#/media/File:Proxy_concept_en.svg)) to preserve your privacy.<p>
:warning: Disabling may cause [false positives](https://csrc.nist.gov/glossary/term/false_positive) when opening some emails. <p>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Allow Affiliate & Tracking Links

***

# Parental Control :family_man_woman_boy:
### YouTube Restricted Mode
![Disabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/disabled.svg) Enforce YouTube Restricted Mode
### Block Bypass Methods <sup><sup>[1](https://github.com/nextdns/metadata/tree/master/parentalcontrol)</sup></sup>
:warning: Enabling may cause unintended breakage. <p>
![Disabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/disabled.svg) Block Bypass Methods

***

# Denylist :no_entry:

Denylist entries block any requests from that source. The entries below may further harden `Balanced` [blocklist](https://github.com/yokoffing/NextDNS-Config#blocklists-1) profiles while not interfering with everyday browsing.

<details>
	
### Apple tracking domains <sup><sup>[1](https://twitter.com/mysk_co/status/1588308341780262912) [2](https://github.com/nextdns/metadata/pull/1132) [3](https://github.com/badmojr/1Hosts/issues/536) [4](https://old.reddit.com/r/nextdns/comments/vz9kla/at_last_nextdns_added_the_1host_xtra/ig8zsnn/)</sup></sup>
Not currently in NextDNS's [Native Tracking Protection](https://github.com/yokoffing/NextDNS-Config#native-tracking-protection-1) [list](https://github.com/nextdns/metadata/blob/master/privacy/native/apple): <sup>[1](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/wildcard/native.apple.txt)</sup>

	xp.apple.com
	acfeedbackws.icloud.com
	api-adservices.apple.com
	feedbackws.fe.apple-dns.net
	feedbackws.icloud.com
	iadsdk.apple.com
	notes-analytics-events.apple.com
	notes-analytics-events.news.apple-dns.net
	stocks-analytics-events.news.apple-dns.net
	weather-analytics-events.apple.com
	weather-analytics-events.news.apple-dns.net
	
### Twitter tracker

	syndication.twitter.com

### NVIDIA Gefore Experience <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/650)</sup></sup>

	events.gfe.nvidia.com

### Junk surveillance software

    spappmonitoring.com
    a-spy.com
    alltracker.org
    aispyer.com

</details>

***

# Allowlist :white_check_mark: 

Allowlist entries override any blocks. These entries may be needed for `Strict` and `Aggressive` [blocklist](https://github.com/yokoffing/NextDNS-Config#blocklists-1) profiles.

<details>

### Facebook / Instagram <sup><sup>[1](https://github.com/jerryn70/GoodbyeAds/issues/309)</sup></sup> 

	graph.facebook.com
	graph.instagram.com
	i.instagram.com

### Apple iMessage GIFs <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/560)</sup></sup> / Spotlight Search <sup><sup>[2](https://github.com/badmojr/1Hosts/issues/562)</sup></sup> 

	smoot.apple.com

### Apple Store <sup><sup>[1](https://www.reddit.com/r/nextdns/comments/xx4cwn/solutionapple_store_connection_issues/)</sup></sup> 

	amp-api-edge.apps.apple.com
	amp-api-search-edge.apps.apple.com

### Xiaomi device updates <sup><sup>[1](https://blocklist-tools.developerdan.com/entries/search?q=update.intl.miui.com)</sup></sup> 

	update.intl.miui.com

### Google Nest usage metrics <sup><sup>[1](https://old.reddit.com/r/nextdns/comments/yzvnuw/nest_usage_metrics_being_blocked/)</sup></sup> 

    logsink.devices.nest.com

### [Spectrum](https://www.spectrum.net) login <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/640)</sup></sup>

	pov.spectrum.net

### Zoom <sup><sup>[1](https://oisd.nl/excludes.php?w=log.zoom.us) [2](https://oisd.nl/excludes.php?w=us04logfiles.zoom.us)</sup></sup> 

	logfiles.zoom.us
	us04logfiles.zoom.us
	us04zpns.zoom.us

### YouTube history <sup><sup>[1](https://blocklist-tools.developerdan.com/entries/search?q=s.youtube.com)</sup></sup> 

	s.youtube.com

### Hulu <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/762)</sup></sup>

	ads-fa-darwin.hulustream.com

### Epic Games Launcher <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/643)</sup></sup>

	eulatracking-public-service-prod06.ol.epicgames.com

### NVIDIA Gefore Experience <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/650)</sup></sup>
	
	gfe.nvidia.com
	nvgs.nvidia.cn

### [imgur](https://imgur.com/) <sup><sup>[1](https://github.com/lightswitch05/hosts/issues/358) [2](https://old.reddit.com/r/nextdns/comments/t3jmvk/imgur_loads_then_goes_blank_no_matter_which/)</sup></sup>

	js.media-lab.ai

### [CBS](https://www.cbsnews.com/live/#x) News livestream <sup><sup>[1](https://github.com/nextdns/metadata/issues/1030)</sup></sup> 

	production-cmp.isgprivacy.cbsi.com

### [FiveThirtyEight](https://fivethirtyeight.com/) videos / [National Geographic](https://www.nationalgeographic.com/) website <sup><sup>[1](https://github.com/notracking/hosts-blocklists/issues/788)</sup></sup>

	dcf.espn.com

### [Men's Health](https://www.menshealth.com/nutrition/a40868905/chris-hemsworth-chicken-pasta-bake-recipe-centr/) videos <sup><sup>[1](https://github.com/badmojr/1Hosts/issues/651)</sup></sup>

	glimmer.hearstapps.com
    
### NextDNS
Just in case a [filterlist goes haywire](https://github.com/yokoffing/NextDNS-Config/issues/10#issuecomment-1327956655) and blocks your access

    nextdns.io

</details>

***

# Settings :gear:

### Logs
**Storage location** → Switzerland

### Block Page
:warning: Enabling may cause breakage if the [NextDNS Root CA](https://help.nextdns.io/t/g9hmv0a/how-to-install-and-trust-nextdns-root-ca) is not on your devices. This setting also breaks [iCloud Private Relay](https://support.apple.com/en-us/HT212614).<sup>[1](https://help.nextdns.io/t/g9hdska)</sup>
<br><br> ![Disabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/disabled.svg) Enable Block Page
### Anonymized EDNS Client Subnet <sup><sup>[1](https://help.nextdns.io/t/m1hmv04/what-is-edns-client-subnet-ecs) </sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Anonymized EDNS Client Subnet
### Cache Boost <sup><sup>[1](https://old.reddit.com/r/nextdns/comments/girmcf/new_setting_cache_boost/)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Cache Boost
### CNAME Flattening <sup><sup>[1](https://medium.com/nextdns/nextdns-added-cname-uncloaking-support-becomes-the-first-cross-platform-solution-to-the-problem-e3f437f84342) [2](https://developers.cloudflare.com/dns/additional-options/cname-flattening) [3](https://advancedweb.hu/what-is-cname-flattening-and-how-it-helps-redirecting-the-apex-domain/) </sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable CNAME Flattening
### Web3 <sup><sup> [1](https://twitter.com/NextDNS/status/1491034351391305731) [2](https://gabygoldberg.notion.site/f7050e62461143d49345e7b46eb5576b)</sup></sup>
![Enabled](https://raw.githubusercontent.com/crssi/NextDNS-Config/main/icons/enabled.svg) Enable Web3 → (optional)

***
# FAQ :question:

### How do I signup for NextDNS?
Click [here](https://nextdns.io/?from=xujj63g5)!

### Is it redundant to set DoH at browser-level if I'm already using it at system-level?
Unless you use a separate profile for the browser, it is not neccessary, and it should not slow down your web browsing.<sup>[1](https://old.reddit.com/r/nextdns/comments/yfjvqy/is_it_redundant_to_set_at_doh_at_browserlevel_if/iu3vjzt/?context=3)</sup> However, I recommend [setting it in your web browser](https://www.itechtics.com/dns-over-https/#how-to-enable-or-disable-dns-over-https-in-your-browsers) anyway. 

### If I have a profile for my router and another profile for my device, which one will my device use?
The device will use the profile set by the NextDNS app or the installed [root CA](https://help.nextdns.io/t/g9hmv0a/how-to-install-and-trust-nextdns-root-ca). However, if the device has not been configured to use a separate profile, then it will use the wifi/router configuration.<sup>[1](https://old.reddit.com/r/nextdns/comments/yf4hnv/question_about_home_router_and_app_running_in/)</sup>

### Can I block YouTube ads with NextDNS only?
[No, you can't](https://discourse.pi-hole.net/t/how-do-i-block-ads-on-youtube/253/2) block first-party ads using only DNS-level blocking. You will need an adblocker.

### What browser should I use that has adblocking?
* [Brave](https://brave.com) is a great choice, especially [if you prefer Chrome](https://youtu.be/VHwIyR6ca4o?t=249), want uninstrusive [fingerprint protection](https://brave.com/privacy-updates/4-fingerprinting-defenses-2.0/), and don't enjoy doing a lot of tweaking.<sup>[1](https://github.com/brave/brave-browser/wiki/Deviations-from-Chromium-(features-we-disable-or-remove)#what-chromium-features-are-removed-for-privacysecurity-reasons)</sup>
* [Firefox](https://www.mozilla.org/en-US/firefox/new/) with [uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/)<sup>[1](https://github.com/gorhill/uBlock/wiki/About-%22Why-uBlock-Origin-works-so-much-better-than-Pi%E2%80%91hole-does%3F%22)</sup> and configured using [Betterfox](https://github.com/yokoffing/Betterfox).
* [Orion](https://browser.kagi.com/) is a promising, [up-and-coming](https://idioms.thefreedictionary.com/up-and-coming) browser for Apple devices.

Here are the suggested browsers for each operating system:

| Browser | Windows | macOS | Linux | iOS | Android |
|:-------:|:-------:|:-----:|:-----:|:---:|:-------:|
|  Brave  |    x    |   x   |   x   |  x  |    x    |
| Firefox |    x    |   x   |   x   |     |         |
|  Orion  |         |   x   |       |  x  |         |

### What is the difference between security, privacy, and anonymity?
See [article](https://thenewoil.org/secprivanon.html) | [video](https://youtu.be/Wpkh-hfULgE)

### Does NextDNS hide activity from my Internet Service Provider (ISP)?
[No](https://www.reddit.com/r/nextdns/comments/tavcgm/comment/i039u1r/?context=3). NextDNS is only concerned about DNS traffic. You would need a [quality](https://www.youtube.com/watch?v=cK4MQv-OwyM) [VPN](https://www.ivpn.net/blog/why-you-dont-need-a-vpn/) to hide all activity from your ISP.

***
# Mentions :books:

User Comments: 
[1](https://reddit.com/r/moddedandroidapps/comments/wbud1e/aerowitter_twifucker_non_root_twitter_mod/iiloq0p/?context=2)
[2](https://reddit.com/r/nextdns/comments/xoyyw2/nextdns_as_a_set_it_and_forget_it_solution/?context=3)
[3](https://reddit.com/r/nextdns/comments/vxh4pt/comment/ifykqyh/?context=1)
[4](https://reddit.com/r/nextdns/comments/y3zmhb/comment/isc2o4q/?context=3)
[5](https://reddit.com/r/nextdns/comments/yp6o09/comment/ivhwook/?context=3)
[6](https://reddit.com/r/nextdns/comments/ys3s1s/comment/ivxdcd2/?context=3)
[7](https://reddit.com/r/nextdns/comments/yzvnuw/nest_usage_metrics_being_blocked/)

#### Guides
* [FMHY: DNS Adblocking](https://github.com/nbats/FMHYedit/blob/main/AdblockVPNGuide.md#-dns-adblocking) → NextDNS → Guide
* [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists#nextdns---limited-freepaid-) → Online DNS services

#### Contributions
* [1Hosts](https://github.com/badmojr/1Hosts/issues?q=is%3Aissue+author%3Ayokoffing+)
* [Easylist](https://github.com/easylist/easylist/issues?q=is%3Aissue+author%3Ayokoffing+)
* [AdGuard](https://github.com/AdguardTeam/AdguardFilters/issues?q=is%3Aissue+author%3Ayokoffing+)
* [uBlock Origin](https://github.com/uBlockOrigin/uAssets/issues?q=is%3Aissue+author%3Ayokoffing+)

***

# Support :heart:
I’m a one-person operation, working in mental health and running this page as a passion project in my time off. If you enjoy my work, please leave a tip! Your support is incredibly appreciated and allows me to dedicate time to this project :blush:

<img align="top" width="25px" src="https://coekuss.com/quietfox/bitcoin.png"> Bitcoin: 334gaiEjn6wY1VksQvYe5L668JjtPEPyiM

<img align="top" width="20px" src="https://coekuss.com/quietfox/paypal.png"> PayPal: [paypal.me](about:blank) (forthcoming)

***

<div align='center'><a href='https://www.websitecounterfree.com'><img src='https://www.websitecounterfree.com/c.php?d=9&id=19651&s=1' border='0' alt='Free Website Counter'></a><br / ></div>
<div align='center'>23 July 2022</div>
