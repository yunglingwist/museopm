# Project Management of Cilekler
### HTML-Based Digital Storytelling Game for Museum Visitor Engagement

> *A browser-based interactive narrative game commissioned for a museum exhibition.*
> *Play as a Time Detective. Make choices. Uncover the mystery. Visit the exhibition.*

---

## 🎮 Play the Game

**[▶ Launch Cilekler](https://grandtuvalet.github.io/Cilekler)**

Or scan the QR code at the museum entrance.

No installation. No account. No personal data collected.

---

## About the Project

**Cilekler** is a static, browser-based interactive storytelling game built with [Twine](https://twinery.org) and published via [GitHub Pages](https://pages.github.com).

The player takes on the role of a **Time Detective** investigating a historical mystery connected to real artefacts from a museum exhibition. Choices shape the story, leading to one of several distinct endings — each of which invites the player to visit the museum in person.

| Property         | Details                                              |
|------------------|------------------------------------------------------|
| Type             | Interactive narrative / branching story game         |
| Platform         | Any modern web browser (Chrome, Firefox, Safari)     |
| Play time        | ~10–15 minutes                                       |
| Language         | English                                              |
| Hosting          | GitHub Pages (static, no server)                     |
| Data privacy     | No PII collected, no cookies, no analytics           |
| Access           | URL or QR code (on-site at the museum)               |

---

## Repository Structure

```
Cilekler/
│
├── index.html                  # Main game file (Twine export + custom styling)
├── style.css                   # Custom CSS for layout and typography
│
├── assets/
│   ├── images/                 # AI-generated passage images
│   └── audio/                  # Ambient sound files
│
└── docs/                       # Project documentation (B1874 deliverables)
    ├── 1-Project-Charter.docx
    ├── 1b-Financial-Budget-Plan.docx
    ├── 2-Gantt-Chart.xlsx
    ├── 3-SRS.docx
    ├── 4-Architecture-Diagrams/
    │   ├── system-architecture.jpg
    │   └── application-diagram.jpg
    ├── 5-Sample-Use-Case.docx
    ├── 6-Testing-Methodology-and-a-Test-Case.docx
    ├── 7-Slideshow.docx
    └── 8-User-Manual.docx
```

---

## Project Deliverables

This repository includes all deliverables required for the **B1874 — Project Management and Software Engineering for Cultural Heritage** course exam at the University of Bologna (DHDK, FICLIT, A.Y. 2025/2026).

| # | Deliverable                          | File                                          | Status  |
|---|--------------------------------------|-----------------------------------------------|---------|
| 1 | Project Charter                      | `docs/1-Project-Charter.docx`                 | ✅ Done |
| 1b| Financial Budget Plan                | `docs/1b-Financial-Budget-Plan.docx`          | ✅ Done |
| 2 | Gantt Chart                          | `docs/2-Gantt-Chart.xlsx`                     | ✅ Done |
| 3 | Software Requirement Specification   | `docs/3-SRS.docx`                             | ✅ Done |
| 4 | Architecture Diagrams                | `docs/4-Architecture-Diagrams/`               | ✅ Done |
| 5 | Sample Use Case                      | `docs/5-Sample-Use-Case.docx`                 | ✅ Done |
| 6 | Testing Methodology & Test Case      | `docs/6-Testing-Methodology-and-a-Test-Case.docx` | ✅ Done |
| 7 | Slideshow                            | `docs/7-Slideshow.docx`                       | ✅ Done |
| 8 | User Manual                          | `docs/8-User-Manual.docx`                     | ✅ Done |

---

## Development Process

The project follows a **Waterfall** process model, selected because:

- Requirements were defined upfront by the museum commission brief
- The 8-week academic timeline requires a fixed, sequential plan
- The team of 4 has specialised, non-overlapping roles
- The scope is small and stable — no iterative sprints needed

### Phases

```
Week 1–2  →  Initiation & Requirements (Charter, SRS)
Week 3    →  Design (Architecture, Use Case)
Week 3–4  →  Narrative & Asset Production (story script, images, audio)
Week 4–5  →  Twine Implementation (passages, branching, endings)
Week 5–6  →  HTML/CSS Development (styling, responsive layout, deployment)
Week 7    →  Verification & Validation (testing, bug fixes, content review)
Week 8    →  Delivery (documentation, final review, submission)
```

---

## Tech Stack

| Tool / Technology    | Role                                          | Cost     |
|----------------------|-----------------------------------------------|----------|
| [Twine](https://twinery.org) | Story authoring (branching passages) | Free     |
| HTML / CSS / JS      | Web delivery and custom styling               | Free     |
| [GitHub Pages](https://pages.github.com) | Static hosting        | Free     |
| VS Code              | Code editor                                   | Free     |
| AI image tools       | Passage illustration generation               | ~€120    |
| Audio tools          | Ambient sound                                 | ~€50     |

---

## Architecture

Cilekler is a **single-tier, fully client-side static application** with no server, no backend, and no database.

```
Visitor / Museum Institution
        │  (URL or QR code)
        ▼
   Web Browser  ──────────────────────────────────────
        │                                             │
   Presentation Layer          GitHub Pages CDN (static file host)
   (HTML / CSS / JS)                    │
        │                       index.html + assets
   Application Layer
   ├── Story Engine       (loads and navigates passages)
   ├── Choice Handler     (processes player input)
   ├── Asset Loader       (injects images and audio)
   └── Session Manager    (tracks visited passages)
        │
   Data Layer
   ├── Story Content      (Twine HTML passages)
   ├── Asset Bundle       (images + audio)
   └── Session State      (browser sessionStorage)
```

---

## The Team

| Role                        | Member         |
|-----------------------------|----------------|
| Project Manager & Art Lead  | Ceyda Uyar     |
| Writer & Presenter          | Team Member 2  |
| Twine Developer             | Team Member 3  |
| Web Developer               | Team Member 4  |

---

## Testing

Testing follows a **manual, multi-level approach** covering:

- Narrative unit testing (every passage and link)
- Asset integration testing (images and audio across 3 browsers)
- Branch / path testing — all narrative paths to all endings
- Cross-browser and responsive testing (Chrome, Firefox, Safari; desktop + mobile)
- Performance testing (load time < 5 seconds)
- Domain validation (content accuracy and tone review)
- Privacy check (no PII, no external calls)

Full methodology and Test Case TC-01 are documented in `docs/6-Testing-Methodology-and-a-Test-Case.docx`.

---

## Privacy

Cilekler does not collect, store, or transmit any personal data.
No cookies. No analytics. No account required. No external tracking of any kind.

---

## Licence & Credits

- Game content and narrative: © 2026 Cilekler Team — all rights reserved
- Images: original AI-generated assets produced by the team
- Audio: original or sourced under open licences with attribution (see `assets/audio/`)
- Built with [Twine](https://twinery.org) — open-source, MIT Licence
- Hosted on [GitHub Pages](https://pages.github.com)

---

## Academic Context

This project was developed as the final exam deliverable for:

**B1874 — Project Management and Software Engineering for Cultural Heritage**
DHDK Master's Programme · FICLIT · University of Bologna · A.Y. 2025/2026
Instructor: Paolo Bonora


