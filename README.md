<!-- ═══════════════ HERO · the 6-second layer ═══════════════ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:020024,45:0A2463,100:1E6FD9&height=210&section=header&text=Chaitanya%20Srivastava&fontSize=46&fontColor=E6F1FF&fontAlignY=36&desc=Backend%20Developer%20%C2%B7%20Node.js%20%C2%B7%20PostgreSQL%20%C2%B7%20Redis&descSize=17&descAlignY=57&animation=fadeIn" alt="Chaitanya Srivastava"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=600&lines=I+build+backends+that+handle+money+%26+concurrency;ACID+transactions+%C2%B7+idempotent+APIs+%C2%B7+caching;Learning+system+design%2C+AWS+%26+distributed+systems" alt="typing"/>
</p>

<p align="center">
  📍 Jamshedpur, India &nbsp;&nbsp;·&nbsp;&nbsp; 🎓 B.Tech IT @ VIT Vellore ’28 &nbsp;&nbsp;·&nbsp;&nbsp; 💼 Ex-intern @ Tata Steel, KalkiNi
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/chaitanya-srivastava-904473300/"><img src="https://img.shields.io/badge/LinkedIn-0A2463?style=for-the-badge&logo=linkedin&logoColor=E6F1FF"/></a>
  <a href="mailto:srivastavachaitanya408@gmail.com"><img src="https://img.shields.io/badge/Email-0A2463?style=for-the-badge&logo=gmail&logoColor=E6F1FF"/></a>
  <a href="https://leetcode.com/u/chaitanya0111/"><img src="https://img.shields.io/badge/LeetCode-0A2463?style=for-the-badge&logo=leetcode&logoColor=E6F1FF"/></a>
  <a href="tel:+919798864033"><img src="https://img.shields.io/badge/+91_9798864033-0A2463?style=for-the-badge&logo=whatsapp&logoColor=E6F1FF"/></a>
</p>

<br/>

| 🔧 &nbsp;I build | 💼 &nbsp;I've worked at | 🎯 &nbsp;I'm learning |
|:---:|:---:|:---:|
| Backend systems for money,<br/>auth & concurrent writes | **Tata Steel** — .NET / Oracle<br/>**KalkiNi** — AI surveillance startup | System design · AWS<br/>Docker · Distributed systems |

<br/>

<p align="center">
  <img src="https://skillicons.dev/icons?i=js,nodejs,express,postgres,redis,mongodb,docker,git,linux&theme=dark" alt="stack"/>
</p>

<br/>

<!-- ═══════════════ FEATURED WORK ═══════════════ -->
<h3 align="center">Featured work</h3>

<p align="center">
  <a href="https://github.com/code0101cs/Wallet-Ledger">
    <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=code0101cs&repo=Wallet-Ledger&bg_color=0A192F&title_color=58A6FF&text_color=C9D6EA&icon_color=1F6FEB&border_color=1F3B73&border_radius=10"/>
  </a>
  <a href="https://github.com/code0101cs/PaperStreets">
    <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=code0101cs&repo=PaperStreets&bg_color=0A192F&title_color=58A6FF&text_color=C9D6EA&icon_color=1F6FEB&border_color=1F3B73&border_radius=10"/>
  </a>
</p>

<br/>

<!-- ═══════════════ DEEP-DIVE · for people who stay ═══════════════ -->
<h3 align="center">Want the details? Click any section ↓</h3>

<details>
<summary><b>👋 About me</b> &nbsp;—&nbsp; backend dev who likes the unglamorous parts</summary>
<br/>

Backend developer working in **Node.js, Express and PostgreSQL**, currently doing my B.Tech in Information Technology at **VIT Vellore**.

The parts of backend work I enjoy most are the ones that break quietly: transactions, isolation levels, race conditions on concurrent writes, and APIs that behave correctly when a client retries. My internships taught me something I didn't expect — **reading a codebase I didn't write is the harder skill**, and the more useful one.

</details>

<details>
<summary><b>💼 Experience</b> &nbsp;—&nbsp; Tata Steel (2026) · KalkiNi (2025)</summary>
<br/>

**Intern · Tata Steel** &nbsp;<sub>May – Jun 2026 · Jamshedpur · On-site</sub>
- Worked on two internal **.NET** applications running on **Oracle**
- Migrated jQuery 1 → 3 and Bootstrap 3 → 4, plus feature and bug-fix work

