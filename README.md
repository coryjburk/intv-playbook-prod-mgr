# Full-Time MBA Program · David Eccles School of Business - Product Management Interview Playbook

**A self-contained, browser-based interview-prep tool for Product Management candidates.**
Built for the University of Utah — David Eccles School of Business MBA program (PM track).

---

## Live Link

[Intv playbook - Prod Mgmt vC](https://coryjburk.github.io/intv-playbook-prod-mgr/)

---

100 PM interview questions, 10 frameworks, an 8-panel battlecard, 10 recruiter red flags, a voice practice studio, an AI-coaching workflow, and a Readiness self-assessment that tracks your rubric grades and confidence over time — all in a single HTML file with no install, no account, and no server.

---

## Table of contents

- [What it is](#what-it-is)
- [Who it's for](#who-its-for)
- [Getting started](#getting-started)
- [The six sections](#the-six-sections)
- [The AI coaching workflow](#the-ai-coaching-workflow)
- [The scoring rubric](#the-scoring-rubric)
- [Reading your Readiness dashboard](#reading-your-readiness-dashboard)
- [Voice practice stats explained](#voice-practice-stats-explained)
- [Data, privacy & sync](#data-privacy--sync)
- [Customizing & maintaining](#customizing--maintaining)
- [Troubleshooting](#troubleshooting)
- [Quick reference](#quick-reference)
- [Credits](#credits)

---

## What it is

The playbook is a single `pm-playbook.html` file that runs entirely in your browser. It contains:

- **100 interview questions** across **8 categories** and **3 difficulty levels**, each with **four answer layers** (a conversational response, a deep dive, coaching on how to score points, and the red flag that tanks the answer).
- **10 frameworks** interviewers expect you to reach for (CIRCLES, RICE, North Star, AARRR, JTBD, and more).
- An **8-panel battlecard** — concepts, power phrases, metrics, prioritization principles, common mistakes, strong-candidate signals, final-round differentiators, and a last-minute review.
- **10 recruiter red flags**, each with its warning signs and the fix.
- A **voice practice studio** that transcribes your spoken answer and reports pace and filler words.
- An **AI-coaching workflow** that grades your answer against a PM rubric.
- A **Readiness self-assessment** that tracks your graded scores and your self-rated confidence side by side.

Everything you do is saved automatically in your browser. There is no sign-in and nothing leaves your device.

## Who it's for

PM candidates preparing for interviews — especially Eccles MBA students targeting Product Management, Product Strategy, Growth, and adjacent roles. It is built for self-directed practice: you rehearse out loud, get graded, and watch your readiness build over time.

---

## Getting started

### Option 1 — Open it locally
Download `pm-playbook.html` and double-click it. It opens in your default browser. Everything works offline except the voice features, which need a Chromium- or Safari-based browser (see below).

### Option 2 — Host it on GitHub Pages
1. Add `pm-playbook.html` to your repository (rename it to `index.html` if you want it served at the repo root).
2. In the repo, go to **Settings → Pages** and set the source to your `main` branch.
3. Save, wait a minute, and visit the published URL.

The file is fully self-contained — there is nothing to build, bundle, or configure.

### Browser support
| Feature | Requirement |
|---|---|
| Question bank, frameworks, battlecard, scoring, Readiness | Any modern browser, desktop or mobile |
| Voice recording / transcription | Chrome, Edge, or Safari (uses the Web Speech API) |
| Copy-to-clipboard | Any modern browser (falls back to text selection) |

If voice isn't available, you can still rehearse with the timer and read the model answers — the prompt says so on screen.

---

## The six sections

Use the top navigation to move between them.

### 1. Question Bank
The 100 questions, filterable by **category** and **difficulty** (Foundational, Core, Advanced) and searchable by keyword. Expand any question to see its four answer layers:

- **Conversational** — a response you'd actually say out loud.
- **Deep Dive** — the underlying concept in depth.
- **Coaching** — how to score points on this question.
- **Red Flag** — what tanks the answer.

Mark questions **Reviewed** as you go; a progress counter tracks how many of the 100 you've covered.

**The eight categories:** Product Sense & Customer Empathy · Product Strategy · Execution & Metrics · Prioritization & Roadmapping · Product Design & User Experience · Analytics & Experimentation · Stakeholder Management & Leadership · Behavioral & Career Motivation.

### 2. Practice & Evaluation
Click **Practice out loud** on any question to open the practice studio. There you can:

- **Record or type your answer.** Voice is transcribed live.
- See your **duration**, **words per minute**, and **filler-word count** as you speak.
- **Reveal the model answer** in four tabs (the same four layers as the question bank).
- **Copy an AI-coach prompt** tailored to that exact question.
- **Log the rubric scores** your AI coach gives you.

### 3. Frameworks
Ten frameworks with their steps and an interview tip for each: **CIRCLES**, **RICE**, **North Star Metric**, **AARRR (Pirate Metrics)**, **Jobs To Be Done**, **Opportunity Solution Tree**, **Strategy Cascade**, **Experiment Design**, **Stakeholder Alignment (RACI + Interests)**, and **Metric-Drop Root Cause**.

### 4. Battlecard
Eight quick-reference panels for last-minute review: Must-Know Concepts, Power Phrases, Metrics to Know Cold, Prioritization Principles, Common Mistakes, Strong-Candidate Signals, Final-Round Differentiators, and a Last-Minute Review checklist.

### 5. Red Flags
The ten patterns that make interviewers quietly write you off — each with its warning signs and exactly how to flip it into a strength.

### 6. Readiness Self-Assessment
Two views of your readiness, side by side: **how you're scoring** (from the rubric grades you log) and **how you feel** (your own confidence ratings). See [Reading your Readiness dashboard](#reading-your-readiness-dashboard).

---

## The AI coaching workflow

This is the core loop. The tool does not call any AI service itself — you bring your answer to Claude, and Claude grades it. That keeps the tool free, private, and able to run anywhere (including GitHub Pages) with no API key.

1. Open a question and click **Practice out loud**.
2. *(Optional)* Record or type your answer so it's included in the prompt.
3. Click **Copy prompt with my answer**. This copies a prompt tailored to that question, including what a strong answer covers, the red flags to avoid, and the six-dimension rubric.
4. Paste it into **Claude** (claude.ai). Claude gives you feedback and ends with your scores in a clean, loggable format:
   ```
   Problem Framing: X/5
   Customer Insight: X/5
   Structure: X/5
   Metrics: X/5
   Prioritization: X/5
   Communication: X/5
   ```
5. Back in the tool, tap the **1–5 score** for each of the six dimensions. The tool rolls them into an **overall score out of 100** and assigns a **readiness tier**.
6. Click **Save evaluation**. The session is logged to your Readiness dashboard, and the question is automatically marked **Reviewed**.

> You enter the scores manually — the AI provides the grade, you record it. The only thing automated is the arithmetic.

---

## The scoring rubric

Every answer is graded on six dimensions, each from **1 to 5**:

| Dimension | What it measures |
|---|---|
| **Problem Framing** | Clarified the question and defined the problem, goal, and scope before jumping to solutions. |
| **Customer Insight** | Named a specific user/segment and the underlying job-to-be-done; real empathy, not just features. |
| **Structure** | Used a clear framework and logical flow; signposted the answer; didn't ramble. |
| **Metrics** | Defined how success is measured; chose the right metrics; distinguished leading vs. lagging; named guardrails. |
| **Prioritization** | Weighed tradeoffs, said what *not* to do, sequenced the work, and showed judgment under constraints. |
| **Communication** | Clear, concise, well-paced, and persuasive delivery; for behavioral answers, a tight STAR arc. |

**How the overall score works:** six dimensions × a maximum of 5 = 30 points, normalized to a 0–100 scale. The result maps onto five readiness tiers:

| Score | Tier |
|---|---|
| 0–49 | Getting Started |
| 50–67 | Developing |
| 68–81 | Competitive |
| 82–91 | Interview Ready |
| 92–100 | Offer Ready |

All six dimensions must be rated before a session can be saved, since the AI-coach prompt always returns all six.

---

## Reading your Readiness dashboard

The Readiness section combines objective and subjective signals.

- **How you're scoring** — your overall average out of 100, your current tier, and the number of graded sessions.
- **Rubric profile** — a bar for each of the six dimensions showing your average, with your **weakest** and **strongest** tagged. This is the fastest way to see, for example, that Metrics is dragging you down across every question.
- **Recent evaluations** — your last ten graded sessions, each with its score, tier, date, and any note you added.
- **How you feel** — a confidence slider (1–5) for each of the eight categories. Once you've logged graded sessions in a category, the row also shows your coach average and a trend arrow.
- **Calibration nudges** — when your felt confidence and your actual grades diverge (for example, you feel solid but keep scoring low, or vice versa), the tool points it out. That gap is the most useful signal in the whole section.

The three buttons at the top let you **Reset confidence ratings**, **Clear practice evaluations**, or **Clear all my progress**. Each asks for confirmation, and each only affects this browser.

---

## Voice practice stats explained

- **Duration** — total time since you started recording.
- **Words per minute** — measured over the time you actually spend *talking*, not including the seconds you pause to think, so a thoughtful pause doesn't deflate the number. The interview sweet spot is roughly **120–150 wpm**.
- **Filler words** — true disfluencies (um, uh, er, and similar) are counted and highlighted. Ambiguous "crutch words" (like, so, actually, right) are surfaced as a gentle note only if you lean on them heavily — they're never penalized, because they usually have legitimate uses.

---

## Data, privacy & sync

- **Everything is stored locally** in your browser via `localStorage`. Nothing is sent to a server, and there is no account or sign-in.
- Three keys hold your data: `eccles_pm_playbook_reviewed_v1` (reviewed questions), `eccles_pm_playbook_confidence_v1` (confidence ratings), and `eccles_pm_playbook_evals_v1` (logged evaluations).
- **It does not sync across devices or browsers.** Your progress on a laptop won't appear on your phone, and vice versa.
- **Private/incognito windows don't persist data.** Use a normal window if you want your progress saved.
- Clearing your browser's site data (or using the in-app **Clear** buttons) erases your progress.

---

## Customizing & maintaining

The file is self-contained. Everything lives in one `<script>` block and a `:root` CSS block.

- **Content** is defined in plain data arrays near the top of the script: `PM_QUESTIONS`, `PM_FRAMEWORKS`, `PM_BATTLECARD`, `PM_REDFLAGS`, plus `PM_RUBRIC` (the six dimensions) and `PM_TIERS` (the five score bands). Edit those to change questions, frameworks, the rubric, or the tier thresholds.
- **Branding** is controlled by CSS variables in `:root` — including the crimson accent (`--red: #CC0000`) and gold (`--gold: #c9a84c`) — plus the Schibsted Grotesk / Inter / IBM Plex Mono type stack.
- **Resetting stored data on a content update:** if you change the questions or rubric and want returning users to start clean, bump the version suffix on the storage keys (for example `_v1` → `_v2`).
- **Upgrade path to live AI grading:** the tool currently uses a copy-paste workflow (no API key, works everywhere). If you later stand up a server-side proxy that holds your API key, the same rubric, rollup, and dashboard can be wired to an in-app "Evaluate" button — only the input method changes.

---

## Troubleshooting

**Voice recording doesn't start.**
Use Chrome, Edge, or Safari, and allow microphone access when prompted. Some browsers only grant mic access over `https://` or a local `file://` page.

**My scores or progress disappeared.**
Check that you're not in a private/incognito window, that you're using the same browser and device, and that you didn't clear your browser's site data. Progress is per-browser and per-device by design.

**The "Copy prompt" button didn't copy anything.**
Grant clipboard permission if prompted. If copy is blocked, the prompt text is still on screen — select it and copy manually.

**Nothing appears on my GitHub Pages URL.**
Confirm the file is named so Pages can serve it (rename to `index.html` for the repo root), that Pages is enabled on the correct branch, and give it a minute to publish.

---

## Quick reference

**The practice-and-log loop, in six steps:**
1. Open a question → **Practice out loud**
2. Record or type your answer *(optional)*
3. **Copy prompt with my answer**
4. Paste into Claude → get your six rubric scores
5. Tap each **1–5** score back in the tool
6. **Save evaluation** → it's tracked in Readiness

**The six rubric dimensions:** Problem Framing · Customer Insight · Structure · Metrics · Prioritization · Communication

**The five tiers:** Getting Started → Developing → Competitive → Interview Ready → Offer Ready

---

## Credits

Built for the **University of Utah — David Eccles School of Business** MBA program, Product Management track, in support of MBA Career Services interview preparation.

The playbook runs entirely in the browser and stores all data locally. It is intended as a personal practice aid; logged scores are self-reported and meant for individual self-assessment, not formal evaluation.
