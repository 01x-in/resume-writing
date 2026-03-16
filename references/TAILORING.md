# Resume Tailoring Workflow

## How to tailor a resume for a specific job description.

---

## Step 1: Analyze the Job Description

Extract the following from the JD:

1. **Company name and role title**
2. **Role type classification:** Engineering Manager / Staff Engineer / Senior IC / Architect / Hybrid
3. **Requirements ranked by importance (1-10):**
   - Count keyword frequency — a skill mentioned 5 times is more important than one mentioned once
   - Distinguish must-haves (listed under "Required") from nice-to-haves ("Preferred")
   - Weight the first 3 bullets of any requirements list higher — they're listed in priority order
4. **Domain/industry context** — healthcare, fintech, e-commerce, etc.
5. **Team context** — team size, reporting structure, cross-functional collaboration signals
6. **Cultural signals** — startup vs. enterprise, move-fast vs. process-heavy, remote vs. onsite

### Output Format

```
Role: [Title] at [Company]
Type: [EM / Staff / IC / Architect]
Location: [City / Remote / Hybrid]

Top Requirements (weighted):
1. [Skill/requirement] — Priority: 9/10 — Evidence: mentioned 4x, listed first
2. [Skill/requirement] — Priority: 8/10 — Evidence: in "must have" section
3. [Skill/requirement] — Priority: 7/10 — Evidence: mentioned 2x
...

Must-Haves: [list]
Nice-to-Haves: [list]
Domain: [industry]
Team Size: [if mentioned]
```

---

## Step 2: Map Your Experience

For each top requirement, identify:

1. **Direct match:** A bullet in your resume that directly demonstrates this skill with metrics
2. **Partial match:** Experience that's related but needs reframing to highlight the relevant aspect
3. **Gap:** No matching experience — need a framing strategy

### Framing Strategies for Gaps

When you lack direct experience in a required area:

- **Adjacent experience:** Frame related work that uses similar skills. E.g., if they want Kubernetes and you've done Docker + ECS, frame it as "container orchestration experience" and mention your Docker/ECS depth.
- **Project experience:** Side projects, open-source, or advisory work that covers the gap.
- **Learning signal:** Recent certifications, courses, or self-directed learning in the area.
- **Transferable framing:** Emphasize the underlying principle rather than the specific tool. E.g., "designed event-driven architectures" covers Kafka even if you used RabbitMQ.
- **Honest omission:** If the gap is real and significant, don't fabricate. Focus on your strengths and address the gap in the cover letter as an area of active development.

---

## Step 3: Tailor the Summary

Rewrite the professional summary to:

1. Mirror the role's title and level in your opening identity statement
2. Include the domain/industry context from the JD
3. Front-load the 1-2 metrics that align with their top requirements
4. Use terminology from the JD (ATS matching)

**Example — Original summary:**
> Engineering Manager with 10+ years in backend development. Led teams building APIs and cloud infrastructure.

**Example — Tailored for a fintech EM role:**
> Engineering Manager with 10+ years building real-time financial systems. Led a team of 12 engineers to deliver a payment processing platform handling $500M+ in annual transactions. Deep expertise in distributed systems (Kafka, gRPC), regulatory compliance (PCI-DSS), and scaling teams through hypergrowth.

The tailored version mirrors the JD's language (fintech, real-time, compliance) and front-loads relevant metrics.

---

## Step 4: Reorder Skills Section

1. Take the JD's top requirements
2. Reorder your skills section so the highest-priority skills appear first
3. Use the exact same terminology the JD uses (e.g., if they say "CI/CD" don't write "continuous integration and deployment")
4. Add any skills from the JD that you have but hadn't listed
5. Remove skills that are irrelevant to this role (keep the section focused)

---

## Step 5: Reorder and Rewrite Experience Bullets

For each role on your resume:

1. **Reorder bullets** — put the most JD-relevant bullet first, not chronologically or by impressiveness. The first bullet under each role is what the recruiter reads. Make it count.
2. **Rewrite for emphasis** — if a bullet covers a required skill but buries it, rewrite to front-load the relevant aspect.
3. **Adjust sub-categories** — if the role is EM-type, lead with Team Impact. If Staff/IC, lead with Technical Leadership.
4. **Cut irrelevant bullets** — if a bullet doesn't serve this application and space is tight, remove it.

**Example — Original bullet:**
> Built REST APIs for the billing system using Django and PostgreSQL.

**Tailored for a role emphasizing scalability:**
> Designed and scaled billing APIs handling 50,000+ daily transactions with sub-200ms response times, implementing connection pooling and query optimization (Django, PostgreSQL, Redis).

Same experience, different framing — emphasizing the aspect the JD cares about.

---

## Step 6: Adjust Projects Section

If you have a projects/side-projects section:

1. Reorder projects so the most JD-relevant appears first
2. Rewrite project descriptions to emphasize skills the JD requires
3. Consider adding a project that covers a gap in your work experience

---

## Step 7: Run the Quality Checklist

After tailoring, run the full Quality Checklist from SKILL.md to ensure no anti-patterns were introduced during rewriting.

---

## Step 8: Generate Cover Letter (Optional)

If a cover letter is requested or recommended, read `COVER_LETTERS.md` for the full workflow. The tailored resume + JD analysis provide all the inputs needed.

---

## Time Target

A complete tailoring pass (Steps 1-7) should take under 15 minutes when using the modular resume strategy. If starting from scratch, allow 30-45 minutes.
