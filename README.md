# cairo-mai-projects-ws26

MAI Project Module WS 26/27 at THWS (CAIRO, FIW), supervised by Prof. Dr. Ivan P. Yamshchikov. Monorepo for three student teams: Percy (agentic M365 inbox butler), Vogon (self-hosted AI form-filling assistant) and KIWi (RAG knowledge assistant for the HISinOne CampusPortal).

## Course info
- **Module:** MAI Project Module, 10 ECTS, teams of 3, English
- **Faculty:** FIW – Faculty of Computer Science and Business Information Systems, THWS
- **Center:** CAIRO – Center for AI and Robotics
- **Supervisor:** Prof. Dr. Ivan P. Yamshchikov

## Projects
| Project | Topic | Folder |
|---|---|---|
| **Percy** | Agentic inbox butler for Microsoft 365: triage, scheduled digests, urgent alerts via Telegram/WhatsApp | [`percy/`](percy/) |
| **Vogon** | Self-hosted LLM that fills travel requests / purchase orders and drafts emails (reference: SPARK Workflow) | [`vogon/`](vogon/) |
| **KIWi** | Local RAG assistant for HISinOne CampusPortal knowledge, with source citations | [`kiwi/`](kiwi/) |

## Team members
| Name | Team | GitHub handle |
|---|---|---|
| Abin Skaria | Percy | @Abin-28 |
| Anshita Ramayanam | Percy |  |
| Harshavardini Gowrisankar | Percy |  |
| Dhrumil Desai | Vogon |  |
| Krish Dhanani | Vogon |  |
| Ruisheng He | Vogon |  |
| Svetlana Gorovaia | Vogon |  |
| Chandana Lakshmisagara Udayashankar | KIWi |  |
| Sahana Mysore Venkatesh | KIWi |  |
| Shreyas Hosadurga Sadananda | KIWi |  |
| Suhaim Manna | KIWi |  |

## Milestones
1. **Poster session** – requirements, architecture, chosen stack
2. **Paper** – methodology and evaluation design
3. **Demo** – working prototype with evaluation results

## Repo structure
```
.
├── percy/    # Team Percy
├── vogon/    # Team Vogon
├── kiwi/     # Team KIWi
├── shared/   # Code reused by several teams
└── docs/     # Shared docs, meeting notes, guidelines
```
Each project folder has its own `README.md`, `src/`, `tests/` and `docs/`. Teams decide their own tooling (Docker, CI, etc.) inside their folder.

## Getting started
```bash
git clone https://github.com/Abin-28/cairo-mai-projects-ws26.git
cd cairo-mai-projects-ws26
git checkout -b <team>/<short-description>
```

## Working rules
- Work only in your team's folder. Reading other teams' folders is welcome.
- Do not push directly to `main`: create a branch named `<team>/<short-description>` (e.g. `percy/graph-oauth`), push it and open a pull request.
- Ask a teammate to review before merging. Changes in `shared/` should be reviewed by someone from another team.
- Keep commit messages short, e.g. `percy: add Graph mail fetcher`.

## Data and privacy rules
- **Never commit secrets** (API keys, bot tokens, client secrets). Use `.env` (gitignored) and commit only `.env.example`.
- **Never commit real data** (real emails, real forms, real HISinOne documents). Only anonymised or synthetic samples.
- Self-hosted projects (Vogon, KIWi) must make **no external API calls** with sensitive data.

## License
To be decided with the supervisor. Code adapted from SPARK Workflow (EUPL 1.2) must keep its license notice.
