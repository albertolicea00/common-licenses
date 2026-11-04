# 📜 Software & Content License Collection

This repository contains curated license templates for everyday development, alongside the official upstream license catalog from the **SPDX (Software Package Data Exchange)** standard.

---

## 🗂️ Directory Structure

```text
.
│
├── README.md                      <-- Guide and license index
├── .gitmodules                    <-- SPDX submodule path and upstream URL
│
├── common/                        <-- 26 essential, widely-used licenses (flat list of .txt files)
│   ├── 0BSD.txt
│   ├── AGPL-3.0-only.txt
│   ├── Apache-2.0.txt
│   ├── BSD-2-Clause.txt
│   ├── BSD-3-Clause.txt
│   ├── BUSL-1.1.txt
│   ├── CC-BY-4.0.txt
│   ├── CC-BY-NC-4.0.txt
│   ├── CC-BY-NC-ND-4.0.txt
│   ├── CC-BY-SA-4.0.txt
│   ├── CC0-1.0.txt
│   ├── EPL-2.0.txt
│   ├── EUPL-1.2.txt
│   ├── GFDL-1.3-only.txt
│   ├── GPL-2.0-only.txt
│   ├── GPL-3.0-only.txt
│   ├── ISC.txt
│   ├── LGPL-2.1-only.txt
│   ├── LGPL-3.0-only.txt
│   ├── MIT.txt
│   ├── MPL-2.0.txt
│   ├── PolyForm-Free-Trial-1.0.0.txt
│   ├── PolyForm-Noncommercial-1.0.0.txt
│   ├── PolyForm-Small-Business-1.0.0.txt
│   ├── SSPL-1.0.txt
│   └── Unlicense.txt
│
└── spdx-license-list-data/         <-- Official SPDX repository, tracked as a Git submodule
    ├── text/                      (Plain text license and exception files)
    ├── json/                      (Machine-readable metadata for all licenses)
    ├── html/                      (HTML versions of licenses)
    ├── markdown/                  (Markdown versions of licenses)
    └── ...                        (Other upstream data and project files)
```

---

## 🌐 Official Sources & Canonical References

All licenses listed here are sourced directly from regulatory bodies, standards organizations, and canonical upstream repositories:

