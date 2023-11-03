<img src="https://github.com/gabefletch/DeltaBlock/assets/38300939/02815979-f67d-4dee-8865-178973114236" width=400><br>


[Skip to Installation Steps](https://github.com/gabefletch/DeltaBlock#installation)<br>

A custom DNS profile for NextDNS capable of blocking up to 99%* of ads.<br>
DeltaBlock stops both web-based and in-app ads from loading.<br>
A project by [@gabefletch](https://github.com/gabefletch).<br>

### Notice for New NextDNS Users
DeltaBlock is only designed for use via NextDNS, which is limited to 300,000 queries per month without a subscription. The lowest tier with unlimited queries is available for $1.99/month. Using the DeltaBlock custom profile, however, is completely free.

### NextDNS Affiliate Link
Help DeltaBlock remain running by sharing this link:
https://nextdns.io/?from=pyukpkuc

### Services With Anti-Adblocking Measures
DeltaBlock, like most adblockers, can be detected by sites with anti-adblock measures. YouTube on both mobile and desktop sites and some news sites are the most common examples of this. In other words, DeltaBlock cannot work properly on every site. If you're looking to get past adblock detection on YouTube, [see this guide](https://github.com/psychon-night/bypass-youtube-adblock-blocker/tree/main).<br>

*According to Toolz AdBlock Test. This percentage varies depending on network variables. DeltaBlock stops an average of 96% of ads at all times based on testing between both iOS and macOS devices. The lowest percentage resulting from testing has been 93%, under strenuous network variables with ad-heavy pages.<br>
### Readme Contents
[Installation](https://github.com/gabefletch/DeltaBlock#installation)<br>
[Included Blocklists](https://github.com/gabefletch/DeltaBlock#included-blocklists)<br>
[Changes](https://github.com/gabefletch/DeltaBlock#changes)<br>
[Frequently Asked Questions](https://github.com/gabefletch/DeltaBlock#FAQ)<br>

# Installation
## iOS, iPadOS, macOS, Android
### Via NextDNS App (Recommended)
- Install the NextDNS app on your device of choice
(Available for iOS, iPadOS, macOS or Android)
- Enter the settings for NextDNS and enter `4b3fba` as the Configuration ID.
### Via Apple Config File
(Apple Devices Only)
- [Click here](https://apple.nextdns.io/?profile=4b3fba) to be taken for the NextDNS Apple Config Profile generator for DeltaBlock.
- Download and install the profile via the Settings app.
## Windows
### Via NextDNS App (Recommended)
- Install the NextDNS app by [clicking here](https://nextdns.io/download/windows/stable).
- Enter the settings for NextDNS and enter `4b3fba` as the Configuration ID.
### or via DNS Over HTTPS (Windows 11 Only)
- Open the Settings app
- Go to Network & Internet
- Click on WiFi (or Ethernet)
- Click on Hardware Properties (or ignore this if you clicked Ethernet)
- Click the Edit button next to DNS Server Assignment
- Select Manual
- Enable IPv4
- Enter `45.90.28.0` as Preferred DNS, then select On (manual template) and enter `https://dns.nextdns.io/4b3fba`
- Enter `45.90.30.0` as Alternate DNS, then select On (manual template) and enter `https://dns.nextdns.io/4b3fba`
- Click Save
## Linux
### Via systemd-resolved (Recommended)
- Use the following in /etc/systemd/resolved/.conf:<br>
```
[Resolve]
DNS=45.90.28.0#4b3fba.dns.nextdns.io
DNS=2a07:a8c0::#4b3fba.dns.nextdns.io
DNS=45.90.30.0#4b3fba.dns.nextdns.io
DNS=2a07:a8c1::#4b3fba.dns.nextdns.io
DNSOverTLS=yes
```

## ChromeOS
### Via Secure DNS (Recommended)
- Open the Settings app
- Go to Security and Privacy
- Enable "Use Secure DNS"
- Select "With:Custom" and enter `https://dns.nextdns.io/4b3fba`

## Routers
- Utilize [NextDNS CLI](https://github.com/nextdns/nextdns/wiki).

## DNS-over-TLS/QUIC
`4b3fba.dns.nextdns.io`
## DNS-over-HTTPS
`https://dns.nextdns.io/4b3fba`
## DNS via IPv6
`2a07:a8c0::4b:3fba`<br>
`2a07:a8c1::4b:3fba`

# Included Blocklists
### NextDNS Ads & Trackers Blocklist
A comprehensive blocklist to block ads & trackers in all countries.<br>
- 151,328 entries.<br>
### AdGuard DNS Filter
A filter composed of several other filters (AdGuard Base filter, Social Media filter, Tracking Protection filter, Mobile ads filter, EasyList, and EasyPrivacy) and simplified specifically to be better compatible with DNS-level adblocking.<br>
- 57,007 entries.<br>
https://github.com/AdguardTeam/AdguardSDNSFilter
### OISD
Internet's #1 domain blocklist. Blocks Ads, Mobile Ads, Phishing, Malvertising, Malware, Tracking, Telemetry, Cryptojacking, Analyitics, Spyware, Ransomware, Misleading Marketing, etc.
- 221,708 entries. <br>
https://oisd.nl
### AdGuard Extended Mobile Ads Filter
Filter that blocks ads on mobile devices. Contains all known mobile ad networks.
- 851 entries.<br>
https://kb.adguard.com/general/adguard-ad-filters#mobile-ads-filter
### Goodbye Ads
Specifically designed for mobile ad protection.
- 400,655 entries<br>
  https://github.com/jerryn70/GoodbyeAds
### antipopads
List of popads.net domains.
- 755 entries<br>
https://github.com/Yhonay/antipopads
### HaGeZi - Multi ULTIMATE
Ultimate Sweeper - Strictly cleans the Internet and protects your privacy! Blocks Ads, Affiliate, Tracking (+Referral), Metrics, Telemetry, Phishing, Malware, Scam, Free Hoster, Fake, Coins and other Crap.<br>
- 441,998 entries<br>
https://github.com/hagezi/dns-blocklists
### Energized Ultimate
Strictly blocks advertisements, malwares, spams, statistics & trackers on both web browsing and applications. Flagship Protection Pack from Energized Protection.
-  0 entries<br>
https://github.com/EnergizedProtection/block
### hBlock
Improve your security and privacy by blocking ads, tracking and malware domains.
- 440,885 entries<br>
  https://hblock.molinero.dev
# Changes
## v1.0.1
2 November 2023
- Adds "antipopads," "HaGeZi - Multi ULTIMATE," "Energized Ultimate," and "hBlock" to the list of included blocklists.
## v1.0
1 November 2023
- Initial launch
# FAQ
### Should DeltaBlock replace my browser's adblocker extension?
No. While DeltaBlock has a high blocking percentage, DeltaBlock or any DNS-enabled adblocking system is not capable of getting rid of the site elements where an ad would load like uBlock Origin is capable of. In other words, only using DeltaBlock would block ads just fine, but empty spaces would still be present on the page where the ads would originally be.
### Can I use DeltaBlock along with an adblocker extension?
Yes, and we recommend this. See the above question.
### Why Do Some Blocklists say "0 Entries"?
This is most likely because the author of the blocklist forgot to enter a number for NextDNS to report the entry count when they added it. All blocklist information on this page is derived directly from their listing on NextDNS.
### Can I Use DeltaBlock without paying for NextDNS?
Yes, but you'll be limited to 300,000 queries per month, after which the effects of DeltaBlock will stop working until the next month. NextDNS offers unlimited queries starting at $1.99/month.
### Can I Use DeltaBlock With a Different DNS Service?
Direct support for other DNS services is planned in the future, but no official support exists for DeltaBlock on any service other than NextDNS currently. It is possible to utilize the [NextDNS CLI](https://github.com/nextdns/nextdns/wiki) or export the domain list used by DeltaBlock using third party tools to achieve this. We plan to directly provide this list in the future.
### Where Is The Blocking Perecentage Derived From?
All testing for blocking precentage is dervied from the open-source [Toolz Adblock Test](https://d3ward.github.io/toolz/adblock.html). This percentage is directly effected by differing network variables and may be skewed by the adblocker used by your browser along with DeltaBlock. The highest blocking percentage for DeltaBlock based on iOS and macOS devices is up to 99%. DeltaBlock's lowest internal testing percentage is 93%, although you may see lower numbers depending on your network environment.
### Why Should I Use DeltaBlock Instead of a Browser-based Adblocker?
Because DeltaBlock is a DNS service, it blocks ads across every app on your device instead of being confined to just your browser. The greatest use for this is in-app adblocking on iOS and Android devices. We recommend that you use DeltaBlock and a browser-based adblocker (such as uBlock Origin) in tandem with one another to get rid of visual leftovers caused as a result of ads not loading.
### Got another question?
Feel free to reach out to DeltaBlock's developer at [dub.sh/gabe](https://dub.sh/gabe) via the contact form or your preferred social media.
