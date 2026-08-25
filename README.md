<div align="center">
  <img src="image/auroria_link_256.png" alt="Axovox Logo" width="150"/>
  <h1>Axovox</h1>
  <p><strong>Encrypted team messaging on your own server. Like Discord, but self-hosted — no middleman.</strong></p>
  
  <p>
    <img src="https://img.shields.io/badge/status-beta-blue?style=for-the-badge" alt="Project Status: Beta"/>
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Version-0.14.1%20(46)-blueviolet?style=flat-square&logo=github" alt="Version"/>
    <img src="https://img.shields.io/badge/Release%20Date-2026--08--21-blue?style=flat-square&logo=calendar" alt="Release Date"/>
  </p>

  <p align="center">
    <a href="#-version-française"><img src="https://img.shields.io/badge/_-Lire_en_français-EF4135?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMCIgaGVpZ2h0PSIyMCI%2BPHJlY3Qgd2lkdGg9IjEwIiBoZWlnaHQ9IjIwIiBmaWxsPSIjMDA1NUE0Ii8%2BPHJlY3QgeD0iMTAiIHdpZHRoPSIxMCIgaGVpZ2h0PSIyMCIgZmlsbD0iI2ZmZmZmZiIvPjxyZWN0IHg9IjIwIiB3aWR0aD0iMTAiIGhlaWdodD0iMjAiIGZpbGw9IiNFRjQxMzUiLz48L3N2Zz4=" alt="Lire en français"/></a>
  </p>
</div>

---

## 🚀 Get the Latest Version

> **Note**: Axovox builds are downloaded from the releases below. The installation procedure is identical to Axomind's — follow the guide for your platform.

<div align="center">
  <table>
    <tr>
      <td align="center" width="33%">
        <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_ANDROID.md">
          <img src="https://img.shields.io/badge/Android-Install-2E7D32?style=for-the-badge&logo=android&logoColor=white" alt="Install for Android"/>
        </a>
        <br/>
        <sub>APK • <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_ANDROID.md">Installation guide</a></sub>
      </td>
      <td align="center" width="33%">
        <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_WINDOWS.md">
          <img src="https://img.shields.io/badge/Windows-Install-3A6DF0?style=for-the-badge&logo=windows11&logoColor=white" alt="Install for Windows"/>
        </a>
        <br/>
        <sub>ZIP • <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_WINDOWS.md">Installation guide</a></sub>
      </td>
      <td align="center" width="33%">
        <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_LINUX.md">
          <img src="https://img.shields.io/badge/Linux-Install-8A6DF0?style=for-the-badge&logo=linux&logoColor=white" alt="Install for Linux"/>
        </a>
        <br/>
        <sub>Debian 13 • <a href="https://github.com/Sebastien-VZN/axomind/blob/main/INSTALL_LINUX.md">Installation guide</a></sub>
      </td>
    </tr>
  </table>
</div>

<p align="center">
  <a href="https://github.com/Sebastien-VZN/axovox/releases">
    <img src="https://img.shields.io/badge/View_All-Releases-gray?style=flat&logo=github" alt="All Releases"/>
  </a>
</p>

## 🎥 Preview

<div align="center">
  <a href="https://github.com/Sebastien-VZN/axovox/raw/main/image/output_auroria.mp4">
    <img src="image/desktop_1.jpg" alt="Watch the demo video" width="500">
  </a>
  <p><sub><em>▶ Click to watch the demo — real-time messaging in action</em></sub></p>
</div>

## 📋 Table of Contents

