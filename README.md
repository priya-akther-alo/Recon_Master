# Recon_Master

A comprehensive cybersecurity reconnaissance tool for subdomain enumeration, live host detection, port scanning, vulnerability scanning, malware scanning, and DNS enumeration. Ideal for security researchers and penetration testers.

## Features
- **Subdomain Enumeration**: Uses `amass`, `subfinder`, `theHarvester`, and `dnsrecon`.
- **Live Host Detection**: Identifies active hosts using `httpx`.
- **Port Scanning**: Scans open ports and services with `nmap`.
- **Vulnerability Scanning**: Detects vulnerabilities using `nuclei`.
- **Malware Scanning**: Identifies potential malware indicators in web content.
- **DNS Enumeration**: Gathers DNS records (SOA, NS, MX, TXT, SRV) with `dnsrecon`.
- **JSON and HTML Reports**: Generates professional reports for clients.
- **Email Notifications**: Sends scan results to specified email addresses.
- **Caching**: Reuses previous scan results to save time.

## Installation
1. Install dependencies:
   ```bash
   sudo apt install nmap dnsrecon curl mailutils jq
   go install -v github.com/projectdiscovery/httpx/cmd/httpx@latest
   go install -v github.com/projectdiscovery/nuclei/v2/cmd/nuclei@latest
   go install -v github.com/OWASP/Amass/v3/...@master
   go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
   sudo apt install theharvester


