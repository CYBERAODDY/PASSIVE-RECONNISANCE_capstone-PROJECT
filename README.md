# External Attack Surface Discovery and Reconnaissance (Capstone)

Cybersecurity capstone project. We acted as a junior penetration-testing team and started with reconnaissance.

- **Passive recon target:** example.com
- **Active recon target:** Metasploitable2 lab VM (private lab network only)
- **Status:** passive phase complete; active phase, attack surface diagram and checklist sign-off still in progress

## What is in this repository

| Folder | Contents |
|---|---|
| `report/` | The reconnaissance report (PDF) |
| `evidence/` | Screenshots of every command and result. File names match the appendix labels (A-1, A-2, ...) in the report |
| `commands/` | A list of every command we ran |

## Scope

Only example.com (passive) and the instructor-approved lab network (active) were in scope. No other domain, IP address or network was scanned or probed. Hostnames and IPs that appeared in third-party search results were treated as unverified data and were not contacted.

## Tools used

whois, dig, nslookup, theHarvester, whatweb, and (for the active phase) Nmap.

## Key findings (passive phase)

- example.com is an IANA-reserved domain with no registrant details exposed.
- DNS and web traffic are served through Cloudflare. ARIN confirms 104.20.23.154 belongs to Cloudflare, Inc.
- The domain publishes a null MX record and an SPF `-all` policy, so it is set up to send and receive no email.
- Three registry locks and DNSSEC are enabled.
- theHarvester returned nothing from one source and many unverified hostnames from all sources. These are treated as likely noise until checked.
- No vulnerabilities were identified.

## Notes

- Findings are labelled as confirmed facts or assumptions in the report.
- AI assistance: [state here how AI was used, if your course requires a disclosure.]

## Team

TANIMOLA AYOMIDE ERIC
