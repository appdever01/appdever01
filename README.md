<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12&height=200&section=header&text=Naheem&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Software%20Engineer%20%E2%80%A2%20Backend%20%E2%80%A2%20AI%20Systems&descAlignY=60&descSize=18" width="100%"/>

<p>
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=700&size=22&duration=2800&pause=900&color=00F7FF&center=true&vCenter=true&width=650&lines=Software+Engineer+%E2%9A%A1+Backend+%26+AI+Systems;Designing+systems%2C+not+just+features;Production+software+that+real+users+depend+on;Retrieval+%E2%80%A2+Payments+%E2%80%A2+Infrastructure" alt="Typing SVG" />
</p>

<p>
  <a href="https://linkedin.com/in/naheemolaide"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://x.com/naheem__x"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" /></a>
  <a href="mailto:naheemolaide5@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

</div>

---

## About

```ts
const naheem = {
  role: "Software Engineer",
  education: "B.Eng. Computer Engineering, Obafemi Awolowo University",
  location: "Lagos, Nigeria",
  focus: ["backend systems", "retrieval & AI infrastructure", "payments"],
  stack: ["TypeScript", "Python", "Node", "Postgres + pgvector", "Redis", "Flutter"],
  building: ["Binx", "Plud", "Bucx", "Clymb", "DBDock"],
};
```

---

## Engineering Notes

A few decisions I would defend in a code review.

**Retrieval instead of recall.** Binx AI stores conversation memory in PostgreSQL with pgvector. Rather than resending an entire transcript on every request, it retrieves semantically relevant fragments and reranks them before assembling context, so context size and inference cost stay flat as a conversation grows.

**Separate the workloads.** User-facing requests take the fast path. Summarisation, memory extraction, classification and metadata generation run as asynchronous workers on lower-cost models, off the path a user can feel.

**Payments are unforgiving.** I worked on a Flutter application powering intra-Africa payments that has processed over $1M in transaction volume. Correctness stops being an abstract virtue when the numbers belong to someone.

**Ship it, then run it.** Docker deployments, CI/CD and monitoring, plus the unglamorous half: diagnosing live incidents and profiling slow queries on systems already in production.

---

## Shipping

<table>
  <tr>
    <td width="50%" valign="top">

### [Binx AI](https://usebinx.com)
`ai assistant`

Multimodal assistant on WhatsApp and the web: search, document analysis, reminders, voice transcription and image generation. Reached 1,000 users in its first two days.

<a href="https://usebinx.com"><img src="https://img.shields.io/badge/usebinx.com-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>

</td>
    <td width="50%" valign="top">

### [Bucx](https://bucx.app)
`fintech`

Stablecoin payment infrastructure for USDC transfers on Solana, covering API design, transaction handling and deployment.

<a href="https://bucx.app"><img src="https://img.shields.io/badge/bucx.app-000000?style=for-the-badge&logo=solana&logoColor=white" /></a>

</td>
  </tr>
  <tr>
    <td width="50%" valign="top">

### [Plud](https://plud.app)
`document intelligence`

AI study platform that grounds tutoring, quizzes, flashcards and exam simulation in a student's own material, with live multiplayer sessions.

<a href="https://plud.app"><img src="https://img.shields.io/badge/plud.app-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>

</td>
    <td width="50%" valign="top">

### [Clymb](https://useclymb.com)
`autonomous marketing`

Marketing platform where agents plan, write and schedule campaigns from a single product brief.

<a href="https://useclymb.com"><img src="https://img.shields.io/badge/useclymb.com-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>

</td>
  </tr>
  <tr>
    <td width="50%" valign="top">

### [DBDock](https://dbdock.xyz)
`database devops`

Dashboard and CLI to back up, restore, copy, schedule and migrate PostgreSQL and MongoDB workloads to your own storage, without living in the terminal.

<a href="https://dbdock.xyz"><img src="https://img.shields.io/badge/dbdock.xyz-000000?style=for-the-badge&logo=postgresql&logoColor=white" /></a>

</td>
    <td width="50%" valign="top">

### [Coolify Uptime Monitor](https://github.com/appdever01/coolify-uptime-monitor)
`open source`

Self-hosted uptime monitoring for any Coolify instance. Edge-triggered webhooks and email alerts when apps, services or databases go down.

<a href="https://github.com/appdever01/coolify-uptime-monitor"><img src="https://img.shields.io/badge/source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

</td>
  </tr>
</table>

---

## Recognition

| Placement | Event | Year |
|---|---|---|
| **1st Overall**, from 1,600+ submissions | GTCO Squad Hackathon 3.0 (Team Block X) | 2026 |
| **Runner-up** | Zenith Bank Zecathon 5.0 | 2025 |
| **1st Place** | HackerX Africa AI EduHack | 2024 |
| **Top 10 Worldwide** | Bolt Hackathon | 2024 |
| **1st Place** | BuildCon Hackathon | 2023 |

---

## Stack

<div align="center">

**Languages**
<p>
  <img src="https://skillicons.dev/icons?i=ts,js,python,dart,bash" />
</p>

**Frontend & Mobile**
<p>
  <img src="https://skillicons.dev/icons?i=nextjs,react,flutter,tailwind" />
</p>

**Backend**
<p>
  <img src="https://skillicons.dev/icons?i=nodejs,nestjs,express,fastapi" />
</p>

**Data & Infra**
<p>
  <img src="https://skillicons.dev/icons?i=postgres,redis,mongodb,supabase" />
  <img src="https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
</p>

**Cloud & DevOps**
<p>
  <img src="https://skillicons.dev/icons?i=aws,docker,linux,vercel,cloudflare,nginx" />
</p>

**AI**
<p>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Anthropic-191919?style=for-the-badge&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG%20%26%20Reranking-0D1117?style=for-the-badge" />
</p>

</div>

---

## Activity

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=appdever01&theme=tokyonight&hide_border=true&background=0D1117&ring=00F7FF&fire=00F7FF&currStreakLabel=00F7FF" height="175" />

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=appdever01&theme=tokyonight&exclude=html,css" width="49%" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=appdever01&theme=tokyonight&exclude=html,css" width="49%" />

</div>

---

<div align="center">

### Get in touch

Open to Summer 2027 software engineering internships.

<a href="mailto:naheemolaide5@gmail.com"><img src="https://img.shields.io/badge/naheemolaide5@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://linkedin.com/in/naheemolaide"><img src="https://img.shields.io/badge/naheemolaide-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://x.com/naheem__x"><img src="https://img.shields.io/badge/@naheem__x-000000?style=for-the-badge&logo=x&logoColor=white" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12&height=120&section=footer"/>

</div>
