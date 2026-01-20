 **SentinelScope – Automated OSINT Reconnaissance Framework**

SentinelScope is a modular, Python-powered OSINT (Open Source Intelligence) framework designed to streamline the process of gathering publicly available information from multiple sources.  
It is built for cybersecurity professionals, penetration testers, and researchers who require fast, structured, and reproducible reconnaissance.

---

 Key Capabilities

- GitHub Recon – Extract public profile data, starred repositories, and organizational memberships.
- Phone Number OSINT – Identify country and carrier details from phone numbers.
- WHOIS Lookup – Retrieve domain registration data, name servers, and status.
- Subdomain Enumeration – Discover subdomains from multiple public intelligence sources.
- LinkedIn Search Automation – Perform targeted Google dorking for LinkedIn profiles.
- Unified "Run All" Mode – Execute all modules in a single workflow with consistent output formatting.

---

 Project Layout

`
SentinelScope/
│
├── sentinelscope_main.py          # Main menu and execution flow
├── ghprofilescan.py              # GitHub profile reconnaissance
├── phoneosintlookup.py           # Phone number OSINT
├── domainwhoislookup.py          # WHOIS domain lookup
├── subdomain_mapper.py             # Subdomain enumeration
├── linkedinprofilesearch.py      # LinkedIn profile search
├── sentinelscope_config.py         # API tokens and configuration
├── requirements.txt                # Python dependencies
└── output/                         # Generated reports
`

---

 Installation

Clone the repository and install dependencies:

`bash
git clone https://github.com/frangelbarrera/sentinelscope.git
cd sentinelscope
pip install -r requirements.txt
`

> Note: For GitHub Recon, set your personal access token in sentinelscope_config.py to avoid API rate limits.

---

 Usage

Run the toolkit:

`bash
python sentinelscope_main.py
`

Select a module from the menu or choose Run All to execute the full reconnaissance workflow.

---

 Example Output

GitHub Recon:
`
Username: torvalds
Name: Linus Torvalds
Public Repos: 8
Followers: 246,000+
Organizations: Linux Foundation
`

Phone Number OSINT:
`
Phone Number: +1 2025550123
Country: Washington D.C.
Carrier: Unknown
`

---

 Disclaimer

This tool is intended for educational and authorized security testing purposes only.  
The author is not responsible for any misuse or damage caused by this software.

---

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
