# Naheem Olaide

Software engineer focused on backend systems, AI and developer tools. B.Sc. Computer Engineering student at Obafemi Awolowo University, Nigeria.

[Email](mailto:naheemolaide5@gmail.com) · [LinkedIn](https://linkedin.com/in/naheemolaide) · [X](https://x.com/naheem__x)

Open to software engineering internships for summer 2027.

## Open source

| Project | What it does |
| --- | --- |
| [Repo Doctor](https://github.com/appdever01/repo-doctor) | Rust CLI that checks local setup requirements for Node.js and Python projects, with findings and next steps. |
| [Editlane](https://github.com/appdever01/editlane) | Local CLI and read-only MCP server that gathers relevant source files and nearby tests for coding agents. |
| [React Loading Regions](https://github.com/appdever01/react-loading-regions) | Independent loading states for React, with skeletons and checks that compare loading and loaded layouts. |
| [Coolify Uptime Monitor](https://github.com/appdever01/coolify-uptime-monitor) | Self-hosted monitoring with webhook and email alerts when Coolify resources go down or recover. |
| [OneBucket](https://github.com/appdever01/one-bucket) | One file-upload API for AWS S3, Cloudflare R2, Cloudinary and local storage. |
| [Repair WebMCP](https://github.com/appdever01/repair-webmcp) | Interactive 3D repair guides where people and AI agents work together through WebMCP. |

Issues, feedback and contributions are welcome. Each project's README covers its setup and current scope.

## Products

- [Plud](https://plud.app): Study tools built around uploaded course material, including tutoring, quizzes and flashcards.
- [Binx](https://usebinx.com): AI assistant for WhatsApp and the web. Built conversation memory with PostgreSQL, pgvector and reranking, with background workers for summarisation and memory extraction.
- [DBDock](https://dbdock.xyz): Database backup, restore and migration tools. Built schema analysis, type mapping and storage adapters for the CLI and hosted platform.
- [Bucx](https://bucx.app): USDC payments on Solana, with idempotent transfers and transaction confirmation handling.
- [Clymb](https://useclymb.com): Marketing tools for planning, writing and scheduling campaigns.

## How I solve problems

I start by understanding the user’s problem and tracing the existing workflow. I look for the smallest complete solution, make the tradeoffs clear, and check the failure cases before calling it finished.

<details>
<summary>Plud: helping learners work with their own material</summary>

A study response needs context from the learner’s uploaded material. I separate document preparation from question answering: extract the material, split it into searchable chunks, then retrieve and rerank relevant evidence for the response.

```mermaid
flowchart TD
    Upload["Uploaded course material"] --> Extract["Extract text and structure"]
    Extract --> Index["Create chunks and embeddings"]
    Index --> Store[("PostgreSQL: text and vector indexes")]
    Question["Learner question"] --> Retrieve["Retrieve relevant material"]
    Store --> Retrieve
    Retrieve --> Rank["Rerank and assess evidence"]
    Rank --> Context["Assemble source context"]
    Context --> Response["Generate study response"]
```

</details>

<details>
<summary>Binx: remembering what matters in a conversation</summary>

A longer conversation leaves more history to consider for each reply. I retrieve relevant history and rerank stored facts before building the model’s context. Memory extraction and summarisation run separately from the reply path.

```mermaid
flowchart TD
    Message["User message"] --> Retrieve["Retrieve relevant history and facts"]
    Memory[("PostgreSQL + pgvector")] --> Retrieve
    Retrieve --> Rank["Rerank memory candidates"]
    Rank --> Context["Build response context"]
    Context --> Model["Generate reply"]
    Message -.-> Background["Background memory processing"]
    Background --> Memory
```

</details>

<details>
<summary>DBDock: moving data between different database models</summary>

MongoDB documents and PostgreSQL tables represent data differently. I analyse fields, nested structures and possible references, then produce a mapping that can be reviewed before migration. The conversion reports per-table results and errors instead of treating a partial transfer as success.

```mermaid
flowchart TD
    Source[("MongoDB collections")] --> Analyse["Analyse fields and nested structures"]
    Analyse --> Map["Map types and possible references"]
    Map --> Plan["Review migration plan"]
    Plan --> Convert["Convert and insert documents"]
    Convert --> Target[("PostgreSQL tables")]
    Convert --> Report["Per-table results and conversion errors"]
```

</details>

## Experience

At Tekcify, I work on backend and AI systems and deploy products with Docker and GitHub Actions to Linux and AWS. My earlier work includes verification workflows and query optimisation at 3rdlink (Vouchmark), and a Flutter payments app at Cardri Technology that processed over $1 million in transaction volume.

## Recognition

| Result | Event | Year |
| --- | --- | --- |
| 1st place, Team Block X, among 1,600+ submissions | GTCO Squad Hackathon 3.0 | 2026 |
| Runner-up | Zenith Bank Zecathon 5.0 | 2025 |
| 1st place | HackerX Africa AI EduHack | 2024 |
| 1st place | BuildCon Hackathon | 2023 |

## Tools I use

<p>
  <img src="assets/languages/typescript.svg" alt="TypeScript" title="TypeScript" width="36" height="36" />&nbsp;
  <img src="assets/languages/javascript.svg" alt="JavaScript" title="JavaScript" width="36" height="36" />&nbsp;
  <img src="assets/languages/python.svg" alt="Python" title="Python" width="36" height="36" />&nbsp;
  <img src="assets/languages/sql.svg" alt="SQL (PostgreSQL)" title="SQL (PostgreSQL)" width="36" height="36" />&nbsp;
  <img src="assets/languages/dart.svg" alt="Dart" title="Dart" width="36" height="36" />&nbsp;
  <img src="assets/languages/rust.svg" alt="Rust" title="Rust" width="36" height="36" />
</p>

**Languages:** TypeScript, JavaScript, Python, SQL and Dart. Rust for Repo Doctor.

**Backend and data:** Node.js, NestJS, PostgreSQL, pgvector, MongoDB and Redis.

**Web and mobile:** React, Next.js and Flutter.

**Infrastructure:** Docker, AWS, Cloudflare R2 and GitHub Actions.
