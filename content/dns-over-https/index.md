---
title: "DNS over HTTPS service"
date: 2018-04-10
tags: []
draft: false
---

# DNS over HTTPS service

We operate experimental DNS over HTTPS service at:

<div style="font-size: 150%; margin-top: 1em; margin-bottom: 1em; text-align: center">https://dns.dns-over-https.com/dns-query</div>

We recommend using [m13253/dns-over-https](https://github.com/m13253/dns-over-https) to access our service. [Other compatible clients](https://github.com/curl/curl/wiki/DNS-over-HTTPS) are also supported.

DNS over HTTPS enhances your online security and privacy. Also it prevents possible DNS poisoning deployed by your ISP or company.

## Notes

- We might shut down our service at any time -- probably because we run out of our pocket money.
- We reserve the rights to prevent abuse of our services, including but not limited to: occupying large amount of computing resources, initiating cyberattacks, conducting illegal penetration tests.
- We regularly keep access logs to monitor service health, and periodically clear them every day.
- To protect privacy, we do recursive queries with DNSSEC check by ourselves without relying on other public DNS resolvers. **That would be much slower, you have been warned.**
- Your IP prefix (/24 for IPv4, /48 for IPv6) is used for retrieving GeoDNS-related results. For doh-client, you may use no\_ecs to opt out.
- Some domains (especially those hosted on Alibaba DNS) fail to resolve due to connectivity problems. Write to us if it happens. We will forward related quries to Google or CloudFlare's resolvers.

## Contact

Feel free to write to the "dns" mailbox of "dns-over-https.com" in case of anything you want to tell us.
