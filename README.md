# Arrey Etta

Software engineer and designer in Yaoundé, Cameroon, working remotely. I build AI products end to end: the model calls and data pipelines, the interface, the payments, and the emails that bring people back.

### Building: Arkoo

[Arkoo](https://arkoojobs.com) is a job-search product built around **Autopilot**, an agent that finds roles that fit, tailors the CV and cover letter for each one, and fills in the employer's own application form.

- **Sourcing.** A daily pipeline reads 24 sources, including Greenhouse, Ashby, Lever, SmartRecruiters, Workable, YC's Work at a Startup and boards found through VC portfolios. It scores each listing's quality and retires dead ones.
- **Deterministic first.** A DOM-only fill engine ([open source](https://github.com/jordan-ae/ats-form-fill)) reads, fills and reads back Greenhouse, Ashby and Lever forms, and ATS APIs cover more. That's about 89% of postings with no LLM in the loop. The model only maps unfamiliar questions and drafts open-ended answers.
- **No invented facts.** Work authorisation, salary, notice period and similar answers come only from what the user has stored. The model can match a stored value to a form's option, but it never picks the value. Every draft it writes is saved for the user to correct.
- **Gated submission.** Thirteen checks run on the live page before a single submit press: trap wording, field read-back, the tailored CV attached, per-company caps and budget. Anything that fails goes to a review queue. Autopilot is in private pilot.

The same fill code runs in a Chrome extension for people who'd rather press submit themselves.

### Also built

- **[Pheme](https://github.com/jordan-ae/Pheme)**: a shared memory layer for AI coding agents. Decisions and constraints live with the project in Postgres and pgvector, and every agent reads and writes them over MCP or REST.
- **[arrey-cli](https://github.com/jordan-ae/arrey)**: installs AI tools into your project as editable source code, the way shadcn/ui does for components. Published on npm.

### Open source

I've contributed to [Stakwork](https://github.com/stakwork): the bounty planner and Hive chat in [sphinx-tribes-frontend](https://github.com/stakwork/sphinx-tribes-frontend), plus [sphinx-nav-fiber](https://github.com/stakwork/sphinx-nav-fiber) and [hive](https://github.com/stakwork/hive).

### Stack

TypeScript · React / Next.js · React Native · Node · Supabase / Postgres · AWS · Cloudflare · LLM APIs

### Elsewhere

[arrey.codes](https://arrey.codes) · [Writing](https://substack.com/@arreyetta/posts) · [LinkedIn](https://www.linkedin.com/in/arrey-etta-24530b1a2/)
