# DefenderXDRQueries
Repository for generically useful KQL Queries for threat hunting for Microsoft DefenderXDR

## IOC Queries
Queries using external feed sources to query.

## Notepad-plus-plus installer detection  
Sentinel query, to span june 2025 onwardrs. https://github.com/pporkka/DefenderXDRQueries/blob/main/KQL_HuntForNotepadPlusPlus_installers.kql query to detect known external list of pre 8.9.1 npp installer hashes. 

### Rösti IOCs Feed KQL

Rosti-IOCs-feed.kql - using https://rosti.bin.re/feeds/mde-all to find interesting events. Note this may produce huge amount of results. You may want to change the feed to one of the other more restricted types found here: https://rosti.bin.re/feeds (look at the bottom of the page for Defender for Endpoint iocs)

### KQL_SuspiciousChromeExtensions.kql
Query to get a list (my list, others exist in which case you can use this as an example) and verify your environment endpoints against the known malicious (or suspicious) chrome extensions. Please, see https://github.com/pporkka/MaliciousChromeExt

## Vulnerability data

Queries for existing vulnerabilities (unpatched) in devices from Defender XDR data

### EPSS-enriched-XDR-device-vulnerability-data.kql

This uses Exploit Prediction Scoring System (EPSS) to enrich vulnerability data found in devices (from Defender for Endpoint).

The idea is to find vulnerabilities that are likely to be exploited or have already been exploited if EPSS is high enough.



