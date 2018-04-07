# FacebookCyberSecurityCourseWeek9
Honeypot implementations and analysis.

Honeypots deployed using google cloud compute instances.

Mapping:

mhn-honeypot-1 (2,789 attacks) - Dionaea
mhn-honeypot-2 (7,859 attacks) - Amun
mhn-honeypot-3 (885 attacks) - Snort 
mhn-honeypot-4 (0 attacks) - Shockpot
mhn-honeypot-5 (3,793 attacks) - Suricata

TOP 5 Attacks Signatures:
ET DROP Dshield Block Listed Source group 1 (297 times)
ET CINS Active Threat Intelligence Poor Reputation IP TCP group 4 (100 times)
ET SCAN Suspicious inbound to MSSQL port 1433 (96 times)
ET CINS Active Threat Intelligence Poor Reputation IP TCP group 65 (68 times)
ET SCAN Suspicious inbound to mySQL port 3306 (43 times)

TOP 5 Attacked ports:
445 (4,670 times)
80 (3,277 times)
3389 (3,151 times)
5060 (828 times)
23 (370 times)

TOP 5 Attacker IPs:
10.128.0.7 (3,094 attacks)
50.76.179.69 (2,787 attacks)
5.62.39.237 (568 attacks)
77.72.82.72 (191 attacks)
182.74.214.226 (160 attacks)

Attacks in the last 24 hours of test (4/5/18 - 4/6/18):
15,339

Notes:
mhn-honeypot-3 (Snort) needed -Pn argument for nmap utility to function against server.
mhn-honeypot-4 (Shockpot) did not function as expected (no attacks detected). Upon search engine research, server may have needed to be rebooted, and Shockpot deploy script needed to be re-ran (https://github.com/threatstream/shockpot/issues/4)
