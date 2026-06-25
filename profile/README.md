# Brainstorm

  **The local-first knowledge OS.** Your data, your apps, your machine.

  Brainstorm is a knowledge-management product modeled as a desktop operating
  system: a secure shell that hosts sandboxed apps over your own data. Notes,
  databases, a graph, a calendar, mail, a browser — every app reads and writes
  the same local vault, and nothing leaves your machine unless you say so.

  ### What makes it different

  - **Local-first.** Your vault lives on your device. Encrypted at rest, yours to
    own, export, and move. The cloud is optional and never holds your content.
  - **Apps over one data model.** Every app speaks [Block Protocol](https://blockprotocol.org)
    for data interop, so a task in one app is the same object everywhere else.
  - **Real-time, conflict-free sync.** Built on [Yjs](https://yjs.dev) CRDTs —
    collaborate live across devices and people, offline-tolerant by design.
  - **Capability-governed sandbox.** Apps run isolated and can only touch what
    you grant them, mediated by a per-vault capability ledger. Security is the
    boundary, not an afterthought.
  - **Rich text that composes.** A [Lexical](https://lexical.dev)-based editor
    shared across every surface.

  ### The repos
  
  | Repo | What it is |
  |------|-----------|
  | `shell` | The product — Electron shell, sandboxed apps, capability ledger, IPC broker, core services |
  | `sync` | Real-time + restore sync engine |
  | `cloud` | Optional control plane — billing, catalog, relay. Never stores vault content |
  | `site` | [getbrainstorm.online](https://getbrainstorm.online) |
  | `harness` | Orchestration hub — design docs, dev MCP server, dogfood harness |

  ---

  *Built in the open. Local-first, agent-ready, yours.*
