# resume-writing

A Claude Code skill for writing, reviewing, and tailoring high-impact resumes. Goes beyond keyword matching — applies proven resume strategy: ownership language, impact-first framing, role-type-specific structuring, and the 8-second recruiter scan test.

**This is not a template filler. It's a strategic writing system.**

---

## What It Does

- **Write a new resume** from scratch with strategic structure and impact-first bullets
- **Tailor an existing resume** to a specific job description with weighted requirement matching
- **Rewrite weak bullets** using the ownership bullet formula: `Action Verb → What You Did → Measurable Outcome → (Tech)`
- **Review and critique** any resume against a comprehensive quality checklist
- **Generate cover letters** that tell a narrative story, not just restate the resume
- **Guide formatting** for ATS compliance — fonts, layout, and anti-patterns

## Who It's For

Works across all experience levels and role types:

- **Early Career (0-3 years)** — Projects, internships, career objectives, one-page format
- **Senior / Staff Engineers** — Technical depth, cross-team influence, system-level impact
- **Engineering Managers** — Team impact, technical leadership, business outcomes
- **DevOps / Platform Engineers** — Infrastructure scale, developer experience, reliability
- **Career Changers** — Strategic reframing of existing experience for a different role type

---

## Install

### Claude Code

```bash
claude install-skill https://github.com/YOUR_USERNAME/resume-writing
```

Or manually drop the `resume-writing/` folder into your skills directory.

### Manual

Clone the repo and copy to your Claude Code skills location:

```bash
git clone https://github.com/YOUR_USERNAME/resume-writing.git
cp -r resume-writing ~/.claude/skills/
```

---

## Usage

Once installed, the skill triggers automatically when you mention resumes, CVs, job applications, cover letters, or career documents. Examples:

**Write a new resume:**
> "Help me write a resume. I'm a backend engineer with 6 years of experience targeting senior roles."

**Tailor for a job posting:**
> "Tailor my resume for this job description: [paste JD]"

**Rewrite a bullet:**
> "Rewrite this bullet to be more impactful: 'Responsible for maintaining backend services'"

**Review a resume:**
> "Review my resume and flag any issues"

**Generate a cover letter:**
> "Write a cover letter for the Staff Engineer role at Stripe based on my resume"

**Quick checklist:**
> "Run the quality checklist on my resume"

---

## What's Inside

```
resume-writing/
├── SKILL.md                        # Core skill — strategy, bullet formula, checklist
├── LICENSE.txt                     # MIT License
├── references/
│   ├── ROLE_GUIDES.md              # Detailed guidance per role type + experience level
│   ├── TAILORING.md                # Job-specific tailoring workflow (8 steps)
│   ├── COVER_LETTERS.md            # Cover letter structure and strategy
│   └── FORMATTING.md               # Fonts, ATS compliance, layout rules
└── templates/
    └── ats-clean.md                # Blank ATS-friendly resume template
```

**`SKILL.md`** loads every time the skill triggers. Contains the core philosophy, bullet formula, resume structure guide, quality checklist, 8-second scan test, and modular resume strategy.

**Reference files** load on demand — only when the specific task requires deeper guidance. This keeps the context lean for simple tasks (rewrite one bullet) while providing depth for complex ones (tailor a full resume to a JD).

---

## The Bullet Formula

Every resume bullet follows this pattern:

```
Action Verb → What You Did → Measurable Outcome → (Technology/Context)
```

**Before:**
> Responsible for backend systems and performance optimization.

**After:**
> Reduced P95 API latency from 4s to 200ms by resolving N+1 query patterns and implementing Redis caching (Django, PostgreSQL).

---

## Quality Checklist

The skill runs these checks before finalizing any resume:

- No bullets start with "Responsible for", "Assisted with", "Helped with"
- No bullets exceed 2 lines
- Every bullet contains at least one metric or number
- No generic phrases ("passionate", "results-driven", "team player")
- Summary is under 5 lines
- Consistent date formatting
- Every bullet starts with a strong action verb
- Technologies in skills section appear in experience bullets
- Top 3 achievements are in the top half of page 1

---

## The 8-Second Scan Test

Before any resume is finalized, it's validated against how recruiters actually read:

1. Can you see the candidate's level in 2 seconds?
2. Do numbers jump off the page?
3. Is career progression visible?
4. Are the strongest achievements in the top half of page 1?
5. Would a recruiter reading ONLY the first bullet of each role want to call?

---

## Contributing

PRs welcome. If you have resume insights from hiring experience, recruiter feedback, or proven strategies — open an issue or submit a PR to the relevant reference file.

Areas that could use community input:
- Role guides for additional functions (Product Manager, Data Engineer, Designer, etc.)
- Industry-specific tailoring advice (healthcare, fintech, defense, etc.)
- International resume conventions (EU, Asia, Middle East formatting differences)
- Additional templates

---

## License

MIT — see [LICENSE.txt](LICENSE.txt)

---

Built by [01x](https://01x.in) · [github.com/01x-in](https://github.com/01x-in)
