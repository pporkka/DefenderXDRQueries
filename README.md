# DefenderXDRQueries
Repository for generically useful KQL Queries for threat hunting for Microsoft DefenderXDR

## IOC Queries
Queries using external feed sources to query.

### Rösti IOCs Feed KQL

Rosti-IOCs-feed.kql - using https://rosti.bin.re/feeds/mde-all to find interesting events. Note this may produce huge amount of results. You may want to change the feed to one of the other more restricted types found here: https://rosti.bin.re/feeds (look at the bottom of the page for Defender for Endpoint iocs)

## Vulnerability data

Queries for existing vulnerabilities (unpatched) in devices from Defender XDR data

### EPSS-enriched-XDR-device-vulnerability-data.kql

This uses Exploit Prediction Scoring System (EPSS) to enrich vulnerability data found in devices (from Defender for Endpoint).

The idea is to find vulnerabilities that are likely to be exploited or have already been exploited if EPSS is high enough.



