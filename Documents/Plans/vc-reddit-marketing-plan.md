# Reddit Marketing Skill for Vantage Circle

## Context

**Problem:** Deepmani needs to manage Vantage Circle's Reddit marketing effort efficiently — currently responsible for 100% of Reddit strategy, community building, authority posts, and lead generation to meet MQL targets.

**Goal:** Build a custom Claude Code skill that helps with Reddit content strategy, post creation, community analysis, and lead qualification — automating repetitive tasks while maintaining authenticity and community fit.

**Why a skill?** As a custom Claude Code skill (not generic tool), this becomes a reusable `/reddit` command that can:
- Generate campaign-specific Reddit content aligned with Vantage Circle brand
- Analyze subreddit communities and identify high-intent lead opportunities
- Create post templates for different content types (authority posts, case studies, troubleshooting)
- Track engagement and MQL-relevant metrics
- Suggest content ideas based on HR/HRMS pain points

---

## Implementation Plan

### Phase 1: Skill Structure & Core Workflows

**Files to create:**
- `vantage-circle-reddit.skill` — Main skill manifest (JSON/YAML)
- `SKILL.md` — Skill documentation with workflows

**Skill capabilities (5 core workflows):**

1. **Subreddit Analysis** — Research target subreddits (r/humanresources, r/HRMS, r/startup, etc.)
   - Find relevant communities by audience & topic
   - Extract community rules, posting guidelines, audience size
   - Identify posting patterns and engagement rates
   - Flag communities where Vantage Circle can build authority

2. **Authority Post Generation** — Create high-value, lead-friendly content
   - Format: Thought leadership on HRMS trends, employee retention, recognition strategies
   - Inputs: Topic, pain point, target audience tier
   - Output: Reddit-optimized post (title, body, CTAs that fit Reddit norms)
   - Tone: Helpful expert, not salesy (critical for Reddit authenticity)

3. **Case Study Adaptation** — Adapt existing Vantage Circle case studies for Reddit
   - Inputs: Client industry, problem solved, metrics achieved
   - Output: Formatted as Reddit case study post (question format for r/humanresources AMA threads)
   - Preserve anonymity while highlighting results

4. **Lead Qualification Checker** — Identify high-intent comments/DMs in Reddit discussions
   - Pattern matching: pain points that match Vantage Circle's solution
   - Flag engagement opportunities (responses to posts, DMs from prospects)
   - Suggest follow-up messaging aligned with community norms

5. **Content Calendar & Topic Ideas** — Generate Reddit-specific campaign ideas
   - Monthly themes aligned with HR calendar (benefits season, Q1 planning, retention challenges)
   - Weekly topic suggestions based on Reddit trends + Vantage Circle expertise
   - Cross-link to LinkedIn content strategy for repurposing

---

### Phase 2: Knowledge Base & References

**Files to create:**

