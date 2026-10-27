# Arrey Etta

Software engineer and designer in Yaoundé, Cameroon, working remotely. I build AI products end to end: the model calls and data pipelines, the interface, the payments, and the emails that bring people back.

### Building: Arkoo Autopilot

[Arkoo](https://arkoojobs.com) is a job-search product, and its core is **Autopilot**: an AI agent that runs a candidate's job search end to end. On a schedule it picks the roles worth applying to and writes a tailored CV and cover letter for each. Then it opens the employer's real application in a cloud browser, fills every field, checks its own work, submits, and sends the candidate a receipt.

- **Plans.** It reads postings from 24 sources, from Greenhouse, Ashby and Lever boards to YC's Work at a Startup and VC portfolio boards. It rules out jobs the candidate can't legally be hired for, then scores the shortlist with a fast decision model that answers typed questions with a confidence, for a fraction of a cent per posting. It applies to the best matches within daily and per-company limits.
- **Writes.** For every job it tailors the CV and cover letter, and drafts answers to open-ended questions from the candidate's own CV and past answers. A fabrication guard throws out any draft that states a number the candidate's material doesn't contain.
- **Acts in a real browser.** Each application runs in a [Browser Use](https://browser-use.com) cloud browser driven by Playwright. An injected form engine ([open source](https://github.com/jordan-ae/ats-form-fill)) reads and fills Greenhouse, Ashby and Lever forms. A navigator follows Apply links from job boards through to the employer's own form.
- **Doesn't invent facts.** Work authorisation, salary and notice period come only from what the candidate has stored; the model maps questions and options, never the facts. Every answer it writes goes into an answer bank, and the candidate's corrections are what it uses next time.
- **Checks before it submits.** Thirteen gates run on the live page before a single press of submit, including read-back of every field, the right CV attached, trap wording, eligibility and budget. Anything that fails goes to a review queue, and every submission leaves a receipt with a screenshot.

Autopilot is in private pilot. The same engine powers a Chrome extension for candidates who'd rather press submit themselves.

### Also built

- **[Pheme](https://phemesh.vercel.app)**: a shared memory layer for AI coding agents. Decisions and constraints live with the project in Postgres and pgvector, and every agent reads and writes them over MCP or REST.
- **[arrey-cli](https://github.com/jordan-ae/arrey)**: installs AI tools into your project as editable source code, the way shadcn/ui does for components. Published on npm.

### Open source

I've contributed to [Stakwork](https://github.com/stakwork): the bounty planner and Hive chat in [sphinx-tribes-frontend](https://github.com/stakwork/sphinx-tribes-frontend), plus [sphinx-nav-fiber](https://github.com/stakwork/sphinx-nav-fiber) and [hive](https://github.com/stakwork/hive).

### Stack

TypeScript · React / Next.js · React Native · Node · Supabase / Postgres · AWS · Cloudflare · LLM APIs

### Elsewhere

[arrey.codes](https://arrey.codes) · [Writing](https://substack.com/@arreyetta/posts) · [LinkedIn](https://www.linkedin.com/in/arrey-etta-24530b1a2/)
