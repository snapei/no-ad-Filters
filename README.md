# 屏蔽Google和YouTube广告规则
# AdGuard DNS filter

前身为 *AdGuard 简化域名过滤器*。

该过滤器由其他几个过滤器（AdGuard Base 过滤器、社交媒体过滤器、跟踪保护过滤器、移动广告过滤器、EasyList 和 EasyPrivacy）组成，专门进行了简化，以更好地兼容 DNS 级广告拦截。

The direct link to the filter: https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt.

请注意，要使用该过滤器，必须支持基本的广告拦截规则语法。 [basic ad blocking rules syntax](https://kb.adguard.com/en/general/how-to-create-your-own-ad-filters). 仅提取主机文件没有太大意义。

This is a default filter for [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) and for the public [AdGuard DNS](https://adguard.com/en/adguard-dns/overview.html) servers.

### 如何手动构建 AdGuard DNS 过滤器

```
yarn install
yarn run build
```

The output is written to `Filters/filter.txt`.

## DNS 过滤器结构

### Ad servers广告服务器

#### 这些过滤列表可阻止用于在网站上提供和显示广告的域名

* [AdGuard Base filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/BaseFilter/sections/adservers.txt)

* [AdGuard Base filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/BaseFilter/sections/adservers_firstparty.txt)

* [AdGuard Base filter — foreign servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/BaseFilter/sections/foreign.txt)

* [AdGuard Mobile Ads filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/MobileFilter/sections/adservers.txt)

* [AdGuard Spanish/Portuguese filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/SpanishFilter/sections/adservers.txt)

* [AdGuard Spanish/Portuguese filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/FrenchFilter/sections/adservers_firstparty.txt)

* [AdGuard common Cyrillic filters ad servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/common-sections/adservers.txt)

* [AdGuard common Cyrillic filters ad servers — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/common-sections/adservers_firstparty.txt)

* [AdGuard Russian filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/RussianFilter/sections/adservers_firstparty.txt)

* [AdGuard Ukrainian filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/UkrainianFilter/sections/adservers_firstparty.txt)

* [AdGuard Belarusian language ad servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/Belarusian/sections/filter.txt)

* [AdGuard Bulgarian language ad servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/Bulgarian/sections/filter.txt)

* [AdGuard Kazakh language ad servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/CyrillicFilters/Kazakh/sections/filter.txt)

* [AdGuard Turkish filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/TurkishFilter/sections/adservers.txt)

* [AdGuard Turkish filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/TurkishFilter/sections/adservers_firstparty.txt)

* [AdGuard French filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/FrenchFilter/sections/adservers.txt)

* [AdGuard French filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/FrenchFilter/sections/adservers_firstparty.txt)

* [AdGuard Japanese filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/JapaneseFilter/sections/adservers.txt)

* [AdGuard Japanese filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/JapaneseFilter/sections/adservers_firstparty.txt)

* [AdGuard German filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/GermanFilter/sections/adservers.txt)

* [AdGuard Chinese filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/ChineseFilter/sections/adservers.txt)

* [AdGuard Chinese filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/ChineseFilter/sections/adservers_firstparty.txt)

* [AdGuard Dutch filter](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/DutchFilter/sections/adservers.txt)

* [AdGuard Dutch filter — first-party servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/DutchFilter/sections/adservers_firstparty.txt)

* [EasyList](https://raw.githubusercontent.com/easylist/easylist/master/easylist/easylist_adservers.txt)

* [EasyList — third-party servers](https://raw.githubusercontent.com/easylist/easylist/master/easylist/easylist_thirdparty.txt)

* [EasyList — adult third-party servers](https://raw.githubusercontent.com/easylist/easylist/master/easylist_adult/adult_adservers.txt)

* [EasyList — adult popup servers](https://raw.githubusercontent.com/easylist/easylist/master/easylist_adult/adult_adservers.txt)

* [EasyList Germany](https://raw.githubusercontent.com/easylist/easylistgermany/master/easylistgermany/easylistgermany_adservers.txt)

* [EasyList Italy](https://raw.githubusercontent.com/easylist/easylistitaly/master/easylistitaly/easylistitaly_adservers.txt)

* [EasyList China](https://raw.githubusercontent.com/easylist/easylistchina/master/easylistchina.txt)

* [EasyList Dutch](https://raw.githubusercontent.com/easylist/easylistdutch/master/easylistdutch/block_third_party_server.txt)

* [ABPindo](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/src/advert/adservers.txt)

* [ABPindo — third-party servers](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/src/advert/thirdparty.txt)

* [AdblockID](https://raw.githubusercontent.com/realodix/AdBlockID/master/src/adservers.adfl)

* [hostsVN](https://raw.githubusercontent.com/bigdargon/hostsVN/master/filters/adservers.txt)

* [hostsVN Threat](https://raw.githubusercontent.com/bigdargon/hostsVN/master/extensions/threat/filter.txt)

### 跟踪服务器

#### 这些过滤列表阻止用于跟踪和分析的域

* [AdGuard Tracking Protection filter — third-party trackers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/SpywareFilter/sections/tracking_servers.txt)

* [AdGuard Tracking Protection filter — first-party trackers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/SpywareFilter/sections/tracking_servers_firstparty.txt)

* [AdGuard Tracking Protection filter — mobile trackers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/SpywareFilter/sections/mobile.txt)

* [EasyPrivacy](https://raw.githubusercontent.com/easylist/easylist/master/easyprivacy/easyprivacy_trackingservers.txt)

* [EasyPrivacy — third-party trackers](https://raw.githubusercontent.com/easylist/easylist/master/easyprivacy/easyprivacy_thirdparty.txt)

* [EasyPrivacy — international trackers](https://raw.githubusercontent.com/easylist/easylist/master/easyprivacy/easyprivacy_trackingservers_international.txt)

* [EasyPrivacy — third-party international](https://raw.githubusercontent.com/easylist/easylist/master/easyprivacy/easyprivacy_thirdparty_international.txt)

### Cryptominers加密者

#### 这些过滤列表用于过滤加密者

* [AdGuard Base filter cryptominers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/BaseFilter/sections/cryptominers.txt)

### Exception

#### These lists are used to exclude domains that cause serious site breakages

* [Exclusion rules](https://github.com/AdguardTeam/AdGuardSDNSFilter/blob/master/Filters/exclusions.txt)
* [Exception rules](https://github.com/AdguardTeam/AdGuardSDNSFilter/blob/master/Filters/exceptions.txt)

### News Exchange

#### These lists are used to block teaser advertisements

* [AdGuard Russian filter news exchange servers](https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/RussianFilter/sections/news_exchange.txt)

### Regional lists

#### These filter lists block various types of advertising, tracking, scams and malware on sites of a specific language group

* [Frellwits Swedish Filter](https://raw.githubusercontent.com/lassekongo83/Frellwits-filter-lists/master/Frellwits-Swedish-Hosts-File.txt)
* [Persian Blocker Hosts](https://raw.githubusercontent.com/MasterKia/PersianBlocker/main/PersianBlockerHosts.txt)

### Others

* [Additional rules](https://github.com/AdguardTeam/AdGuardSDNSFilter/blob/master/Filters/rules.txt)
