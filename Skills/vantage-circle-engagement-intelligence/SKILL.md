---
name: vantage-circle-engagement-intelligence
description: Analyzes market trends and employee engagement challenges across Reddit, LinkedIn, and research. Use to identify pain points, emerging trends, and content opportunities for Vantage Circle. Outputs monthly challenge maps, business case language, and content calendar recommendations.
---

# Vantage Circle Engagement Intelligence Skill

Extract market insights from Reddit discussions, LinkedIn posts, and third-party research to identify what HR/recognition leaders are struggling with. Use these insights to inform your content strategy, positioning, and engagement efforts.

## 1. Domain Knowledge

This skill synthesizes data from three sources:

- **Reddit:** Organic, unfiltered discussions from HR leaders asking real questions
- **LinkedIn:** Professional discourse, executive thought leadership, business case framings
- **Research:** Third-party authority (Gartner, Forrester, McKinsey) on trends and ROI

**Key principle:** Reddit tells you what problems exist. LinkedIn tells you how to talk about them. Research tells you why they matter and what's coming next.

---

## 2. Core Workflows

### Workflow 1: Reddit Community Mining for Pain Points

**When to use:** Monthly to identify recurring challenges in target communities.

**Step-by-step:**

1. **Select Communities**
   - Primary: r/humanresources (broadest HR audience)
   - Secondary: r/HRMS (technical HR)
   - Tertiary: r/startups (founder/culture audience)

2. **Define Time Window**
   - Last 30 days (monthly cycle)
   - Look for recurring themes across posts + comments

3. **Keyword Extraction**
   - Search for: "recognition," "engagement," "retention," "culture," "employee appreciation"
   - Cluster keywords into pain points
   - Track frequency (how often mentioned?)
   - Track sentiment (problem or solution discussion?)

4. **Pain Point Identification**
   - **Recognition adoption** — "People don't use our recognition program"
   - **Recognition fatigue** — "Recognition feels corporate/fake"
   - **Engagement measurement** — "How do we measure engagement impact?"
   - **Retention correlation** — "Does recognition actually reduce turnover?"
   - **Budget justification** — "How do we prove ROI to finance?"
   - **Implementation challenges** — "Best practices for rolling out new program?"
   - **Culture scaling** — "How to maintain culture as we grow?"
   - **Employee burnout** — "Retention is broken; people are burning out"

5. **Frequency Analysis**
   - Rank pain points by how often they appear
   - Note if frequency is increasing or decreasing (trend signal)
   - Identify seasonal variations (e.g., recognition discussions spike before holidays)

6. **Solution Gap Mapping**
   - For each pain point: What are people already trying?
   - What solutions are working?
   - What's missing or not working well?
   - Where's the gap Vantage Circle can fill?

**Output:**
```
Reddit Community Mining Report - [MONTH]

TOP PAIN POINTS (Ranked by frequency):
1. Recognition adoption (34% of posts mention) — Trend: ↑ increasing
   - Solution attempts: "Make it simpler," "Tie to values"
   - Gaps: No clear adoption framework; most solutions reactive
   - VC fit: HIGH (adoption is VC's strength)

2. Recognition authenticity (28% of posts) — Trend: ↑ stable
   - Solution attempts: "Peer-to-peer," "Tie to company culture"
   - Gaps: Struggling to make it feel non-corporate
   - VC fit: HIGH (peer recognition is VC's focus)

3. Engagement measurement (22% of posts) — Trend: ↓ declining
   - Solution attempts: Surveys, engagement scores, pulse checks
   - Gaps: Linking engagement to business outcomes
   - VC fit: MEDIUM (VC shows correlation, not causation alone)

4. [Continue for top 10 pain points]
```

---

### Workflow 2: LinkedIn Trend & Language Analysis

**When to use:** Monthly to understand how professionals frame and discuss these challenges.

**Step-by-step:**

1. **Identify Trending HR/Recognition Topics**
   - Search LinkedIn for: #HRtech, #EmployeeEngagement, #RecognitionCulture, #CultureFirst
   - Find top posts (1K+ likes, 100+ comments) from last 30 days
   - Extract post topics, themes, messaging

2. **Language Pattern Extraction**
   - What words do they use for problems?
     - "Disengaged employees," "retention crisis," "burnout," "quiet quitting"
     - vs. Positive: "culture," "recognition," "belonging," "purpose"
   - What resonates with audiences?
     - Numbers: "27% higher retention," "3x engagement lift"
     - Stories: Case studies, employee testimonials
     - Principles: "Culture eats strategy," "People stay for people"

3. **Business Case Framing**
   - How do thought leaders justify investment in employee programs?
   - What ROI language works?
     - "X investment → Y retention improvement → $Z savings"
     - "Culture metric A → Business metric B → Revenue impact C"
   - How do they tie HR to business outcomes?

4. **Competitor Content Monitoring**
   - What are Lattice, 15Five, Culture Amp, HiBob posting about?
   - Which posts get most engagement?
   - What messaging angles do they use?