**Software Development Intern · KalkiNi** &nbsp;<sub>Aug – Dec 2025 · Vellore</sub>
- Joined an **AI surveillance startup** at its initial stage
- Learned to navigate and contribute to a codebase I didn't write

</details>

<details>
<summary><b>🚀 Projects in depth</b> &nbsp;—&nbsp; ledger · backtester · auth · expense tracker</summary>
<br/>

**💸 [Wallet / Ledger System](https://github.com/code0101cs/Wallet-Ledger)** &nbsp;`Node.js` `Express 5` `PostgreSQL` `JWT`
- Double-entry accounting: balances are **derived from an append-only ledger**, never stored as a mutable column
- `SELECT ... FOR UPDATE` row locking so concurrent transfers can't overdraw an account
- **Idempotency keys** so a retried request never double-posts an entry
- Every transfer is one DB transaction — all writes commit or none do

**📊 [Paper Streets](https://github.com/code0101cs/PaperStreets)** &nbsp;`Node.js` `MongoDB` `EJS` `Chart.js`
- Backtests **Moving Average Crossover** and **Buy-and-Hold** strategies on historical market data
- Trade log, final portfolio value, and a price chart with BUY/SELL signals
- Session-based auth with saved backtest history per user

**🔐 [Authentication System](https://github.com/code0101cs/Authentication-System)** &nbsp;`Node.js` `bcrypt`
- Password hashing, sessions and protected routes built from scratch

**🧾 [Expense Tracker](https://github.com/code0101cs/Expense_Tracker)** &nbsp;`Node.js` `EJS`
- Server-rendered CRUD app for tracking expenses

</details>

<details>
<summary><b>🎯 Currently working on</b> &nbsp;—&nbsp; system design · AWS · Docker · security</summary>
<br/>

| | |
|---|---|
| ⚙️ **System design** | Load balancing, horizontal scaling, and where the cache actually belongs |
| ☁️ **AWS** | EC2, RDS, and getting IAM permissions right without opening everything up |
| 🐳 **Docker & CI/CD** | So deploys stop being a manual process |
| 🔒 **Security** | Looking at systems from an attacker's point of view |
| 🌐 **Distributed systems** | Eventual consistency, and what breaks when a service stops responding |

</details>

<details>
<summary><b>🧰 Full stack</b> &nbsp;—&nbsp; JS · Node · Postgres · Redis · Mongo · Docker</summary>
<br/>

| Area | Tools |
|---|---|
| **Languages** | JavaScript |
| **Backend** | Node.js, Express, REST APIs, MVC |
| **Databases** | PostgreSQL, MongoDB (Mongoose), Redis |
| **Auth & security** | JWT, bcrypt, express-session |
| **Frontend (server-rendered)** | EJS, HTML, CSS, Chart.js |
| **Tooling** | Git, Docker, Postman, Linux |

</details>

<details>
<summary><b>📊 GitHub activity</b></summary>
<br/>

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=code0101cs&show_icons=true&include_all_commits=true&count_private=true&bg_color=0A192F&title_color=58A6FF&text_color=C9D6EA&icon_color=1F6FEB&border_color=1F3B73&border_radius=10"/>
  <img height="165" src="https://streak-stats.demolab.com?user=code0101cs&background=0A192F&ring=1F6FEB&fire=58A6FF&currStreakNum=E6F1FF&sideNums=E6F1FF&currStreakLabel=58A6FF&sideLabels=58A6FF&dates=8892B0&stroke=1F3B73&border=1F3B73&border_radius=10"/>
</p>

<p align="center">
  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=code0101cs&bg_color=0A192F&color=58A6FF&line=1F6FEB&point=E6F1FF&area=true&area_color=1F6FEB&hide_border=true&radius=10"/>
</p>

</details>

<br/>

<!-- ═══════════════ FOOTER ═══════════════ -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/code0101cs/code0101cs/output/github-snake-dark.svg"/>
    <img alt="contribution snake" src="https://raw.githubusercontent.com/code0101cs/code0101cs/output/github-snake.svg"/>
  </picture>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1E6FD9,55:0A2463,100:020024&height=110&section=footer"/>
</p>
