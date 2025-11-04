
# ⚓ Allegheny Service Navigator (ASN) Development Repository

The Allegheny Service Navigator is a non-profit initiative dedicated to solving critical service delivery issues by centralizing and verifying resource information for individuals experiencing homelessness in Allegheny County, PA.

This repository holds the entire codebase for the ASN platform, including the public-facing static site and the MediaWiki application.

---

## 1. Project Overview & Mission

The core problem in social service delivery is relying on **outdated, disparate, and difficult-to-search information.** The ASN is built to transition from static resource lists to a dynamic, searchable knowledge base.

Our data collection model is uniquely focused on capturing **real-world resolution pathways** and **operational status** directly from frontline case managers and individuals with lived experience, providing a critical layer of data on service efficacy that traditional directories lack.

---

## 2. Platform & Technical Stack

The Navigator is built on a highly structured knowledge-base foundation to ensure data integrity and complex query functionality.

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Primary Platform** | **MediaWiki** | Core knowledge base application, installed in the `/wiki` subdirectory. |
| **Data Structure** | **Semantic MediaWiki (SMW)** | Transforms the wiki into a structured database, enabling powerful, filtered searches. |
| **Verification** | **FlaggedRevisions** | Enforces a mandatory content approval workflow to ensure all published data is partner-verified. |
| **Frontend** | HTML/CSS | Public-facing landing page (`index.html`) on the root domain. |

---

## 3. Repository Structure

This is a unified repository containing all code for both the live landing page and the core application.

```
allegheny-service-navigator/
├── README.md              # This file.
├── index.html             # Public-facing Landing Page (served from root /)
├── /wiki/                 # Full MediaWiki Installation
│   ├── LocalSettings.php  # (Sensitive config - SEE .gitignore)
│   ├── extensions/        # SMW, FlaggedRevisions, Maps, etc.
├── .gitignore             # Critical file excluding cache, temp, and sensitive config.
└── /assets/               # Logo, font files, etc.
```

***NOTE on Security:*** The `/wiki/LocalSettings.php` file, which contains database credentials and secret keys, is explicitly excluded via the `.gitignore` file. **DO NOT** commit this file. A `LocalSettings.php.sample` may be provided for guidance.

---

## 4. Current Development Status

The project is currently in the **Data Structuring and Platform Build Phase (Q4 2025)**.

| Status | Details |
| :--- | :--- |
| **Live Status** | Static Partner Portal Live at `[Your Domain URL]` |
| **Development Focus** | Finalizing the Semantic MediaWiki (SMW) data schema for service provider entities. |
| **Next Milestone** | Finalizing the mobile-responsive skin and implementing the FlaggedRevisions verification workflow. |

---

## 5. Collaboration & Contact

We welcome technical contributions and input on the data structure. Please use the following resources to get started.

### A. Key Links
*   **Live Landing Page:** `[Your Root Domain URL]`
*   **Project Management Board:** `[Link to Your GitHub Project Board]`
*   **Legal Status:** Registered non-profit organization in the Commonwealth of Pennsylvania.

### B. Contact
For all technical inquiries, collaboration requests, and partnership proposals, please contact the Project Lead:

**Email:** `Contact.ASNav@proton.me`