1. **`references/reddit-communities.md`** — Target subreddit index
   - List: r/humanresources, r/HRMS, r/startups, r/smallbusiness, r/recruiting, r/management
   - For each: audience profile, posting guidelines, content that works, typical engagement rates
   - Vantage Circle fit analysis (where authority can be built vs. where it's too commercial)

2. **`references/reddit-best-practices.md`** — Reddit posting dos/don'ts
   - Authenticity rules (no overly promotional content; build genuine value first)
   - Engagement patterns (best times to post, comment structure, AMA best practices)
   - MQL-friendly CTAs (soft-sell approaches: "Happy to answer questions," resource sharing)
   - When to use r/humanresources vs. comments in r/startup vs. direct outreach

3. **`references/vantage-circle-positioning.md`** — Vantage Circle messaging for Reddit
   - Core value props: Employee retention, recognition culture, HRMS simplification
   - Pain points Vantage Circle solves: Low engagement, recognition fatigue, HR admin burden
   - Credential building: Team expertise in HRMS, employee psychology, culture strategy
   - Competitive angles (vs. traditional HRMS, vs. DIY recognition programs)

4. **`templates/`** — Post templates for common content types
   - `authority-post-template.txt` — Structure for thought leadership
   - `case-study-template.txt` — Format for anonymized success story
   - `comment-response-template.txt` — How to reply helpfully without hard-selling
   - `ama-prep.txt` — AMA (Ask Me Anything) question prep + response strategy

---

### Phase 3: Workflow Logic & Decision Trees

**Built-in workflows will include:**

- **When user says "Create a Reddit post about X":**
  1. Analyze topic against Vantage Circle's HRMS focus
  2. Suggest 3 best subreddits for this content
  3. Check community rules + tone guidelines
  4. Generate title options (with Reddit-specific formatting tips)
  5. Write post body (authentic, helpful, naturally mentions Vantage Circle if relevant)
  6. Suggest best posting time + engagement strategy

- **When user says "Analyze r/humanresources for opportunities":**
  1. Pull community stats (subscriber count, posting frequency, top posts)
  2. Identify pain points in recent discussions
  3. Flag Vantage Circle-relevant threads
  4. Recommend content angles that would resonate
  5. Suggest engagement calendar

- **When user says "Help me respond to this Reddit comment":**
  1. Understand the commenter's problem/context
  2. Suggest response approach (helpful, credible, non-promotional)
  3. If lead-qualified: Flag for outreach; suggest soft landing page
  4. Generate response options: expert answer + light resource mention

---

### Phase 4: Integration with Existing Systems

**Connection points:**
- **LinkedIn case studies** → Adapt for Reddit anonymized format
- **Vantage Circle creative skill** — Link to brand guidelines (even though Reddit is text-focused, understanding brand voice matters)
- **MQL tracking** — Add fields for tracking leads sourced from Reddit
- **Content calendar** — Align Reddit schedule with LinkedIn + Twitter posting rhythm

---

## Critical Files to Modify/Create

| File | Purpose | Status |
|------|---------|--------|
| `vantage-circle-reddit.skill` | Main skill manifest | Create new |
| `SKILL.md` | Workflow documentation | Create new |
| `references/reddit-communities.md` | Target subreddit research | Create new |
| `references/reddit-best-practices.md` | Community etiquette + strategy | Create new |
| `references/vantage-circle-positioning.md` | Brand messaging for Reddit | Create new |
| `templates/authority-post-template.txt` | Content template | Create new |
| `templates/case-study-template.txt` | Case study format | Create new |
| `templates/comment-response-template.txt` | Reply strategy | Create new |
| `templates/ama-prep.txt` | AMA preparation guide | Create new |

---

## Verification & Testing

**How to test the skill:**

1. **Workflow 1 — Authority Post Generation:**
   - Input: "Create a Reddit post about combating employee recognition fatigue"
   - Expected: Post title (Reddit-formatted), body text, 2-3 subreddit suggestions, engagement tips
   - Validation: Post reads authentic (not salesy), includes subtle positioning, follows r/humanresources norms

2. **Workflow 2 — Subreddit Analysis:**
   - Input: "Analyze r/humanresources for lead opportunities"
   - Expected: Community overview, recent pain points, top post themes, Vantage Circle fit assessment
   - Validation: Insights are actionable; tie back to employee retention/recognition themes

3. **Workflow 3 — Case Study Adaptation:**
   - Input: "Adapt the XYZ company case study for Reddit (anonymized)"
   - Expected: Formatted as Reddit case study, anonymized company, metrics highlighted
   - Validation: Anonymity preserved; results credible without over-claiming

4. **Workflow 4 — Lead Qualification:**
   - Input: "This commenter mentioned 'our recognition program is stale—need something modern'"
   - Expected: Flagged as high-intent; suggested response; MQL-ready contact suggestion
   - Validation: Flags are accurate; responses don't feel spammy

---

## Success Criteria

✅ Skill reduces time to research + write Reddit posts from 1-2 hours to 30 mins  
✅ Generated posts maintain authenticity (Reddit upvotes/engagement validates this)  
✅ Skill helps identify 2-3 high-intent Reddit leads per month  
✅ Content calendar integrates with existing LinkedIn strategy  
✅ Team uses skill weekly for content ideation + response strategy  

---

## Next Steps (After Planning)

1. **Write SKILL.md** with 5 detailed workflows
2. **Create reference docs** (subreddit guide, best practices, positioning)
3. **Build post templates** for common content types
4. **Package as .skill file** (compatible with Claude Code's skill format)
5. **Test with real Reddit research** before deployment