- [⚠️ Project Status](#️-project-status-beta-version)
- [✨ Key Features](#-key-features)
- [💻 Supported Platforms](#-supported-platforms)
- [🎨 Gallery](#-gallery)
- [📊 Performance & Real Cost](#-performance--real-cost)
- [🤖 Bot API](#-bot-api)
- [🌐 About Axomind](#-about-axomind)
- [🟢 Server Status](#-server-status)
- [🤝 Bug Reports & Feedback](#-bug-reports--feedback)
- [📜 Changelog](#-changelog)
- [🛣️ Roadmap & Future of the Project](#️-roadmap--future-of-the-project)
- [👤 Author](#-author)
- [🇫🇷 Version Française](#-version-française)

---

## ⚠️ Project Status: Beta Version

> This project is in active development. Bugs and unexpected behaviors are likely. Feedback is welcome.

> **📧 About emails**
> Email-based features (account verification, password reset, 2FA) are currently disabled. Accounts work without any email step.

---

## ✨ Key Features

**🔒 Privacy & Security**
- 🔒 **Strong Encryption** — Messages and files are encrypted with AES-256-GCM, both when stored on the server and while being sent. Your conversations stay private.
- 🛡️ **Two-factor authentication** — Email-code 2FA at login with anti-spam and bad-attempt detection (currently disabled).
- 🔐 **Access Control** — Each member only sees what they're allowed to, with role-based permissions

**⚡ Real-Time**
- ⚡ **Instant Delivery** — Messages arrive instantly, with automatic reconnection if the link drops
- 📱 **Multi-Device** — Stay signed in on **up to 2 devices for Axovox** (1 desktop + 1 mobile). If you also use Axomind, you get **2 more sessions in parallel** — up to 4 active sessions in total per account, by design

**🎨 Interface**
- 🎨 **27 Themes** — Each with a light and a dark variant, switchable on the fly, with Aurora animations and glassmorphism
- 🌍 **33 Languages** — Full UI translation with native language flags

**💬 Messaging**
- 👥 **Private Channels** — Dedicated spaces for your teams, projects, or topics
- 🎤 **Audio Messages** — Record and send voice clips in your conversations
- 📎 **File Sharing** — Up to 10 files per message (documents, images, videos, audio — 10 MB each)
- ⏱️ **Retention** — Messages kept 1 year on the server / 2 years locally, with optional 24h auto-delete · Files kept 1 month (3 months if pinned)
- 🔤 **Native Spell Check** — In-house fork with French + English support, Levenshtein suggestions, smart filtering of URLs/emails/mentions

**🧩 Integrations**
- 🤖 **Bot API** — Send messages from CI/CD, monitoring, or automation tools (n8n, Make, Zapier...)
- 🔗 **Contextual Linking** — Attach conversations to your projects, tasks, or any external resource

---

<details>
<summary>🛠️ <strong>Tech Stack</strong> — for the curious</summary>

<br/>

<p align="center">
  <a href="https://www.php.net/" target="_blank"><img src="https://img.shields.io/badge/PHP-8.4-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.4"/></a>
  <a href="https://flutter.dev/" target="_blank"><img src="https://img.shields.io/badge/Flutter-Stable-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter"/></a>
  <a href="https://nodejs.org/" target="_blank"><img src="https://img.shields.io/badge/Node.js-LTS-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/></a>
  <a href="https://www.postgresql.org/" target="_blank"><img src="https://img.shields.io/badge/PostgreSQL-Latest-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
  <a href="https://www.nginx.com/" target="_blank"><img src="https://img.shields.io/badge/Nginx-Stable-269539?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx"/></a>
  <a href="https://www.debian.org/" target="_blank"><img src="https://img.shields.io/badge/Debian-13-A81D33?style=for-the-badge&logo=debian&logoColor=white" alt="Debian 13"/></a>
</p>

**How it works (in plain words):**
1. **The app** talks to the server over a secure connection (HTTPS), and a separate live channel keeps everything in sync in real time
2. **The live channel** can keep 2 sessions open at once for Axovox (1 desktop + 1 mobile). The same design supports 2 extra sessions for Axomind in parallel — 4 active sessions total per account
3. **The server** protects accounts on several layers: route checks, attack protection, AES-256-GCM encryption, and a unique token per session
4. **The database** stores everything encrypted, keeps data only as long as needed, and is tuned for fast reads on conversations and messages

</details>

---

## 💻 Supported Platforms

| Platform | Status                 |
|:--------:|:-----------------------|
| Android  | ✅ Supported           |
| Windows  | ✅ Supported           |
| Linux    | ✅ Supported           |
| macOS    | ❌ Not yet supported   |
| iOS      | ❌ Not yet supported   |

---

## 🎨 Gallery

<p align="center">
  <img src="image/desktop_1.jpg" alt="Desktop Screenshot 1" width="49%"/>
  <img src="image/desktop_8.jpg" alt="Desktop Screenshot 8" width="49%"/>
</p>
<p align="center"><sub>Desktop view (left) · Desktop view (right)</sub></p>

<p align="center">
  <img src="image/mobil_0.jpg" alt="Mobile Screenshot 0" width="24%"/>
  <img src="image/mobil_8.jpg" alt="Mobile Screenshot 8" width="24%"/>
</p>
<p align="center"><sub>Mobile view (left) · Mobile view (right)</sub></p>

<details>
<summary>📸 More screenshots — full desktop & mobile gallery</summary>

### 💻 Desktop Experience

<p align="center">
  <img src="image/desktop_2.jpg" alt="Desktop Screenshot 2" width="49%"/>
  <img src="image/desktop_3.jpg" alt="Desktop Screenshot 3" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_4.jpg" alt="Desktop Screenshot 4" width="49%"/>
  <img src="image/desktop_5.jpg" alt="Desktop Screenshot 5" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_6.jpg" alt="Desktop Screenshot 6" width="49%"/>
  <img src="image/desktop_7.jpg" alt="Desktop Screenshot 7" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_9.jpg" alt="Desktop Screenshot 9" width="49%"/>
  <img src="image/desktop_10.jpg" alt="Desktop Screenshot 10" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_11.jpg" alt="Desktop Screenshot 11" width="49%"/>
  <img src="image/desktop_12.jpg" alt="Desktop Screenshot 12" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_13.jpg" alt="Desktop Screenshot 13" width="49%"/>
  <img src="image/desktop_14.jpg" alt="Desktop Screenshot 14" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_15.jpg" alt="Desktop Screenshot 15" width="49%"/>
</p>

### 📱 Mobile Experience

<p align="center">
  <img src="image/mobil_1.jpg" alt="Mobile Screenshot 1" width="19%"/>
  <img src="image/mobil_2.jpg" alt="Mobile Screenshot 2" width="19%"/>
  <img src="image/mobil_3.jpg" alt="Mobile Screenshot 3" width="19%"/>
  <img src="image/mobil_4.jpg" alt="Mobile Screenshot 4" width="19%"/>
  <img src="image/mobil_5.jpg" alt="Mobile Screenshot 5" width="19%"/>
</p>

<p align="center">
  <img src="image/mobil_5.png" alt="Mobile Screenshot 5 (alt)" width="19%"/>
  <img src="image/mobil_6.jpg" alt="Mobile Screenshot 6" width="19%"/>
  <img src="image/mobil_7.jpg" alt="Mobile Screenshot 7" width="19%"/>
  <img src="image/mobil_9.jpg" alt="Mobile Screenshot 9" width="19%"/>
  <img src="image/mobil_10.jpg" alt="Mobile Screenshot 10" width="19%"/>
</p>

<p align="center">
  <img src="image/mobil_11.jpg" alt="Mobile Screenshot 11" width="19%"/>
  <img src="image/mobil_12.jpg" alt="Mobile Screenshot 12" width="19%"/>
  <img src="image/mobil_13.jpg" alt="Mobile Screenshot 13" width="19%"/>
</p>

</details>

---

## 📊 Performance & Real Cost

Hardware specs, load test results (200 users burst, 0 failures) and infrastructure cost analysis — shared with Axomind, since both run on the same server.

→ **[Read detailed analysis](https://github.com/Sebastien-VZN/axomind/blob/main/PERF.md)**

---

## 🤖 Bot API

Send automated messages into any conversation from your CI/CD, monitoring, or automation tools (n8n, Zapier, Make...). → **[Full documentation](https://github.com/Sebastien-VZN/axomind/blob/main/API_BOT.md)**

---

## 🌐 About Axomind

<div align="center">
  <img src="image/logo_axomind.png" alt="Axomind Logo" width="150"/>
</div>

**Axomind** is a broader project that builds on Axovox. It brings together three connected modules:
- **🗓️ Project planning** — Timeline-based Gantt
- **🧠 Mind maps** — For ideas and knowledge
- **💬 Messaging** — Axovox, integrated as the communication layer

The core idea behind Axomind is **contextual linking**: each conversation is attached to a task or a mind map node, so the discussion and the work it relates to stay in the same place. Axovox remains available as a **standalone messaging app** for people who only need the chat side.

Both Axovox and Axomind run on the same custom modular framework. → **[See details on the Axomind repo](https://github.com/Sebastien-VZN/axomind#-about-axovox)**

<div align="center">
  <a href="https://github.com/Sebastien-VZN/axomind"><img src="https://img.shields.io/badge/Axomind-Repository-3423A6?style=for-the-badge&logo=github&logoColor=white" alt="Axomind Repository"/></a>
</div>

---

## 🟢 Server Status

<div align="center">
  <a href="https://quantive-studio.fr/status.php">
    <img src="https://img.shields.io/badge/Server-Status-8A6DF0?style=for-the-badge&logo=serverless&logoColor=white" alt="Server Status"/>
  </a>
  <p><sub>Check the live status of Axovox services</sub></p>
</div>

---

## 🤝 Bug Reports & Feedback

Axovox is in beta. Bug reports, feature ideas and general feedback are welcome — open an issue on the repository (GitHub account required), every entry is read and considered.

The application source code is proprietary and kept private as a deliberate security choice. This public repository contains the documentation, install guides and release builds — not the codebase. External code contributions aren't part of the project model.

---

## 📜 Changelog

All notable releases — from the first public alpha to the latest beta — are documented in [CHANGELOG.md](CHANGELOG.md) ([version française](CHANGELOG_FR.md)).

---

## 🛣️ Roadmap & Future of the Project

### Current hosting — a deliberate choice, not the endgame

The full stack (Axomind + Axovox) currently runs on a single self-hosted refurbished mini-PC. This isn't an ideological stance — it's the result of architecture decisions that pushed energy efficiency to roughly **90% below an equivalent managed cloud setup** in the benchmarks above.

The software is optimized. The limiting factor today isn't technical, it's financial: **I will not move production to a hosting provider until the business plan is solid**, and I'm uncompromising on that point. Self-hosting is therefore the production mode until that condition is met — not by default, by discipline.

### What I need next: real-world feedback and serious collaboration

The technical foundation is solid. What it needs now isn't more code in isolation — it's exposure to real teams using it, so the next features are driven by actual operational needs, not assumptions:

- **Field feedback** from people who communicate and coordinate work daily
- **Serious collaborators** to evaluate which features genuinely move the needle for an organization
- **A grounded scope** for what comes next, decided from usage data — not from a roadmap written in a vacuum

The base is in place. The next step is making sure each addition goes in the right direction.

### Currently in development

- **Spell check** — in-house fork is live; hardening continues (clipboard edge cases, coverage expansion)
- **Quota system** — client-side management is rebuilt; server-side auto-cleanup needs deployment and verification
- **Rich text editor** — fork of `flutter_quill` is live; stability hardening continues

### AI in the project — a tool under control, not an autopilot

AI plays a real role in how I work, but the model stays explicit: **every decision and every line of integration is supervised. AI is an extension of the operator, not a replacement.**

**No vibe coding.** Letting an AI run the keyboard without review is strictly off the table in my workflow. Every AI-produced suggestion — code, configuration, refactor — is read, challenged and validated against the existing test suite before it goes anywhere near production. The rule is simple: the AI proposes, the operator decides, and the tests adjudicate.

**Multi-provider, not single-vendor.** Hands-on practice covers the major US providers (Anthropic, OpenAI, Google), Chinese models, and the full self-hosted catalog reachable through Ollama — each one evaluated on real tasks, not on benchmarks taken at face value. The point isn't to bet on one model; it's to know which one fits which problem.

**Tests as ground truth for the AI itself.** Over 800 automated tests and a full CI/CD pipeline — format check, static analysis, unit tests, integration tests, multi-platform builds, load benchmarks — don't just protect the app. They're the standard the AI checks its own work against. Every critical path can be replayed against real conditions, so AI-assisted changes are validated by measurable returns, not by impressions.

On that practical baseline, Axovox integrates with AI agents through the **Bot API** — send automated messages from CI/CD, monitoring, or automation tools (n8n, Zapier, Make...). Any MCP-compatible client can connect to the Axomind MCP server, which exposes Axovox messaging actions where a bot is assigned.

**MCP server repository:** [github.com/Sebastien-VZN/axomind-mcp](https://github.com/Sebastien-VZN/axomind-mcp)

**Bot API documentation:** [API_BOT.md](https://github.com/Sebastien-VZN/axomind/blob/main/API_BOT.md) — 3 routes, 13 actions, full reference with code examples.

The next step is expanding the tool set based on real field feedback — the same prerequisite as the rest of the roadmap.

---

## 👤 Author

<div align="center">
  <a href="https://sebastien-vezzani.xyz/" target="_blank"><img src="https://img.shields.io/badge/Portfolio-3423A6?style=for-the-badge&logo=firefox-browser&logoColor=white" alt="Link to Portfolio"/></a>
</div>

---

## 🇫🇷 Version Française

<div align="center">
  <img src="image/auroria_link_256.png" alt="Logo Axovox" width="150"/>
  <h1>Axovox</h1>
  <p><strong>Messagerie d'équipe chiffrée sur votre propre serveur. Comme Discord, mais autohébergé — sans intermédiaire.</strong></p>
</div>

## ⚠️ Statut du projet : Version Beta

> Ce projet est en développement actif. Des bugs et comportements inattendus sont probables. Les retours sont bienvenus.

> **📧 À propos des emails**
> Les fonctionnalités liées à l'email (vérification de compte, réinitialisation de mot de passe, 2FA) sont actuellement désactivées. Les comptes fonctionnent sans étape email.

---

## 🎥 Aperçu

<div align="center">
  <a href="https://github.com/Sebastien-VZN/axovox/raw/main/image/output_auroria.mp4">
    <img src="image/desktop_1.jpg" alt="Regarder la vidéo de démonstration" width="500">
  </a>
  <p><sub><em>▶ Cliquez pour regarder la démo — messagerie en temps réel en action</em></sub></p>
</div>

---

## ✨ Fonctionnalités Clés

**🔒 Confidentialité & Sécurité**
- 🔒 **Chiffrement fort** — Messages et fichiers chiffrés en AES-256-GCM, à la fois sur le serveur et lors de l'envoi. Vos conversations restent privées.
- 🛡️ **Double authentification** — 2FA par code email à la connexion avec détection des tentatives suspectes (désactivée pour le moment).
- 🔐 **Contrôle d'Accès** — Chaque membre ne voit que ce à quoi il est autorisé, avec des permissions par rôle

**⚡ Temps Réel**
- ⚡ **Livraison Instantanée** — Les messages arrivent en direct, avec reconnexion automatique en cas de coupure
- 📱 **Multi-Appareils** — Restez connecté sur **2 appareils pour Axovox** (1 desktop + 1 mobile). Si vous utilisez aussi Axomind, vous disposez de **2 sessions supplémentaires en parallèle** — jusqu'à 4 sessions actives au total par compte, par design

**🎨 Interface**
- 🎨 **27 Thèmes** — Chacun avec une variante claire et une sombre, interchangeables à la volée, avec animations Aurora et glassmorphism
- 🌍 **33 Langues** — Traduction complète de l'interface avec drapeaux natifs

**💬 Messagerie**
- 👥 **Canaux Privés** — Des espaces dédiés pour vos équipes, projets ou sujets
- 🎤 **Messages Audio** — Enregistrez et envoyez des clips vocaux dans vos conversations
- 📎 **Partage de Fichiers** — Jusqu'à 10 fichiers par message (documents, images, vidéos, audio — 10 Mo chacun)
- ⏱️ **Rétention** — Messages conservés 1 an sur le serveur / 2 ans en local, avec suppression automatique optionnelle après 24h · Fichiers conservés 1 mois (3 mois si épinglé)
- 🔤 **Correcteur orthographique natif** — Fork maison avec support français + anglais, suggestions Levenshtein, filtrage intelligent des URLs/emails/mentions

**🧩 Intégrations**
- 🤖 **API Bot** — Envoyez des messages depuis vos outils CI/CD, monitoring ou plateformes d'automatisation (n8n, Make, Zapier...)
- 🔗 **Lien Contextuel** — Associez des conversations à vos projets, tâches ou ressources externes

---

<details>
<summary>🛠️ <strong>Stack Technologique</strong> — pour les curieux</summary>

<br/>

<p align="center">
  <a href="https://www.php.net/" target="_blank"><img src="https://img.shields.io/badge/PHP-8.4-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.4"/></a>
  <a href="https://flutter.dev/" target="_blank"><img src="https://img.shields.io/badge/Flutter-Stable-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter"/></a>
  <a href="https://nodejs.org/" target="_blank"><img src="https://img.shields.io/badge/Node.js-LTS-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/></a>
  <a href="https://www.postgresql.org/" target="_blank"><img src="https://img.shields.io/badge/PostgreSQL-Latest-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
  <a href="https://www.nginx.com/" target="_blank"><img src="https://img.shields.io/badge/Nginx-Stable-269539?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx"/></a>
  <a href="https://www.debian.org/" target="_blank"><img src="https://img.shields.io/badge/Debian-13-A81D33?style=for-the-badge&logo=debian&logoColor=white" alt="Debian 13"/></a>
</p>

**Fonctionnement (en clair) :**
1. **L'application** dialogue avec le serveur via une connexion sécurisée (HTTPS), et un canal temps réel séparé garde tout synchronisé en direct
2. **Le canal temps réel** peut maintenir 2 sessions ouvertes pour Axovox (1 desktop + 1 mobile). Le même design supporte 2 sessions supplémentaires pour Axomind en parallèle — 4 sessions actives au total par compte
3. **Le serveur** protège les comptes sur plusieurs niveaux : vérifications des accès, protection contre les attaques, chiffrement AES-256-GCM, et un jeton unique par session
4. **La base de données** stocke tout de façon chiffrée, ne conserve les données que le temps utile, et est optimisée pour des lectures rapides sur les conversations et les messages

</details>

---

## 💻 Plateformes supportées

| Plateforme | Statut                         |
|:----------:|:-------------------------------|
| Android    | ✅ Supporté                    |
| Windows    | ✅ Supporté                    |
| Linux      | ✅ Supporté                    |
| macOS      | ❌ Non supporté pour le moment |
| iOS        | ❌ Non supporté pour le moment |

---

## 🎨 Galerie

<p align="center">
  <img src="image/desktop_1.jpg" alt="Capture desktop 1" width="49%"/>
  <img src="image/desktop_8.jpg" alt="Capture desktop 8" width="49%"/>
</p>
<p align="center"><sub>Vue desktop (gauche) · Vue desktop (droite)</sub></p>

<p align="center">
  <img src="image/mobil_0.jpg" alt="Capture mobile 0" width="24%"/>
  <img src="image/mobil_8.jpg" alt="Capture mobile 8" width="24%"/>
</p>
<p align="center"><sub>Vue mobile (gauche) · Vue mobile (droite)</sub></p>

<details>
<summary>📸 Plus de captures — galerie desktop & mobile complète</summary>

### 💻 Expérience Desktop

<p align="center">
  <img src="image/desktop_2.jpg" alt="Capture desktop 2" width="49%"/>
  <img src="image/desktop_3.jpg" alt="Capture desktop 3" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_4.jpg" alt="Capture desktop 4" width="49%"/>
  <img src="image/desktop_5.jpg" alt="Capture desktop 5" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_6.jpg" alt="Capture desktop 6" width="49%"/>
  <img src="image/desktop_7.jpg" alt="Capture desktop 7" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_9.jpg" alt="Capture desktop 9" width="49%"/>
  <img src="image/desktop_10.jpg" alt="Capture desktop 10" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_11.jpg" alt="Capture desktop 11" width="49%"/>
  <img src="image/desktop_12.jpg" alt="Capture desktop 12" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_13.jpg" alt="Capture desktop 13" width="49%"/>
  <img src="image/desktop_14.jpg" alt="Capture desktop 14" width="49%"/>
</p>

<p align="center">
  <img src="image/desktop_15.jpg" alt="Capture desktop 15" width="49%"/>
</p>

### 📱 Expérience Mobile

<p align="center">
  <img src="image/mobil_1.jpg" alt="Capture mobile 1" width="19%"/>
  <img src="image/mobil_2.jpg" alt="Capture mobile 2" width="19%"/>
  <img src="image/mobil_3.jpg" alt="Capture mobile 3" width="19%"/>
  <img src="image/mobil_4.jpg" alt="Capture mobile 4" width="19%"/>
  <img src="image/mobil_5.jpg" alt="Capture mobile 5" width="19%"/>
</p>

<p align="center">
  <img src="image/mobil_5.png" alt="Capture mobile 5 (alt)" width="19%"/>
  <img src="image/mobil_6.jpg" alt="Capture mobile 6" width="19%"/>
  <img src="image/mobil_7.jpg" alt="Capture mobile 7" width="19%"/>
  <img src="image/mobil_9.jpg" alt="Capture mobile 9" width="19%"/>
  <img src="image/mobil_10.jpg" alt="Capture mobile 10" width="19%"/>
</p>

<p align="center">
  <img src="image/mobil_11.jpg" alt="Capture mobile 11" width="19%"/>
  <img src="image/mobil_12.jpg" alt="Capture mobile 12" width="19%"/>
  <img src="image/mobil_13.jpg" alt="Capture mobile 13" width="19%"/>
</p>

</details>

---

## 📊 Performance & Coût Réel

Spécifications matérielles, résultats des tests de charge (200 users burst, 0 échec) et analyse des coûts d'infrastructure — partagés avec Axomind, les deux tournant sur le même serveur.

→ **[Lire l'analyse détaillée](https://github.com/Sebastien-VZN/axomind/blob/main/PERF.md)**

---

## 🤖 API Bot

Envoyez des messages automatisés dans vos conversations depuis vos outils CI/CD, monitoring ou plateformes d'automatisation (n8n, Zapier, Make...). → **[Documentation complète](https://github.com/Sebastien-VZN/axomind/blob/main/API_BOT.md)**

---

## 🌐 À propos d'Axomind

<div align="center">
  <img src="image/logo_axomind.png" alt="Logo Axomind" width="150"/>
</div>

**Axomind** est un projet plus large qui s'appuie sur Axovox. Il réunit trois modules connectés :
- **🗓️ Planification** — Diagramme Gantt sur une chronologie
- **🧠 Cartes mentales** — Pour les idées et les connaissances
- **💬 Messagerie** — Axovox, intégré comme couche de communication

L'idée centrale d'Axomind est le **lien contextuel** : chaque conversation est rattachée à une tâche ou à un nœud de carte mentale, pour que la discussion et le travail qui s'y rapporte restent au même endroit. Axovox reste disponible comme **application de messagerie autonome** pour celles et ceux qui n'ont besoin que de la partie chat.

Axovox et Axomind reposent sur le même framework modulaire personnalisé. → **[Voir les détails sur le dépôt Axomind](https://github.com/Sebastien-VZN/axomind#-about-axovox)**

<div align="center">
  <a href="https://github.com/Sebastien-VZN/axomind"><img src="https://img.shields.io/badge/Axomind-Dépôt-3423A6?style=for-the-badge&logo=github&logoColor=white" alt="Dépôt Axomind"/></a>
</div>

---

## 🟢 Statut du Serveur

<div align="center">
  <a href="https://quantive-studio.fr/status.php">
    <img src="https://img.shields.io/badge/Serveur-Statut-8A6DF0?style=for-the-badge&logo=serverless&logoColor=white" alt="Statut du Serveur"/>
  </a>
  <p><sub>Vérifiez le statut en direct des services Axovox</sub></p>
</div>

---

## 🤝 Bugs & Retours

Axovox est en beta. Les remontées de bugs, suggestions et retours d'usage sont les bienvenus — ouvrez une issue sur le dépôt (compte GitHub requis), chaque entrée est lue et étudiée.

Le code source de l'application est propriétaire et reste privé par choix de sécurité. Ce dépôt public contient la documentation, les guides d'installation et les builds de release — pas le code de l'application. Les contributions de code externes ne font pas partie du modèle du projet.

---

## 📜 Changelog

Toutes les versions notables — de la première alpha publique à la dernière beta — sont documentées dans [CHANGELOG_FR.md](CHANGELOG_FR.md) ([English version](CHANGELOG.md)).

---

## 🛣️ Roadmap & Avenir du projet

### Hébergement actuel — un choix assumé, pas une finalité

L'ensemble de la stack (Axomind + Axovox) tourne aujourd'hui sur un seul mini-PC reconditionné autohébergé. Ce n'est pas une posture idéologique — c'est le résultat de choix d'architecture qui ont poussé l'efficience énergétique à environ **90 % en dessous d'une stack cloud managée équivalente** dans les benchmarks ci-dessus.

Le logiciel est optimisé. Le facteur limitant aujourd'hui n'est pas technique, il est financier : **je ne basculerai pas la production chez un hébergeur tant que le plan business n'est pas solide**, et je suis intransigeant sur ce point. L'autohébergement est donc le mode de production tant que cette condition n'est pas remplie — pas par défaut, par discipline.

### Ce dont le projet a besoin maintenant : feedback terrain et collaboration sérieuse

La base technique est solide. Ce qui lui manque, ce n'est pas davantage de code en vase clos — c'est l'exposition à des équipes réelles qui l'utilisent, pour que les prochaines fonctionnalités soient guidées par des besoins opérationnels concrets, pas par des hypothèses :

- **Retours terrain** de personnes qui communiquent et coordonnent du travail au quotidien
- **Collaborateurs sérieux** pour évaluer quelles fonctionnalités font réellement bouger les choses dans une organisation
- **Un périmètre ancré dans le réel** pour la suite, décidé à partir de l'usage — pas d'une roadmap écrite hors-sol

Les fondations sont là. L'étape suivante est de s'assurer que chaque ajout va dans le bon sens.

### En cours de développement

- **Correcteur orthographique** — le fork maison est en ligne ; la fiabilisation continue (cas limites du presse-papier, couverture étendue)
- **Système de quotas** — la gestion côté client est reconstruite ; l'auto-cleanup côté serveur doit être déployé et vérifié
- **Éditeur de texte riche** — le fork de `flutter_quill` est en ligne ; la fiabilisation de la stabilité continue

### L'IA dans le projet — un outil sous contrôle, pas un pilote automatique

L'IA joue un rôle réel dans ma façon de travailler, mais le modèle reste clair : **chaque décision et chaque ligne d'intégration est supervisée. L'IA est une extension de l'opérateur, pas un remplaçant.**

**Pas de vibe coding.** Laisser une IA piloter sans relecture est strictement banni de mes usages. Chaque suggestion produite par l'IA — code, configuration, refactor — est lue, challengée et validée contre la suite de tests existante avant d'aller où que ce soit en production. La règle est simple : l'IA propose, l'opérateur décide, les tests tranchent.

**Multi-fournisseurs, pas mono-éditeur.** Ma pratique couvre les principaux fournisseurs américains (Anthropic, OpenAI, Google), les modèles chinois, et l'ensemble du catalogue autohébergé accessible via Ollama — chacun évalué sur des tâches réelles, pas sur des benchmarks pris au mot. L'objectif n'est pas de miser sur un modèle, c'est de savoir lequel répond à quel problème.

**Les tests comme vérité terrain pour l'IA elle-même.** Plus de 800 tests automatisés et un pipeline CI/CD complet — vérification de format, analyse statique, tests unitaires, tests d'intégration, builds multi-plateforme, benchmarks de charge — ne protègent pas seulement l'application. Ils sont le standard contre lequel l'IA confronte son propre travail. Chaque point critique peut être rejoué en conditions réelles, donc les modifications assistées par IA sont validées par des retours mesurables, pas par des impressions.

Sur cette base pratique, Axovox s'intègre aux agents IA via l'**API Bot** — envoyez des messages automatisés depuis vos outils CI/CD, monitoring ou plateformes d'automatisation (n8n, Zapier, Make...). N'importe quel client MCP peut se connecter au serveur MCP Axomind, qui expose les actions de messagerie Axovox là où un bot est affecté.

**Repo du serveur MCP :** [github.com/Sebastien-VZN/axomind-mcp](https://github.com/Sebastien-VZN/axomind-mcp)

**Documentation API Bot :** [API_BOT.md](https://github.com/Sebastien-VZN/axomind/blob/main/API_BOT.md) — 3 routes, 13 actions, référence complète avec exemples de code.

L'étape suivante est d'étendre le set d'outils selon les retours terrain réels — le même prérequis que le reste de la roadmap.

---

## 👤 Auteur

<div align="center">
  <a href="https://sebastien-vezzani.xyz/" target="_blank"><img src="https://img.shields.io/badge/Portfolio-3423A6?style=for-the-badge&logo=firefox-browser&logoColor=white" alt="Lien vers le Portfolio"/></a>
</div>

---