5. **Emerging Trends**
   - What's being discussed now that wasn't 6 months ago?
   - (E.g., "AI for recognition," "Gen Z engagement," "remote team recognition")

**Output:**
```
LinkedIn Trend Analysis - [MONTH]

TOP TRENDING TOPICS:
1. "Recognition culture" (trending ↑) — 2,400+ posts, avg engagement 8%
   - Top performing angle: Story + metrics ("How we built recognition culture from scratch")
   - Language that works: "authentic," "peer-to-peer," "scale," "culture-first"
   - VC positioning: Emphasize peer recognition + culture angle

2. "Retention ROI" (trending ↑) — 1,800+ posts, avg engagement 6%
   - Top performing angle: Business case ("What's the ROI of recognition program?")
   - Language that works: Numbers, savings, retention %, turnover reduction
   - VC positioning: Show specific retention improvements from VC customers

3. [Continue for top 5-10 trending topics]

BUSINESS CASE LANGUAGE THAT WORKS:
- "X% reduction in voluntary turnover = $Y savings in hiring costs"
- "Recognition culture improves engagement by Z points"
- "Culture investment of $A → Revenue impact of $B (ROI: X:1)"

EMERGING TRENDS (6-12 month outlook):
- AI-powered recognition personalization
- Remote team recognition (bigger challenge post-WFH shift)
- Gen Z expects frequent, authentic recognition (not annual awards)
- ESG + culture alignment (recognition tied to company values)
```

---

### Workflow 3: Third-Party Research Integration

**When to use:** Quarterly or when research reports are published.

**Step-by-step:**

1. **Source Research**
   - Gartner: HR Tech trends, culture assessments
   - Forrester: Employee engagement market trends
   - McKinsey: Future of work, employee experience studies
   - ADP Research Institute: Engagement & retention trends
   - Mercer, Deloitte: Total rewards reports
   - LinkedIn Workplace Report: Engagement trends
   - Company reports: Vantage Circle, Lattice, Culture Amp whitepapers (if public)

2. **Extract Key Findings**
   - What % of companies do X? (benchmark)
   - What's the ROI of Y? (business case)
   - What's emerging in Z? (future trends)

3. **ROI & Business Case Data**
   - Recognition impact on retention: (e.g., "Companies with strong recognition culture have 22% lower turnover")
   - Engagement correlation: (e.g., "Engaged employees are 17% more productive")
   - Cost of turnover: (e.g., "Replacing employee costs 50-200% of annual salary")
   - Recognition budget vs. ROI: (e.g., "1% investment in recognition = 2-3% turnover reduction")

4. **Trend Outlook**
   - Gartner: What HR tech will be critical in 2026-2027?
   - Emerging needs companies are addressing now?

**Output:**
```
Third-Party Research Summary - [MONTH/QUARTER]

KEY STATISTICS:
- 72% of companies say employee recognition is important (Gallup)
- Companies with strong peer recognition have 21% lower turnover (ADP Research)
- Every 1% improvement in engagement = 2-3% improvement in retention (Mercer)
- Cost of replacing one employee: 50-200% of annual salary (Society for HR Management)

ROI BENCHMARKS:
- Recognition program investment: Typically 0.5-1% of payroll
- Expected return: 2-5% turnover reduction = $X savings
- Engagement ROI: 2-3 points improvement on 10-point scale within 6-12 months

EMERGING TRENDS (Gartner, Forrester, McKinsey):
1. Culture is the new competitive advantage (post-WFH)
2. Real-time, peer-driven recognition (vs. annual awards)
3. Recognition tied to company values/ESG goals
4. Personalization at scale (AI-assisted recognition)
5. Remote + hybrid team recognition challenges

VANTAGE CIRCLE POSITIONING INSIGHTS:
- Focus on peer-recognition ROI (highest impact, most unique positioning)
- Emphasize "culture-first" vs. "compliance-first" (differentiator)
- Lead with retention impact, then engagement, then business case
```

---

### Workflow 4: Integrated Challenge Map

**When to use:** Monthly to synthesize all sources and create actionable strategy.

**Step-by-step:**

1. **Synthesize Data**
   - Combine Reddit pain points + LinkedIn trends + research data
   - Create master list of challenges facing HR/recognition leaders

2. **Create Challenge Matrix**
   - For each challenge: frequency, growth trend, research support, Vantage Circle fit
   - Score on: Frequency (how often mentioned?), Intensity (how urgent?), Growth (is it trending?), VC fit (how well positioned?)

3. **Rank by Opportunity**
   - High frequency + High VC fit = TOP OPPORTUNITY (post about this)
   - High frequency + Medium VC fit = OPPORTUNITY (can address, need good framing)
   - Low frequency + High VC fit = NICHE OPPORTUNITY (expert position, low volume)
   - Low frequency + Low VC fit = SKIP (not a priority)

