<img src="assets/hero.svg" width="100%" alt="Chaitanya Srivastava, backend developer. Based in Jamshedpur, studying B.Tech IT at VIT Vellore 2024–28, works with Node.js, Express, PostgreSQL and Redis."/>

<p align="center">
  <a href="https://www.linkedin.com/in/chaitanya-srivastava-904473300/">LinkedIn</a>
  &nbsp;/&nbsp;
  <a href="mailto:srivastavachaitanya408@gmail.com">Email</a>
  &nbsp;/&nbsp;
  <a href="https://leetcode.com/u/chaitanya0111/">LeetCode</a>
  &nbsp;/&nbsp;
  <a href="tel:+919798864033">+91 97988 64033</a>
</p>

<img src="assets/statement.svg" width="100%" alt="Statement of work: B.Tech IT at VIT Vellore from Jul 2024; Software Development Intern at KalkiNi from Aug 2025; Intern at Tata Steel from May 2026; built Wallet Ledger in 2026; now learning system design, AWS, Docker and distributed systems."/>

<a href="https://github.com/code0101cs/Wallet-Ledger"><img src="assets/wallet-ledger.svg" width="100%" alt="Wallet Ledger: a double-entry payments API in Node.js and PostgreSQL with row-level locking and idempotency keys."/></a>

<a href="https://github.com/code0101cs/PaperStreets"><img src="assets/paper-streets.svg" width="100%" alt="Paper Streets: a backtester for moving-average crossover and buy-and-hold strategies on historical stock data."/></a>

<br/>

<details>
<summary><b>How a transfer moves through Wallet Ledger</b></summary>
<br/>

Every transfer runs inside one PostgreSQL transaction. The sender's wallet row is locked first, so two transfers from the same account queue up instead of racing each other to spend the same balance.

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'IBM Plex Sans, Helvetica, Arial','primaryColor':'#0B1A33','primaryTextColor':'#E7EEFA','primaryBorderColor':'#2E6BE6','lineColor':'#5B9BFF','actorBkg':'#0B1A33','actorTextColor':'#E7EEFA','actorBorder':'#2E6BE6','actorLineColor':'#2E6BE6','signalColor':'#5B9BFF','signalTextColor':'#4C7FD6','noteBkgColor':'#0B1A33','noteTextColor':'#E7EEFA','noteBorderColor':'#2E6BE6','labelBoxBkgColor':'#0B1A33','labelBoxBorderColor':'#2E6BE6','labelTextColor':'#E7EEFA','loopTextColor':'#4C7FD6'}}}%%
sequenceDiagram
    participant C as Client
    participant A as Auth middleware
    participant T as Transfer controller
    participant DB as PostgreSQL
    C->>A: POST /transfer with JWT and Idempotency-Key
    A->>T: Verified user
    T->>DB: BEGIN
    T->>DB: Check the idempotency key is unused
    T->>DB: SELECT wallet FOR UPDATE
    T->>DB: Sum entries to get the balance
    alt Enough balance
        T->>DB: Insert transaction, DEBIT entry, CREDIT entry
        T->>DB: COMMIT
        T-->>C: Transfer posted
    else Not enough balance
        T->>DB: ROLLBACK
        T-->>C: Insufficient funds
    end
```

Balance is always `SUM(credits) - SUM(debits)` over the entries table. There is no balance column that could drift out of sync.

</details>

<details>
<summary><b>The internships in detail</b></summary>
<br/>

**Intern, Tata Steel** <sub>May – Jun 2026, Jamshedpur, on-site</sub>

Worked on two internal .NET applications running on Oracle. Migrated jQuery 1 to 3 and Bootstrap 3 to 4, and shipped feature work and bug fixes alongside.

**Software Development Intern, KalkiNi** <sub>Aug – Dec 2025, Vellore</sub>

Joined an AI surveillance startup in its initial stage. The most useful thing I learned there was how to read a codebase I didn't write, which turned out to be harder than writing new code.

</details>

<details>
<summary><b>What I'm learning right now</b></summary>
<br/>

| | |
|---|---|
| **System design** | Load balancing, horizontal scaling, and where the cache actually belongs |
| **AWS** | EC2, RDS, and getting IAM permissions right without opening everything up |
| **Docker and CI/CD** | So deploys stop being a manual process |
| **Security** | Looking at systems the way an attacker would |
| **Distributed systems** | Eventual consistency, and what breaks when a service stops responding |

</details>

<details>
<summary><b>Everything I work with</b></summary>
<br/>

| | |
|---|---|
| **Language** | JavaScript |
| **Backend** | Node.js, Express, REST APIs, MVC |
| **Data** | PostgreSQL, MongoDB with Mongoose, Redis |
| **Auth** | JWT, bcrypt, express-session |
| **Server-rendered UI** | EJS, HTML, CSS, Chart.js |
| **Tooling** | Git, Docker, Postman, Linux |

</details>

<details>
<summary><b>Other projects</b></summary>
<br/>

**[Authentication System](https://github.com/code0101cs/Authentication-System)** &nbsp;Password hashing, sessions and protected routes, built from scratch.

**[Expense Tracker](https://github.com/code0101cs/Expense_Tracker)** &nbsp;A server-rendered app for logging and reviewing expenses.

</details>

<details>
<summary><b>GitHub activity</b></summary>
<br/>

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=code0101cs&show_icons=true&include_all_commits=true&count_private=true&bg_color=0A192F&title_color=58A6FF&text_color=C9D6EA&icon_color=2E6BE6&border_color=1C3056&border_radius=12"/>
  <img height="165" src="https://streak-stats.demolab.com?user=code0101cs&background=0A192F&ring=2E6BE6&fire=5B9BFF&currStreakNum=E7EEFA&sideNums=E7EEFA&currStreakLabel=5B9BFF&sideLabels=8EA2C6&dates=8EA2C6&stroke=1C3056&border=1C3056&border_radius=12"/>
</p>

<p align="center">
  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=code0101cs&bg_color=0A192F&color=8EA2C6&line=5B9BFF&point=E7EEFA&area=true&area_color=2E6BE6&hide_border=true&radius=12"/>
</p>

</details>
