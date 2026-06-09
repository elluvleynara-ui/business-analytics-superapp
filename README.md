# SuperApp AI Agent — Banking SuperApp Concept

> A university Business Analytics project. We built an AI agent for a banking superapp that gives users a personalized life development plan — because all banking superapps look the same, and we wanted to change that.

**Live bot:** [@agent00_test_bot](https://t.me/agent00_test_bot)

---

## The idea

Our professor — a practicing business analyst — said something that stuck with me:

> *"All banking superapps in Kazakhstan are identical. If you want users to choose yours, you need to trigger something real in them."*

So we asked: what if the superapp didn't just hold your money, but actually helped you figure out what to do with your life?

The answer was an AI agent that talks to a user, understands their life stage and pain points, and gives them a concrete IDP — Individual Development Plan. Not motivational fluff. An actual plan with steps.

---

## What we built

### Telegram bot — [@agent00_test_bot](https://t.me/agent00_test_bot)

The bot launched and reached **961 users**, 82.5% of them aged 16–25, mostly students. It asks the user a few questions and generates a personalized development plan based on their life stage.

We didn't just launch and watch. We analyzed what happened:
- The initial trigger (external/automated) got people in the door
- Retention was low — users came but didn't come back
- Finance was the #1 declared interest (57.8% of users) but had the worst engagement — less than 10% actually interacted with financial features
- Career content had a CSAT of 88.6% — the highest in the whole product

That gap between what people say they want and what they actually engage with — that became the core insight for our second iteration strategy.

---

## What's in this repo

```
/docs
  ├── IDP_framework.pdf          — Life stage development plans (birth → career → family)
  ├── Target_audience_analysis.docx — Full analysis of 500 synthetic user profiles
  ├── Trigger_analysis.pdf       — Which triggers work and why (FOMO, procrastination, income)
  ├── AI_agent_strategy.pdf      — UVP, engagement loops, retention mechanics

/data
  └── synthetic_audience.xlsx    — 500+ synthetic profiles segmented by life stage
                                   Sheets: Base data, Age 16, Pregnancy, Birth,
                                   Childhood (0–6), School, University,
                                   Work & Career, Family & Adult life, OKR
```

---

## My part — IDP module

I worked in the **IDP team**. Our job was to design the development plan logic — what the agent actually tells a person based on their life stage.

We broke life into 9 stages and for each one defined:
- Key risks (medical, financial, regional, social)
- Action plan
- KPIs to track progress

| Life stage | Core focus |
|---|---|
| Base profile | Language, digital literacy, legal status |
| School | Academic performance, digital skills, career direction |
| University | Practical experience, portfolio, career planning |
| Work & Career | Skill growth, income stability, promotion path |
| Family & Adult life | Financial buffer, housing, work-life balance |
| Skills & Monetization | From skill to income — formats, niches, scaling |

The framework was designed to feed into the AI agent's recommendation engine — when a user describes their situation, the agent maps them to a life stage and generates relevant next steps.

---

## The data

We built a **synthetic audience database** of 500+ profiles covering residents of Kazakhstan from age 16 to 63 — manually structured by the team across multiple life stages.

Each profile includes demographic data, income level, digital literacy score, family structure, regional location, employment type, and NLP tags like `#has_car`, `#financial_pressure`, `#single_parent`.

This let us run real product analytics — segmentation, trigger analysis, CSAT breakdowns — on a realistic Kazakh population distribution (52% Kazakh-speaking, 48% Russian-speaking; 64% urban, 22% district centers, 14% rural).

---

## What we learned

**961 users is a real number**, but the more interesting number is the retention rate — which was low. We spent the second half of the project figuring out why, and the analysis pointed to three things:

1. The entry trigger (automation) attracted volume without intent
2. Financial features were broken — people wanted them but couldn't use them
3. The agent needed to give value in the first 2 minutes, not after onboarding

The fix we proposed: lead with FOMO to attract → use anti-procrastination mechanics (daily micro-tasks, streaks) to retain → unlock financial features only after fixing the UX gap.

---

## Stack

- Telegram Bot API
- AI agent backend (conversational logic)
- Excel — synthetic data design and segmentation
- Product analytics — CSAT, retention, trigger mapping

---

## Team

This was a group project for the Business Analytics course at **SDU University**, 2025.

The project had 11 functional modules mirroring a banking superapp architecture:

| # | Module |
|---|---|
| 1 | R&D |
| 2 | Architecture |
| 3 | Innovations |
| 4 | OKR |
| 5 | Services Platform |
| 6 | **IDP** ← my team |
| 7 | Business & Personal Growth |
| 8 | Wish List |
| 9 | Ecosystem Auditing |
| 10 | Onboarding & Survey |
| 11 | Rewards & Motivation |

I was part of the **IDP module** — responsible for life stage framework design, synthetic data for the IDP segment, and trigger analysis for the 16–25 age group.