4. **Extract Content Calendar**
   - For each top opportunity: Generate 2-3 post ideas
   - Suggest timing (is it seasonal? is it trending now?)
   - Suggest format (authority post, case study, comparison, advice thread)

5. **Identify Positioning Angle**
   - For each challenge: How should Vantage Circle uniquely address it?
   - What's the messaging angle?
   - What's the proof point?

**Output:**
```
MONTHLY CHALLENGE MAP - [MONTH]

TIER 1 OPPORTUNITIES (Top Content Focus):

Challenge 1: RECOGNITION ADOPTION (Frequency: 34%, Trend: ↑, VC Fit: HIGHEST)
- Problem: "We launched recognition program but adoption is only 20%"
- Current solutions: Gamification, incentives, manager mandates
- Gap: No clear adoption framework; most companies reactive
- VC positioning: Peer recognition + minimal friction = 60%+ adoption in 90 days
- Research support: ADP shows peer recognition 3x higher adoption than top-down
- Content ideas:
  * Authority post: "Why recognition adoption fails (and 3-part framework that works)"
  * Case study: "From 20% to 65% adoption in 90 days (here's what we did)"
  * Comment response: [Framework for adoption challenges]
- Timing: Post ASAP (high search intent, evergreen)
- Expected engagement: HIGH (commonly discussed pain)

Challenge 2: ENGAGEMENT MEASUREMENT (Frequency: 22%, Trend: ↓, VC Fit: MEDIUM)
- Problem: "How do we measure if our recognition program actually drives engagement?"
- Current solutions: Engagement surveys, pulse checks, internal metrics
- Gap: Hard to tie to business outcomes; causation unclear
- VC positioning: Show correlation between recognition, engagement, and retention
- Research support: McKinsey shows 17% productivity lift from engagement; VC shows recognition is driver
- Content ideas:
  * Authority post: "How to measure recognition ROI (the business case method)"
  * Thought leadership: "Why engagement scores alone are misleading"
  * Case study: "Recognition → Engagement ↑ → Retention ↑ → Revenue impact"
- Timing: Q2, Q3 (budget planning cycles; finance wants ROI)
- Expected engagement: MEDIUM (more technical, less universal)

[Continue for top 10 challenges]

SEASONAL OPPORTUNITIES:
- January: Culture reset, engagement planning ("How to build recognition culture in 2026")
- March-April: Q1 reviews, budget planning ("Tying recognition to Q1 goals")
- July-August: Summer retention ("Retention crisis: how recognition helps")
- Oct-Nov: Benefits season prep ("Recognition as part of total rewards")

VANTAGE CIRCLE POSITIONING SUMMARY:
- Lead message: "Recognition culture scales through peer-to-peer, not top-down"
- Support: Research + case studies showing 60%+ adoption, 15-20% turnover reduction
- Differentiation: Culture-first positioning vs. compliance-first (vs. traditional HRIS)
- Proof points: Customer stories, retention metrics, engagement improvements
```

---

## 3. Workflow Trigger Phrases

- "Extract Reddit pain points for Q2" → Workflow 1: Reddit Community Mining
- "What's trending on LinkedIn for HR this month?" → Workflow 2: LinkedIn Trend Analysis
- "Summarize the latest research on engagement ROI" → Workflow 3: Research Integration
- "Build me a monthly challenge map" → Workflow 4: Integrated Challenge Map
- "What should I post about this month?" → Workflow 4 + output (feeds into content calendar)

---

## 4. Success Metrics

✅ Identifies 10+ specific pain points with quantified frequency (e.g., "34% of r/humanresources posts mention recognition adoption")
✅ Surfaces 3-5 gap opportunities for Vantage Circle to exploit
✅ Outputs actionable monthly insights (content calendar, positioning recommendations)
✅ Reduces time to identify posting topics from 2 hours to 15 minutes
✅ Content strategy informed by data, not guessing

---

## 5. Integration with Other Skills

- **Output feeds to:** Skill 2 (SaaS Post Template Analysis — knows which topics to analyze)
- **Output feeds to:** Skill 3 (Authority Strategy — informs monthly content calendar)
- **Output feeds to:** Skill 0 (Reddit Marketing — knows what to post about + positioning)

---

## 6. Data Sources Reference

See `references/data-sources.md` for:
- Reddit communities to monitor
- LinkedIn search queries
- Research reports and where to find them
- Competitor accounts to monitor

See `templates/monthly-challenge-map.md` for:
- Templated output format
- How to rank and prioritize challenges
- Content ideas generation template

---

## 7. Monthly Workflow

1. Run Workflow 1 (Reddit mining) — 30 min
2. Run Workflow 2 (LinkedIn trends) — 20 min
3. Run Workflow 3 (Research) — 15 min (if new reports available)
4. Run Workflow 4 (Integrated map) — 15 min
5. **Total time: 60-80 minutes → Output: Month's content strategy**

Then pass output to Skill 2 (Template Analysis) and Skill 3 (Authority Strategy) for execution.
