# Awesome Cypherpunk [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of open-source digital self-defense tools, operational security guides, self-hosted sovereign infrastructure, OSINT toolkits, and freedom bandwidth resources maintained by the **[Cypherpunk Society](https://cypherpunksociety.org)** at Frontier Tower, San Francisco.

---

## Contents

- [1. Foundational Digital Hygiene (Start Here)](#1-foundational-digital-hygiene-start-here)
- [2. Surveillance Self-Defense & Threat Modeling](#2-surveillance-self-defense--threat-modeling)
- [3. Hardened Operating Systems & Endpoint Security](#3-hardened-operating-systems--endpoint-security)
- [4. Self-Hosting & Sovereign Cloud Replacements](#4-self-hosting--sovereign-cloud-replacements)
- [5. Encrypted & Decentralized Communications](#5-encrypted--decentralized-communications)
- [6. Freedom Bandwidth, Tor & Censorship Circumvention](#6-freedom-bandwidth-tor--censorship-circumvention)
- [7. Counter-Surveillance & Spyware Forensics](#7-counter-surveillance--spyware-forensics)
- [8. Open-Source Intelligence (OSINT) & Public-Interest Data](#8-open-source-intelligence-osint--public-interest-data)
- [9. Aaron Swartz Open-Source Legacy Projects](#9-aaron-swartz-open-source-legacy-projects)
- [10. Classic Cypherpunk Texts & Archives](#10-classic-cypherpunk-texts--archives)

---

## 1. Foundational Digital Hygiene (Start Here)

- **[Andrej Karpathy's *Digital Hygiene*](https://karpathy.bearblog.dev/digital-hygiene/)** — Practical baseline checklist for everyday personal security: password managers, hardware FIDO2/U2F keys (`YubiKey`), DNS filtering (`NextDNS` / `Pi-hole`), `Signal`, `Brave`, virtual credit cards (`Privacy.com`), `Mullvad VPN`, application firewall monitoring (`Little Snitch`), full-disk encryption, work/personal device separation, and avoiding IoT telemetry.
- **[Privacy Guides](https://www.privacyguides.org/)** — Community-audited recommendations for privacy-respecting browsers, email providers, DNS resolvers, and mobile/desktop hardening (successor to PrivacyTools).
- **[Consumer Reports Security Planner](https://securityplanner.consumerreports.org/)** — Customized step-by-step action plans for securing phones, laptops, and accounts.

## 2. Surveillance Self-Defense & Threat Modeling

- **[EFF Surveillance Self-Defense (SSD)](https://ssd.eff.org/)** — The Electronic Frontier Foundation's flagship curriculum on threat modeling, encryption, border-crossing device hygiene, and protest OpSec.
- **[Access Now Digital Security Helpline](https://www.accessnow.org/help/)** — 24/7 rapid-response digital security assistance and training resources for civil society, journalists, and activists.
- **[Library Freedom Project](https://libraryfreedom.org/)** — Slide decks, zines, and train-the-trainer curricula for teaching privacy and Tor in public spaces.
- **[The Hitchhiker's Guide to Online Anonymity](https://anonymousplanet.org/)** — Deep technical handbook on compartmentalization, pseudonymous identities, and network-level operational security.
- **[Autodéfense Numérique (Paris)](https://guide.boum.org/)** — Classic French digital self-defense manual born out of Parisian hackerspaces and La Quadrature du Net workshops.

## 3. Hardened Operating Systems & Endpoint Security

- **[Tails OS](https://tails.net/)** — Amnesic live operating system booted from a verified USB stick that routes all traffic through Tor and leaves zero trace on the host machine.
- **[Qubes OS](https://www.qubes-os.org/)** — "A reasonably secure operating system" using Xen-based virtualization to compartmentalize work, personal, Whonix/Tor, and untrusted disposable VMs.
- **[GrapheneOS](https://grapheneos.org/)** — Hardened, privacy- and security-focused mobile OS for Pixel devices with sandboxed Google Play, per-app network toggles, and exploit mitigations.
- **[Whonix](https://www.whonix.org/)** — Two-VM anonymity OS architecture (Gateway + Workstation) that prevents IP/DNS leaks even if the workstation is compromised.
- **[Objective-See (macOS Open-Source Security)](https://objective-see.org/tools.html)** — Patrick Wardle's free, open-source macOS security suite:
  - **[LuLu](https://objective-see.org/products/lulu.html)** — Open-source macOS outbound firewall (free alternative to Little Snitch).
  - **[OverSight](https://objective-see.org/products/oversight.html)** — Alerts whenever the internal microphone or webcam is activated.
  - **[KnockKnock](https://objective-see.org/products/knockknock.html)** & **[BlockBlock](https://objective-see.org/products/blockblock.html)** — Persistence detection and monitoring.
- **[OpenSnitch](https://github.com/evilsocket/opensnitch)** — GNU/Linux interactive application firewall inspired by Little Snitch.

## 4. Self-Hosting & Sovereign Cloud Replacements

*Open-source, self-hostable alternatives to the commercial cloud stack:*

- **[Awesome-Selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted)** & **[selfh.st](https://selfh.st/)** — Comprehensive directories of software you can host on your own hardware or VPS.
- **Passwords & Keys:**
  - **[Vaultwarden](https://github.com/dani-garcia/vaultwarden)** — Lightweight, Rust-based self-hosted Bitwarden server.
  - **[KeePassXC](https://keepassxc.org/)** — Offline, cross-platform password manager with YubiKey challenge-response support.
- **DNS & Network Filtering:**
  - **[Pi-hole](https://pi-hole.net/)** & **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** — Self-hosted network-wide DNS sinkholes (pair with **[Unbound](https://nlnetlabs.nl/projects/unbound/about/)** for recursive DNS resolution).
  - **[NextDNS](https://nextdns.io/)** — Managed encrypted DNS firewall for mobile/roaming devices.
- **Mesh VPN & Zero-Trust Networking:**
  - **[WireGuard](https://www.wireguard.com/)** — Fast, modern kernel-level VPN tunnel.
  - **[Headscale](https://github.com/juanfont/headscale)** — Open-source, self-hosted implementation of the Tailscale control server.
  - **[Mullvad VPN](https://mullvad.net/)** — Account-number-only VPN accepting cash and Monero, with audited RAM-only WireGuard servers.
- **Files, Collaboration & Photos:**
  - **[Syncthing](https://syncthing.net/)** — Continuous, decentralized peer-to-peer file synchronization with no central server.
  - **[CryptPad](https://cryptpad.org/)** — End-to-end encrypted, zero-knowledge collaborative docs, sheets, and kanban boards.
  - **[Nextcloud](https://nextcloud.com/)** — Self-hosted file suite, calendar (`CalDAV`), and contacts (`CardDAV`).
  - **[Immich](https://immich.app/)** — High-performance self-hosted photo and video backup (on-device ML search).
- **Local AI (Zero Cloud Telemetry):**
  - **[llama.cpp](https://github.com/ggml-org/llama.cpp)** & **[Ollama](https://ollama.com/)** — Run open-weight LLMs and embeddings locally on Apple Silicon or Linux GPUs.

## 5. Encrypted & Decentralized Communications

- **[Signal](https://signal.org/)** — Gold-standard end-to-end encrypted messaging and calls (`Signal Protocol` / `PQXDH` post-quantum handshake).
- **[Matrix](https://matrix.org/)** & **[Element](https://element.io/)** — Open standard for federated, end-to-end encrypted (`Megolm`) real-time chat and Spaces (used by Fedora, Mozilla, Tor, and GrapheneOS; join [`#cypherpunksociety:matrix.org`](https://matrix.to/#/#cypherpunksociety:matrix.org)).
- **[Jitsi Meet](https://jitsi.org/)** — Open-source, WebRTC-based encrypted video conferencing (`meet.jit.si` or self-hosted).
- **[Briar](https://briarproject.org/)** & **[Cwtch](https://cwtch.im/)** — Peer-to-peer, metadata-resistant messaging routed over Tor Onion Services (Briar also syncs over Bluetooth/Wi-Fi mesh during internet blackouts).
- **[SimpleX Chat](https://simplex.chat/)** — Messaging network with zero user identifiers (not even random numbers), using unidirectional queues.
- **[OnionShare](https://onionshare.org/)** — Open-source tool to securely and anonymously share files, host static websites, and chat over Tor Onion Services directly from your laptop.
- **[Bluesky (AT Protocol)](https://bsky.app/)** & **[Mastodon (ActivityPub)](https://joinmastodon.org/)** — Open-protocol social networks with domain-based identity (`@cypherpunksociety.org`).

## 6. Freedom Bandwidth, Tor & Censorship Circumvention

- **[The Tor Project](https://www.torproject.org/)** — Anonymity network and onion routing ecosystem.
- **[Tor Snowflake](https://snowflake.torproject.org/)** — Ephemeral WebRTC browser/standalone proxy that lets anyone donate bandwidth to help censored users reach Tor safely from coworking or home Wi-Fi.
- **[Tor Relay Guide (`community.torproject.org/relay`)](https://community.torproject.org/relay/)** — Official runbooks for operating obfs4 Pluggable Transport bridges, middle/guard relays, and exit nodes.
- **[Emerald Onion](https://emeraldonion.org/)** — US West Coast 501(c)(3) non-profit transit provider and high-capacity Tor exit operator peering in the Bay Area (Fremont Cabal IX) and Seattle.
- **[Nos Oignons](https://nos-oignons.net/)** — French sister non-profit operating community-funded Tor exit nodes alongside **[La Quadrature du Net](https://www.laquadrature.net/)**.
- **[The Calyx Institute](https://calyxinstitute.org/)** — Non-profit privacy educator, Tor relay sponsor, and developer of CalyxOS.

## 7. Counter-Surveillance, Censorship Measurement & Cognitive Security

### The Citizen Lab, Amnesty Tech & Spyware Forensics
- **[The Citizen Lab (UofT Munk School)](https://citizenlab.ca/)** — Interdisciplinary laboratory investigating commercial spyware (Pegasus, Predator, Candiru), transnational repression, and network censorship ([Events & Seminars](https://munkschool.utoronto.ca/events) · [Citizen Lab Summer Institute](https://citizenlab.ca/summerinstitute/)).
- **[Citizen Lab Open-Source Repositories (`github.com/citizenlab`)](https://github.com/citizenlab):**
  - **[`citizenlab/test-lists`](https://github.com/citizenlab/test-lists)** — Community-curated URL testing lists for 200+ countries used by OONI and Censored Planet to detect website blocking.
  - **[`citizenlab/malware-indicators`](https://github.com/citizenlab/malware-indicators)** & **[`citizenlab/malware-signatures`](https://github.com/citizenlab/malware-signatures)** — Open-source YARA rules and IoCs from targeted spyware investigations.
  - **[`citizenlab/chat-censorship`](https://github.com/citizenlab/chat-censorship)** — Data and methodology for measuring automated keyword and image filtering in chat apps.
- **[Amnesty International Security Lab (`github.com/AmnestyTech`)](https://github.com/AmnestyTech)** — Co-investigators on the Pegasus Project; maintains **[`AmnestyTech/investigations`](https://github.com/AmnestyTech/investigations)** (spyware IoCs) and **[Mobile Verification Toolkit (`mvt-project/mvt`)](https://github.com/mvt-project/mvt)** to inspect iOS and Android backups for mercenary spyware traces.

### Global Network Censorship Measurement
- **[OONI — Open Observatory of Network Interference (`ooni.org`)](https://ooni.org/)** ([`github.com/ooni`](https://github.com/ooni)) — Spun out of the Tor Project; anyone can run the open-source **OONI Probe** app to test network blocking/throttling and publish real-time measurements to **[OONI Explorer (`explorer.ooni.org`)](https://explorer.ooni.org/)**.
- **[Censored Planet (University of Michigan)](https://censoredplanet.org/)** — Global remote measurement platform tracking DNS manipulation, TLS middleboxes, and national firewalls.

### Field Counter-Surveillance & Physical Security
- **[EFF Rayhunter](https://github.com/EFForg/rayhunter)** — Open-source Rust tool by EFF that runs on a $20 Orbic mobile hotspot to detect cell-site simulators (IMSI catchers / Stingrays) in the field.
- **[EFF Atlas of Surveillance](https://atlasofsurveillance.org/)** — Crowdsourced database documenting police surveillance tech (ALPRs, facial recognition, drones, Ring partnerships, real-time crime centers).
- **[DeFlock](https://deflock.me/)** — OpenStreetMap-powered community project mapping Automated License Plate Readers (ALPRs).
- **[Precursor / Betrusted (`betrusted.io`)](https://betrusted.io/)** — Bunnie Huang & Xobs's open-hardware, FPGA-verifiable RISC-V handheld device built for high-assurance cryptographic verification.

### Stanford Cyber Policy Center, SIO & Cognitive Security
- **[Stanford Cognitive Security Task Force](https://hai.stanford.edu/)** & **[Stanford Cyber Policy Center](https://cyber.fsi.stanford.edu/)** — Research on AI-driven persuasion, information integrity, cognitive resilience, and neural/BCI data privacy.
- **[Open-Source *Trust and Safety* Curriculum (`tsbook.org`)](https://tsbook.org/)** ([`TeachingTrustSafety` on GitHub](https://github.com/trust-safety-teaching-consortium/TeachingTrustSafety)) — Full open-source textbook, lecture slides, and bot-building labs developed from Stanford's *CS 152: Trust and Safety Engineering*.
- **[`stanfordio/skyfall`](https://github.com/stanfordio/skyfall)** — Open-source Bluesky AT Protocol firehose ingestion tool built at the Stanford Internet Observatory for studying decentralized social graphs in real time.
- **[Journal of Online Trust and Safety (`tsjournal.org`)](https://tsjournal.org/)** — Open-access peer-reviewed research on platform manipulation and information security.
- **[Chaos Computer Club (CCC) Media Archive (`media.ccc.de`)](https://media.ccc.de/)** — Decades of technical lectures on hardware hacking, cryptography, biometrics, and civic infrastructure from Chaos Communication Congress.

## 8. Open-Source Intelligence (OSINT) & Public-Interest Data

### Bellingcat Open-Source Tools & Interactive Training
- **[Bellingcat Online Investigation Toolkit](https://bellingcat-toolkit.pages.dev/)** ([`github.com/bellingcat/toolkit`](https://github.com/bellingcat/toolkit)) — Searchable, community-maintained directory of satellite imagery, geolocation, maritime/aviation tracking, and social-media verification tools.
- **[Bellingcat Open Source Challenge (`challenge.bellingcat.com`)](https://challenge.bellingcat.com/)** — Free interactive CTF platform with 100+ hands-on geolocation, chronolocation, satellite, and maritime OSINT puzzles ideal for group workshops.
- **[Bellingcat Open-Source Research Notebooks](https://github.com/bellingcat/open-source-research-notebooks)** — Ready-to-run Jupyter / Google Colab notebooks teaching command-line and Python OSINT tools with zero local setup.
- **[Bellingcat Workshops (`bellingcat.com/workshops`)](https://www.bellingcat.com/workshops)** & **[Biweekly Thursday Discord Stage Talks](https://discord.gg/bellingcat)** — Live OSINT masterclasses and community walkthroughs.
- **Core Open-Source Repositories at [`github.com/bellingcat`](https://github.com/bellingcat):**
  - **[`auto-archiver`](https://github.com/bellingcat/auto-archiver)** — Automatically archive, hash, and screenshot social media posts, videos, and web pages from spreadsheets before they are taken down.
  - **[`osm-search`](https://osm-search.bellingcat.com/)** ([`github.com/bellingcat/osm-search`](https://github.com/bellingcat/osm-search)) — Visual proximity search over OpenStreetMap landmarks for photo/video geolocation without writing Overpass QL.
  - **[`ShadowFinder`](https://github.com/bellingcat/ShadowFinder)** — Calculates possible global coordinates of an image from object height, shadow length, and timestamp.
  - **[`sar-interference-tracker`](https://github.com/bellingcat/sar-interference-tracker)** — Google Earth Engine tool detecting military GPS/radar interference in Sentinel-1 SAR satellite imagery.
  - **[`wayback-google-analytics`](https://github.com/bellingcat/wayback-google-analytics)** — Links networks of websites by scraping historical Google Analytics IDs across the Wayback Machine.
  - **[`EDGAR`](https://github.com/bellingcat/EDGAR)** — Toolkit for investigating corporate and financial SEC filings.
  - **[`octosuite`](https://github.com/bellingcat/octosuite)** & **[`telegram-phone-number-checker`](https://github.com/bellingcat/telegram-phone-number-checker)** — CLI tools for GitHub and Telegram OSINT.
- **Third-Party Open-Source Tools Recommended by Bellingcat:**
  - **[QGIS](https://qgis.org/)** (open-source desktop GIS), **[Overpass Turbo](https://overpass-turbo.eu/)** (OSM query mining), **[ExifTool](https://exiftool.org/)**, **[InVID / WeVerify](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/)** (video keyframe & reverse-image verification), **[yt-dlp](https://github.com/yt-dlp/yt-dlp)**, **[ArchiveBox](https://archivebox.io/)**, and **[Whisper.cpp](https://github.com/ggml-org/whisper.cpp)**.

### Cross-Border, Legal OSINT & Public-Interest Databases
- **[UC Berkeley Human Rights Center Investigation Lab](https://humanrights.berkeley.edu/)** & **[The Berkeley Protocol on Digital Open Source Investigations](https://www.ohchr.org/en/publications/policy-and-methodological-publications/berkeley-protocol-digital-open-source)** — Co-published with the UN OHCHR; the global legal standard for verifying, chain-of-custody archiving, and presenting open-source digital evidence in court.
- **[Micah Lee's *Hacks, Leaks, and Revelations* (`hacksleaks.com`)](https://hacksleaks.com/)** — Free, open-access hands-on textbook teaching investigative data analysis with Python, SQL, Docker, and OCCRP Aleph on real leaked datasets.
- **[Distributed Denial of Secrets (`ddosecrets.com`)](https://ddosecrets.com/)** — Non-profit whistleblower and public-interest leak archive (501(c)(3)) indexing terabytes of searchable corporate and government datasets.
- **[MuckRock (`muckrock.com`)](https://www.muckrock.com/)** & **[DocumentCloud (`documentcloud.org`)](https://www.documentcloud.org/)** ([`github.com/MuckRock`](https://github.com/MuckRock)) — Open-source Freedom of Information Act (FOIA) request automation and collaborative document analysis suite.
- **[OCCRP Aleph](https://aleph.occrp.org/)** ([`github.com/alephdata/aleph`](https://github.com/alephdata/aleph)) — Open-source investigative data platform indexing company registries, leaked archives, sanctions lists, and court filings for cross-border journalism.
- **[ProPublica Open-Source & Data Tools](https://github.com/propublica)** —
  - **[Nonprofit Explorer & API](https://projects.propublica.org/nonprofits/)** — Searchable database of millions of IRS Form 990 filings.
  - **[`IRSx` (`990-xml-reader`)](https://github.com/propublica/990-xml-reader)** — Python library converting raw IRS 990 XML filings into structured JSON/objects.
  - **[ProPublica Events & Webinars](https://www.propublica.org/events)** — Walkthroughs of investigative methodologies and public datasets.

## 9. Aaron Swartz Open-Source Legacy Projects

*Active open-source projects founded or inspired by Aaron Swartz (`1986–2013`), featured at the annual November **[Aaron Swartz Day & International Hackathon](https://www.aaronswartzday.org/)** at the Internet Archive:*

- **[SecureDrop](https://securedrop.org/)** ([`github.com/freedomofpress/securedrop`](https://github.com/freedomofpress/securedrop)) — *Status: Active & Mature.* Originally coded by Aaron Swartz as *DeadDrop* with Kevin Poulsen and James Dolan; now maintained by the **[Freedom of the Press Foundation](https://freedom.press/)** and used by 70+ major newsrooms (including [ProPublica](https://www.propublica.org/tips/)). Includes **[SecureDrop Workstation](https://github.com/freedomofpress/securedrop-workstation)** built on Qubes OS.
- **[Open Library](https://openlibrary.org/)** ([`github.com/internetarchive/openlibrary`](https://github.com/internetarchive/openlibrary)) — *Status: Active.* Co-created by Aaron Swartz at the **[Internet Archive](https://archive.org/)** as an open, editable catalog for every book ever published (`AGPLv3`). Welcomes developer and data-librarian PRs year-round.
- **[`html2text`](https://github.com/Alir3z4/html2text)** (originally [`aaronsw/html2text`](https://github.com/aaronsw/html2text)) — *Status: Active.* Aaron's Python script converting HTML pages into clean Markdown text; now a foundational building block in modern open-source web-scraping and LLM pipelines.
- **[`web.py`](https://webpy.org/)** ([`github.com/webpy/webpy`](https://github.com/webpy/webpy)) — *Status: Maintained (Python 3).* Minimalist, anti-magic Python web framework created by Aaron Swartz.
- **[Tor2web](https://github.com/globaleaks/Tor2web)** — *Status: Maintained by GlobaLeaks/Hermes Center.* Co-created by Aaron Swartz and Virgil Griffith in 2008 to allow whistleblowers without Tor Browser to reach `.onion` dropboxes.
- **[Aaron Swartz Memorial Archive (`github.com/aaronsw`)](https://github.com/aaronsw)** & **[Raw Thought Blog Archive (`aaronsw.com/weblog`)](http://www.aaronsw.com/weblog/)** — Preserved code and essays.

## 10. Classic Cypherpunk Texts & Archives

- **[A Cypherpunk's Manifesto — Eric Hughes (March 9, 1993)](https://www.activism.net/cypherpunk/manifesto.html)** — *"Privacy is necessary for an open society in the electronic age... Cypherpunks write code."*
- **[The Crypto Anarchist Manifesto — Timothy C. May (1988/1992)](https://www.activism.net/cypherpunk/crypto-anarchy.html)**
- **[Why I Wrote PGP — Phil Zimmermann (1991)](https://www.philzimmermann.com/EN/essays/WhyIWrotePGP.html)**
- **[A Declaration of the Independence of Cyberspace — John Perry Barlow (1996)](https://www.eff.org/cyberspace-independence)**
- **[Guerilla Open Access Manifesto — Aaron Swartz (2008)](https://archive.org/details/GuerillaOpenAccessManifesto)**
- **[Cypherpunks Mailing List Archive (1992–1998)](https://cypherpunks.venona.com/)** — Historical archive of the original `cypherpunks@toad.com` list hosted by John Gilmore in San Francisco.

---

## Contributing

Contributions are welcome! Open a pull request or bring a tool to our weekly Thursday clinic (4:00–5:30 PM) at Frontier Tower, San Francisco.