1. **SPDX (Software Package Data Exchange)**:
   - Website: [https://spdx.org/licenses/](https://spdx.org/licenses/)
   - Official Data Repository: [https://github.com/spdx/license-list-data](https://github.com/spdx/license-list-data)
   - *ISO/IEC 5962 standard for license identification and metadata.*
2. **OSI (Open Source Initiative)**:
   - Website: [https://opensource.org/licenses](https://opensource.org/licenses)
   - *The official steward of the Open Source Definition and certified open-source licenses.*
3. **FSF (Free Software Foundation) / GNU Project**:
   - Website: [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/)
   - *Authors and maintainers of the GPL, AGPL, LGPL, and GFDL families.*
4. **Choose a License (GitHub)**:
   - Website: [https://choosealicense.com/](https://choosealicense.com/)
   - *Curated reference guide created and maintained by GitHub.*
5. **Creative Commons**:
   - Website: [https://creativecommons.org/](https://creativecommons.org/)
   - *Global standard licenses for artistic content, media, datasets, and documentation.*
6. **The PolyForm Project**:
   - Website: [https://polyformproject.org/](https://polyformproject.org/)
   - *Drafting modern source-available and non-commercial license frameworks.*

---

## 🧭 Quick Selection Matrix: Which license should you choose?

| Project Goal | File in `common/` | Category |
| :--- | :--- | :--- |
| Maximum adoption, simplicity, minimal friction | `MIT.txt` | Permissive |
| Corporate-friendly with explicit patent grant/protection | `Apache-2.0.txt` | Permissive |
| Improve my library without locking in those improvements | `MPL-2.0.txt` or `LGPL-3.0-only.txt` | Weak Copyleft |
| Ensure all derivative projects remain 100% free & open | `GPL-3.0-only.txt` | Strong Copyleft |
| Cloud / SaaS backend to prevent unlicensed proprietary hosting | `AGPL-3.0-only.txt` | Strong Network Copyleft |
| Artwork, audio, 3D models, books, documentation | `CC-BY-4.0.txt` or `CC-BY-SA-4.0.txt` | Content / Media |
| Waive all copyright / complete public domain dedication | `Unlicense.txt` or `CC0-1.0.txt` | Public Domain |
| Code audit / evaluation / non-commercial usage only | `PolyForm-Noncommercial-1.0.0.txt` | Source-Available |

---

## 📚 Categorized Breakdown of the Licenses in `common/`

All 26 files reside directly inside [`common/`](./common/) in plain text (`.txt`). Here is how they are grouped and what each one does:

### 1. Permissive Licenses
*Permissive licenses grant nearly unlimited freedom: anyone can use, study, modify, merge, publish, sublicense, and sell copies of the software—including incorporating it into closed-source, proprietary software. The primary requirement is retaining the copyright notice and warranty disclaimer.*

* **`MIT.txt` (MIT License)**:
  - The most widely used open-source license in the world. Extremely concise; only requires preserving the original copyright notice and warranty disclaimer in all copies or substantial portions.
  - *Popular examples*: React, Node.js, Vue.js, jQuery, Rust crates.
* **`Apache-2.0.txt` (Apache License 2.0)**:
  - Robust enterprise license. Includes an explicit grant of patent rights from contributors and terminates patent licenses if someone sues the project for patent infringement.
  - *Popular examples*: Kubernetes, Apache HTTP Server, Android OS, TensorFlow.
* **`BSD-2-Clause.txt` (BSD 2-Clause "Simplified")**:
  - Requires only preserving copyright notices in source code and binaries.
  - *Popular examples*: FreeBSD, Nginx.
* **`BSD-3-Clause.txt` (BSD 3-Clause "New" / "Revised")**:
  - Adds a non-endorsement clause prohibiting the use of authors' names for promotion or endorsement without prior written consent.
  - *Popular examples*: Go (Golang), NumPy, BSD Unix.
* **`ISC.txt` (ISC License)**:
  - Functionally equivalent to MIT and 2-Clause BSD, simplified by the Internet Systems Consortium. Standard in OpenBSD and npm default templates.
* **`0BSD.txt` (BSD Zero Clause)**:
  - Removes even the attribution requirement. Ideal for code snippets, reference implementations, and tutorials.
* **`Unlicense.txt` (The Unlicense)**:
  - Explicit dedication to the public domain paired with a disclaimer of warranty.
* **`CC0-1.0.txt` (Creative Commons Zero 1.0 Universal)**:
  - Internationally vetted legal waiver dedicating software, datasets, and digital assets to the global public domain.

---

### 2. Weak Copyleft Licenses
*Weak copyleft licenses require that modifications made directly to the covered library/source code remain open-source under the same terms. However, they allow the library to be linked or combined with proprietary, closed-source applications without forcing the parent application to open its source code.*

* **`MPL-2.0.txt` (Mozilla Public License 2.0)**:
  - File-level copyleft. Modifying an MPL-covered file requires releasing changes under MPL. Creating new files in the larger project allows choosing any other license (even closed-source).
  - *Popular examples*: Firefox, Terraform (pre-BSL versions), HashiCorp Vault.
* **`LGPL-3.0-only.txt` (GNU Lesser General Public License v3.0)**:
  - Allows proprietary applications to dynamically or statically link with the library, as long as users can re-link or modify the LGPL component.
  - *Popular examples*: 7-Zip (portions), Qt (free edition).
* **`LGPL-2.1-only.txt` (GNU Lesser General Public License v2.1)**:
  - Historic version of LGPL still widely used in core multimedia and system utilities for backwards compatibility.
  - *Popular examples*: FFmpeg, GLib, GNU C Library.
* **`EPL-2.0.txt` (Eclipse Public License 2.0)**:
  - Designed for modular enterprise plugins with file/module copyleft and reciprocal patent protection.
  - *Popular examples*: Eclipse IDE, Clojure, JUnit.

---

### 3. Strong Copyleft Licenses
*Strong copyleft licenses mandate that any derivative work or application that incorporates the licensed code must be distributed in its entirety under the same license terms, ensuring complete source code availability.*

* **`GPL-3.0-only.txt` (GNU General Public License v3.0)**:
  - Flagship free software license. Requires all derivative works to be open-source under GPLv3. Features anti-patent retaliation and anti-"Tivoization" hardware-locking clauses.
  - *Popular examples*: Blender, GIMP, Bash, VLC.
* **`GPL-2.0-only.txt` (GNU General Public License v2.0)**:
  - The landmark 1991 copyleft license that powered the rise of Linux.
  - *Popular examples*: Linux Kernel, Git, WordPress.
* **`AGPL-3.0-only.txt` (GNU Affero General Public License v3.0)**:
  - Extends copyleft to network services (SaaS). If users interact with the program over a network or web interface, the server operator must provide the complete source code to those network users.
  - *Popular examples*: Mastodon, Nextcloud, Grafana, Supabase (parts).
* **`EUPL-1.2.txt` (European Union Public Licence 1.2)**:
  - Strong copyleft license created by the European Commission, legally validated across all 23 official EU languages and explicitly compatible with GPL and MPL.

---

### 4. Source-Available / Restricted Licenses
*These licenses allow users to view, audit, and compile source code, but do **not** meet the Open Source Initiative (OSI) criteria because they place restrictions on commercial usage, cloud hosting, or monetization.*

* **`PolyForm-Noncommercial-1.0.0.txt`**:
  - Grants full rights for evaluation, personal use, research, and modification, explicitly prohibiting commercial advantage or monetary compensation.
* **`PolyForm-Free-Trial-1.0.0.txt`**:
  - Grants permissions solely for evaluation testing up to 32 consecutive calendar days.
* **`PolyForm-Small-Business-1.0.0.txt`**:
  - Grants commercial use provided the business stays below specific revenue or headcount limits.
* **`BUSL-1.1.txt` (Business Source License 1.1)**:
  - Created by MariaDB and utilized by Sentry/CockroachDB. Restricts certain competitive commercial uses (e.g. cloud managed service hosting) before automatically transitioning into an open-source license on a set date.
* **`SSPL-1.0.txt` (Server Side Public License 1.0)**:
  - Created by MongoDB. Mandates that anyone offering the software as a cloud service must open-source the complete surrounding management, automation, and infrastructure software stack.

---

### 5. Media, Assets & Documentation (Creative Commons & Free Documentation)
*Optimized for non-code artifacts such as technical manuals, audio, 3D models, graphics, and training datasets.*

* **`CC-BY-4.0.txt` (Attribution 4.0 International)**:
  - Allows sharing, remixing, and commercial use with author attribution.
* **`CC-BY-SA-4.0.txt` (Attribution-ShareAlike 4.0 International)**:
  - Requires author attribution and mandates derivative works be released under the exact same license terms (used by Wikipedia).
* **`CC-BY-NC-4.0.txt` (Attribution-NonCommercial 4.0 International)**:
  - Permits sharing and remixing exclusively for non-commercial purposes with attribution.
* **`CC-BY-NC-ND-4.0.txt` (Attribution-NonCommercial-NoDerivatives 4.0 International)**:
  - Only allows downloading and sharing the original work in unmodified form for non-commercial purposes.
* **`GFDL-1.3-only.txt` (GNU Free Documentation License v1.3)**:
  - FSF copyleft license crafted specifically for software manuals, technical guides, and instructional textbooks.

---

## 🔄 Managing the SPDX Git Submodule

The directory [`spdx-license-list-data/`](./spdx-license-list-data/) is a Git submodule pointing to the official [SPDX license data repository](https://github.com/spdx/license-list-data). The parent repository records a specific upstream commit; `.gitmodules` records its path and URL. The selected templates in `common/` are maintained separately and are not automatically refreshed when the submodule changes.

### Clone this repository without downloading SPDX

```sh
git clone https://github.com/albertolicea00/common-licenses.git
cd common-licenses
```

GitHub displays the submodule as a link to the recorded upstream commit. Its contents do not need to be downloaded locally or uploaded with this repository.

### Download SPDX locally (optional)

To initialize the submodule at the recorded commit:

```sh
git submodule update --init --recursive
```

### Update to the latest upstream version

Run from the root of this repository:

```sh
git submodule update --remote spdx-license-list-data
git diff --submodule
git add spdx-license-list-data
git commit -m "chore: update SPDX license data"
```

Review the upstream changes before committing the new submodule reference. To restore the version recorded by the parent repository, run `git submodule update --init --recursive`.

---

## ⚙️ How to Apply a License Template to Your Project

1. Pick the template from [`common/`](./common/) that fits your project.
2. Copy it to the root of your project directory as `LICENSE` or `LICENSE.txt`.
3. Open the file and fill in placeholder tags:
   - `[year]` or `<year>`: The current year (e.g., `2026`).
   - `[fullname]` or `<copyright holders>`: Your name, team, or organization.
