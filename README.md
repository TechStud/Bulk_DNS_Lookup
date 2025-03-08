# Bulk_DNS_Lookup v2

A simple bash script that generates a CSV of DNS lookups from a list of domains.  

The original bash script from @LTS_Tom _(see details below)_ has been heavily modified.  
- added script timer **(Duration: 0 days 00 hrs 00 mins 00 secs)**.
- added progress bar: Progress : **[####################################### ]  99% [99/100] -- Resolving: \<domainname\>**
- added detail about **ZoneFiles Compromised domain list** in the script comments.
- added all popular DNS Resolvers from **Cloudflare, Quad9, AdGuard DNS** and a **NextDNS** (Let's test them ALL! - 10 in total)
- added additional functionality to dns query commands to simplify the output _(see example below)_.
- added a Detailed Summary output to console upon running the script. This ensures 
     anyone running it doesn't need to read the source script to understand what's going on.
- NOTE: This script has no command-line arguments or inputs. All configurations must be made within this file alone.

---

_Original v1 of 'Bulk_DNS_Lookup'  
Original Author     : LTS_Tom  
Original Source     : https://forums.lawrencesystems.com/t/which-is-the-best-dns-for-secure-browsing-cloudflare-quad9-nextdns-and-adguard-dns-youtube-release/18910/2  
Original Forum Title: Which Is The Best DNS for Secure Browsing: CloudFlare, Quad9, NextDNS, and AdGuard DNS [YouTube Release]  
      -  Identify which DNS Services are the Best for Filtering Malicious Sites/Domains...  
      -  DNS services tested: Cloudflare, Quad9, AdGuard DNS and NextDNS using a Malicious/Compromised Domains list._  

---
# Usage

1. Save this file locally.
2. Open the file in text editor _(eg: vi, nano...)_
3. Review the file and settings
4. Edit the '**domain_list=**' parameter, to point to the file you want to read from. _(I used the Zonefiles ~20k domain list which are actively compromised as a test)_
5. Save the file.
6. Execute the script
  ```$ sh ./bulk_dns_lookup.sh```
7. Once complete, you should be able to use Excel or equivilant editor to review the contents of the CSV output file.


