# Commands run (passive phase)

All commands were run from a Kali Linux 2026.1 VM (VirtualBox). Target: **example.com** only.

## Domain registration
```
whois example.com
whois 104.20.23.154
```

## DNS
```
dig example.com A
dig example.com AAAA
dig example.com MX
dig example.com NS
dig example.com TXT
nslookup example.com
nslookup -type=AAAA example.com
nslookup -type=MX example.com
nslookup -type=NS example.com
nslookup -type=TXT example.com
nslookup -type=A example.com
```

## Emails and subdomains
```
theHarvester -d example.com -b duckduckgo
theHarvester -d example.com -b all
```

## Web technology
```
whatweb example.com
whatweb https://example.com
```

## Planned for the active phase (lab only)
```
nmap -sn <lab-subnet>/24
nmap -sV <metasploitable2-ip>
```
