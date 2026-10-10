# Hyperbloom October 2026 (UI/UX and Web Design): Rules, Judging, Requirements and Past Editions

> **Access note for the report writer:** devpost.com and every `*.devpost.com` page could not be opened directly from this research session. The shell got HTTP 403 from the egress proxy (org policy) and WebFetch got DNS `ENOTFOUND`. The same was true of web.archive.org, hyperbloomhacks.com, hackathonradar.com and startupgrantsindia.com. All Devpost facts below therefore come from **search-engine extracts of the official Devpost pages**: they are near-verbatim but **not** checked against the live page. The only primary documents read in full were participants' GitHub READMEs (github.com was reachable). **Before submitting, the team must open https://hyperbloom-october.devpost.com/rules themselves** to confirm the deliverables, team size, AI rules and weights. None of these four could be confirmed here.
> Today: 2026-10-10 (Saturday). Deadline: Monday 19 Oct 2026, 5:00pm EDT, which is **Tuesday 20 Oct 2026, 02:30 IST**. About 9 days remain.

## Q1. What is the exact theme / problem statement / track(s)? Is it UI/UX only, or design + build?

### Takeaway
The October 2026 edition is a single-track "UI/UX and Web Design" hackathon. Any product type is allowed (website, web app, mobile interface, dashboard, interactive experience or prototype) and the stated focus is design and usability. The page says a complex backend is not required: a Figma prototype, an interactive mockup or a frontend build can all qualify. No narrower themed prompt (e.g. "build for climate") was found.

### Cited Findings
- Official page title: "Hyperbloom October- UI/UX and Web Design" (the tagline after the colon is blank in the indexed title: "Hyperbloom October- UI/UX and Web Design: - - Devpost"). — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- What to build (search extract of the official page): entries should be "a website, web app, mobile interface, dashboard, interactive experience, or prototype focused on design and usability." — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Scope of ideas (search extract): you can "start with a completely new idea, redesign an existing experience, or explore an unconventional way of solving a familiar problem." — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Design-only entries are allowed (search extract, paraphrased by the search engine): "a complex backend isn't required. A Figma prototype, interactive mockup, or frontend build can qualify". What matters is "how thoughtfully you approach the user, the problem, and the experience." — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- A later search snippet of the same page found no Figma mention in its visible excerpt, so the "Figma prototype" wording comes from one extract only. — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Only one track appears. The extracts mention no sub-tracks; the only special category is "Best Use of Deployxa" (see Q4). — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Each Hyperbloom 2026 edition has had its own domain theme: V2 "Bloom Beyond Limits" (beginner-friendly, open), Summer-bloom '26, September "AI/ML: Build Intelligence", October "UI/UX and Web Design". — [Devpost: Hyperbloom V2](https://hyperbloom-v2.devpost.com/); [Devpost: Hyperbloom Summer](https://hyperbloom-summer-hackathon.devpost.com/); [Devpost: Hyperbloom September](https://hyperbloom-september.devpost.com/)

### Inferences
- A Figma-only entry is officially eligible. However, the sponsor prize (Deployxa, a deployment platform) and the "polish of the prototype or implementation" criterion both reward a **deployed, clickable frontend**. The safest strategy is a Figma case study plus a live coded frontend (e.g. React/Vite deployed on Deployxa). That covers both "prototype" and "implementation".
- "Redesign an existing experience" is explicitly invited, so a well-researched redesign of a real Indian product (e.g. a government portal, railway booking or campus ERP) is in scope. Whether reusing **your own pre-existing code** is allowed is a separate question (see Q2).

### Gaps
- The full verbatim "About the challenge" text and any monthly sub-prompt could not be read, because the live page was unreachable.
- Whether a Figma link alone (with no video or live URL) satisfies the *mandatory* submission form is unconfirmed.

## Q2. Submission requirements: Figma link, demo video (max length), live URL, GitHub repo, case study, screenshots, new vs existing work, AI usage?

### Takeaway
None of the indexed extracts showed October's submission checklist. Below is everything known, mostly by analogy with the September 2026 edition from the same organiser. That edition, per a participant's README, required a 200–500 word description, a public GitHub repo, an AI tools disclosure, a working live demo, a demo video, team members listed, and a post-event survey. October entrants are publicly disclosing pre-existing code reuse and heavy AI assistance in their READMEs, which suggests disclosure is expected. October's actual rule on this is unverified.

### Cited Findings
- **October:** the search engine "couldn't find a separate rules page or a formal list of submission files for this event". The demo video and team size "neither appears in the snippet". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- **September 2026 (EARLIER EDITION, same organiser), submission requirements as listed in a participant README:** "A project description of 200 to 500 words"; "A public GitHub repository"; "An AI tools disclosure"; "A working live demo"; "Team members listed on the Devpost entry"; "A demo video" (that team's script ran 90 seconds, so the official maximum length is not stated); "The post-event survey, after submitting"; eligibility confirmed as students above the age of majority. — [GitHub: dgexplores/hyperbloom-bloompulse README](https://github.com/dgexplores/hyperbloom-bloompulse)
- **September 2026 AI rule (EARLIER EDITION), quoted in the same README:** "using existing models and AI/ML APIs is allowed as long as AI/ML plays a meaningful role". — [GitHub: dgexplores/hyperbloom-bloompulse README](https://github.com/dgexplores/hyperbloom-bloompulse)
- **October entrant disclosure example (Clearledger):** the README says the project was "entered in Hyperbloom October 2026", calls it a "functional design prototype", and says some components were built **before registration** ("disclosed reuse"). It also says development used "substantial AI assistance, including Codex". It ships source as a zip with synthetic data, mentions screenshots, and claims no usability study. — [GitHub: m7mdd77/clearledger-design-prototype](https://github.com/m7mdd77/clearledger-design-prototype)
- **October entrant example (Calmly, repo named "Hyperbloom-October"):** a React 19 + TypeScript + Vite app with a live Vercel URL (hyperbloom-october.vercel.app) and an "in-app accessibility inspector" for "reviewers and judges" that tests contrast and simulates colour blindness. Other features: 44px minimum touch targets (WCAG 2.5.8), OpenDyslexic/Atkinson Hyperlegible fonts, a high-contrast theme, full keyboard navigation and `prefers-reduced-motion` support. The README does not explicitly name the hackathon beyond the repo name. — [GitHub: Leandre99/Hyperbloom-October](https://github.com/Leandre99/Hyperbloom-October)

### Inferences
- Expect the October form to mirror September's: description, link(s), video, team members and probably a repo/AI disclosure field. **Prepare all of these regardless:** a Figma prototype link, a live URL, a public GitHub repo, a 1–3 minute demo video (Devpost norm; the length is unconfirmed), screenshots/gallery images, a case-study write-up (problem → research → personas → flows → wireframes → UI → accessibility audit), and an explicit AI-tools disclosure.
- Strong October competitors are already shipping deployed, accessibility-heavy coded frontends (Calmly). A static Figma file alone may look weak against them on the "polish" and "accessibility" criteria.
- On new vs existing work, add a clear "built during the hackathon" statement and disclose any reused assets, as Clearledger did. That is cheap insurance against a disqualification challenge.

### Gaps
- October's mandatory fields, video maximum length, live-URL requirement and repo requirement: not confirmed (page unreachable).
- October's rule on pre-existing projects / work created only during the submission period: not stated in any extract.
- October's AI-tool usage rule (e.g. whether AI-generated designs are allowed and whether disclosure is required): not stated in any extract.

## Q3. Judging criteria (descriptions and weights), judging process, judges

### Takeaway
The October page lists six focus areas: UX and user flows; visual UI; accessibility and inclusive design; creative interaction and information architecture; problem-solving and originality; and the polish of the prototype or implementation. **No weights were visible.** Two judges are named: Fenil Shah (Software Engineer, Amazon) and Ankur Bhatnagar (IEEE Senior Member). Public voting is not mentioned.

### Cited Findings
- October criteria (search extract, wording paraphrased by the search engine): "UX and user flows, UI appeal, accessibility and inclusive design, interaction and information architecture, problem-solving and originality, and the polish of the prototype or implementation". The extract "doesn't state weightings or a formal scoring rubric". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- A second extract of the same page words them as "UX and user flows, UI, accessibility and inclusive design, creative interaction and information architecture, problem-solving and originality, and a polished prototype". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- October judges: "Fenil Shah, who works as a software engineer at Amazon, and Ankur Bhatnagar, an IEEE senior member." — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Organiser contact for judge enquiries (listed on Hyperbloom pages): hyperbloomhacks@gmail.com. — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/); [Hyperbloom Hacks site](https://www.hyperbloomhacks.com/)
- **EARLIER EDITION, September 2026 AI/ML, weights per a participant README:** Impact & Relevance 25%; Technical Implementation 25%; Innovation & Creativity 20%; AI/ML Integration 20%; Presentation & Demo 10%. — [GitHub: dgexplores/hyperbloom-bloompulse README](https://github.com/dgexplores/hyperbloom-bloompulse)
- **EARLIER EDITION, Summer-bloom '26 criteria:** innovation, impact potential, feasibility. Judge: Shlok Nemani. — [Devpost: Hyperbloom Summer](https://hyperbloom-summer-hackathon.devpost.com/)

### Inferences
- With six roughly parallel criteria and no weights shown, assume about equal weight. Accessibility is an explicit criterion, so a documented WCAG audit (contrast ratios, keyboard flow, screen-reader labels, touch-target sizes, reduced motion) is a direct scoring lever. Many design-hackathon entries skip it.
- The judges are engineers (Amazon SWE, IEEE senior member), not professional product designers. This suggests that clear problem framing, working interactions and a well-explained demo will land better than purely aesthetic Dribbble-style shots.
- If October follows September's pattern, "Presentation & Demo" may carry only about 10% weight, but the video and write-up are how judges experience every other criterion.

### Gaps
- October criterion weights and exact official descriptions: not stated in any accessible extract.
- Judging process details (judging period length, number of rounds, public/popular vote) and full judge bios beyond one line: not stated.

## Q4. Prizes (cash, credits, special categories)

### Takeaway
The total cash pool is US$9,117 (1st $5,059, 2nd $3,029, 3rd $1,029), plus Deployxa hosting credits and a separate "Best Use of Deployxa" prize. That is far larger than earlier Hyperbloom editions (₹19,000 for V2; $710 for September).

### Cited Findings
- "$9,117 in cash across three places, with Deployxa credits and plan subscriptions added." 1st: "$5,059 in cash plus $5,000 in Deployxa credits and 12 months of the Deployxa Team plan". 2nd: "$3,029 in cash and $3,000 in credits". 3rd: "$1,029 in cash and $1,500 in credits". Also "a separate 'Best Use of Deployxa' prize". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Second place, third place and "Best Use of Deployxa" are each listed with one winner. — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- The prize arithmetic checks out: 5,059 + 3,029 + 1,029 = 9,117 (own calculation from the cited figures).
- Deployxa describes itself as a platform to "Ship Any AI-Built Application to Production in 60 Seconds" that "builds, secures, and runs SaaS Products, APIs, AI agents, MCP servers, websites, and backend services", with a free tier ("$0/ forever") and a VS Code extension. — [Deployxa](https://deployxa.com/); [VS Code Marketplace: Deployxa](https://marketplace.visualstudio.com/items?itemName=Deployxa.deployxa-vscode)
- No public source describes the "Best Use of Deployxa" criteria. — search returned none ([Deployxa](https://deployxa.com/))

### Inferences
- Deployxa looks like the main sponsor. A team that deploys its live frontend on Deployxa (free tier) becomes eligible for the extra prize at near-zero cost. Whether one project can win both a placement and Best Use of Deployxa is not stated.
- The pool is about 13× September's, so expect more and stronger entrants than in earlier Hyperbloom editions.

### Gaps
- Cash value (if any) and judging criteria for "Best Use of Deployxa": not stated.
- Whether prizes can stack, the payment method for non-US winners (relevant for Indian bank/PayPal payout and TDS/tax forms), and the payout timeline: not stated.
- No special categories such as "best accessibility" or "best newcomer" were found.

## Q5. Eligibility (India?), team size, age, individual vs team

### Takeaway
Officially: "Above legal age of majority in country of residence; Students only; Companies/professional organizations excluded; all countries/territories, excluding standard exceptions." India is not excluded, but Indian entrants must be **18+** (India's age of majority) and students. Team size for October is not stated.

### Cited Findings
- Eligibility line (Devpost sidebar, via search extract): "Above legal age of majority in country of residence; Students only; Companies/professional organizations excluded; all countries/territories, excluding standard exceptions". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- September 2026 (EARLIER EDITION) was described as "an online AI/ML hackathon for high school and college students". A third-party summary of it says "Teams can be of any size, though solo participation is also allowed". The search engine warned not to assume this applies to October. — [Devpost: Hyperbloom September](https://hyperbloom-september.devpost.com/); [StartupGrantsIndia listing](https://www.startupgrantsindia.com/competitions/hyperbloom-september-aiml)
- The organiser brands itself "created by high schoolers, for high schoolers". — [Hyperbloom Hacks site](https://www.hyperbloomhacks.com/)

### Inferences
- "Standard exceptions" on Devpost normally means US-sanctioned jurisdictions (e.g. Cuba, Iran, North Korea, Syria, Crimea/occupied regions). India is not among them, so India is eligible. This is based on general Devpost practice, not the October rules text.
- There is a tension between the "for high schoolers" branding and the "age of majority" rule. Every Indian team member should be 18+ and able to show student status (college ID) to avoid disqualification at prize-verification time.

### Gaps
- October team size (minimum/maximum), whether solo entries are allowed, and the exact list of excluded countries: not stated in accessible extracts.

## Q6. Key dates (with IST)

### Takeaway
The submission deadline is **19 Oct 2026, 5:00pm EDT = 21:00 UTC = Tuesday 20 Oct 2026, 02:30 IST**. The submission start date, judging period and winner announcement date were not found.

### Cited Findings
- Deadline: "October 19, 2026 at 5:00pm EDT"; the event is "still open" as of the search date. — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- IST conversion: US daylight time runs until 1 Nov 2026, so EDT (UTC−4) applies. 17:00 EDT on Mon 19 Oct is 21:00 UTC on Mon 19 Oct, which is **02:30 IST on Tue 20 Oct 2026** (own calculation with the `date` utility).
- EARLIER EDITIONS for pattern: V2 ran "Mar 16 – Apr 15, 2026" ([Devpost: Hyperbloom V2](https://hyperbloom-v2.devpost.com/)). Summer-bloom '26 ran "Jun 7–30, 2026" ([Devpost: Hyperbloom Summer](https://hyperbloom-summer-hackathon.devpost.com/)). September ran "August 25 to September 14, 2026", with deadline 14 Sep 5:00pm EDT (= 15 Sep 02:30 IST) ([Devpost: Hyperbloom September](https://hyperbloom-september.devpost.com/); [BloomPulse README](https://github.com/dgexplores/hyperbloom-bloompulse)). The Hyperbloom Hacks homepage instead said "September 1st to 14th", a conflict between sources ([Hyperbloom Hacks site](https://www.hyperbloomhacks.com/)).

### Inferences
- Treat the effective Indian deadline as **Monday 19 Oct, 11:59pm IST** for a safety margin. Devpost hard-closes at the timestamp, and Indian teams who read "19 October" as their local day end would actually have 2.5 extra hours. The bigger risk is confusing EDT with IST and planning around the wrong day.
- The September edition went from 14 Sep close to an October event by about 25 Sep. Results are likely announced within 2–4 weeks of 19 Oct, but this is unconfirmed.

### Gaps
- Submission open date, judging period dates and winner announcement date for October: not stated in any accessible source.

## Q7. Who organises Hyperbloom; mission and values; sponsors

### Takeaway
Hyperbloom is run by **Hyperbloom Hacks**, a student-led group that runs online Devpost hackathons for high-school and college students. It promotes "innovation, collaboration, and creativity" and runs monthly or seasonal editions, each themed by tech domain. The listed sponsor/partners are Deployxa (October), Y2 Entrepreneurship Labs (V2 and 2023 mentorship prizes) and YRI (Summer-bloom research fellowship prizes).

### Cited Findings
- Hyperbloom Hacks is "a student-led initiative that organizes hackathons created by high schoolers, for high schoolers, focused on innovation, collaboration, and creativity". It provides "a platform for high school students to learn new skills and collaborate with like-minded peers". Its founders page lists members who are high-school students; no single named founder was found. — [Hyperbloom Hacks site](https://www.hyperbloomhacks.com/)
- Community channels: the website links to a Discord server and an Instagram account (@hyperbloom_hacks). Contact: hyperbloomhacks@gmail.com. — [Hyperbloom Hacks site](https://www.hyperbloomhacks.com/); [imginn mirror of @hyperbloom_hacks](https://imginn.com/y2labs/)
- History: an Instagram mirror shows "#HyperbloomHacks2023" and a grand prize sponsored by Y2 Entrepreneurship Labs (a 1:1 mentorship on turning the project into a startup). That suggests the group has run events since 2023 (third-party mirror, secondhand). — [imginn mirror](https://imginn.com/y2labs/)
- October sponsor: Deployxa (credits, Team plan and "Best Use of Deployxa" prize). Apple, Google and Outlook also appear under a heading on the page, but "the text doesn't make clear whether they are sponsors". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- V2 sponsor: "1:1 Zoom mentorship session with experts from Y2 Entrepreneurship Labs" and ".xyz domain" prizes. — [Devpost: Hyperbloom V2](https://hyperbloom-v2.devpost.com/)
- Summer-bloom '26 prizes: "a YRI Fellowship discounted seat and a 1-on-1 research consultation session with a YRI PhD mentor". — [Devpost: Hyperbloom Summer](https://hyperbloom-summer-hackathon.devpost.com/)

### Inferences
- "Apple, Google, Outlook" are almost certainly Devpost's standard "Add to calendar" links, not sponsors.
- The V2 prizes were in INR (₹), and V2 gallery projects target Indian users ("Rural Indian Teachers", "Tier 2/3 students"). The organisers and much of the participant base appear to be India-connected, so a team solving a concrete Indian user problem fits the community well.
- The organisers value beginner-friendliness, learning and collaboration. A submission that shows a clear design process (research → iteration) probably fits their ethos better than a slick but unexplained final screen.

### Gaps
- The organisers' legal entity, location, named leads and full About-page text could not be read (site unreachable). Discord announcements, the Updates tab and Discussions were also unreachable.

## Q8. Previous Hyperbloom editions: winners and winner traits

### Takeaway
Four earlier editions are confirmed: 2023 Hacks, V2 (Mar–Apr 2026), Summer-bloom '26 (Jun 2026) and September AI/ML (Aug–Sep 2026). **No winner list could be verified for any of them.** Only one project (V2's PathwayAI) appears next to a "Winner" label, and the search engine itself called that placement ambiguous. Visible V2 gallery entries were AI tools for Indian education and skills.

### Cited Findings
- **Hyperbloom V2 "Bloom Beyond Limits" (EARLIER EDITION):** "Mar 16 – Apr 15, 2026"; "₹ 19,000 in cash"; "215 participants". Prizes: grand prize ₹5,000; the "top 10 winning teams will each receive one free .xyz domain"; plus a Y2 Labs 1:1 mentorship. Status: ended, winners announced. — [Devpost: Hyperbloom V2](https://hyperbloom-v2.devpost.com/); [Devpost portfolio listing](https://devpost.com/dawanemanasvi/challenges?page=1)
- **V2 gallery entries seen in search extracts (winner status unverified):**
  - **PathwayAI**: "offline first AI learning platform for Tier 2/3 students", running locally with LLaMA and Groq. A "Winner" label appears next to it in the scrambled gallery text, but "the 'Winner' label could belong to a neighboring project". — [Devpost: Hyperbloom V2 gallery](https://hyperbloom-v2.devpost.com/project-gallery)
  - **Acharya**: "AI Classroom Coach for Rural Indian Teachers". — [Devpost: Hyperbloom V2 gallery](https://hyperbloom-v2.devpost.com/project-gallery)
  - **PhysiX AI**: "Intelligent Simulation Debugging Agent". — [Devpost: Hyperbloom V2 gallery](https://hyperbloom-v2.devpost.com/project-gallery)
  - **SkillForge**: "AI-powered adaptive onboarding engine" that compares a resume against a job description. — [Devpost: Hyperbloom V2 gallery](https://hyperbloom-v2.devpost.com/project-gallery)
- **Summer-bloom '26 (EARLIER EDITION):** Jun 7–30, 2026; 244 participants; criteria innovation, impact potential, feasibility; judge Shlok Nemani; YRI fellowship prizes. One portfolio listing says "$12,000 in prizes", which conflicts with the non-cash YRI prizes on the event page. — [Devpost: Hyperbloom Summer](https://hyperbloom-summer-hackathon.devpost.com/); [Devpost portfolio listing](https://devpost.com/futuretech-term/challenges)
- **September 2026 AI/ML "Build Intelligence" (EARLIER EDITION):** prize pool "$710" per Devpost and the participant README. Another listing says "$1,710", so the sources conflict. Example entry: BloomPulse, a sensor-CSV anomaly detector with cited ISO/OSHA passages, deployed on Vercel with 55 tests (README self-reported; not a confirmed winner). — [Devpost: Hyperbloom September](https://hyperbloom-september.devpost.com/); [HackathonRadar](https://www.hackathonradar.com/database/hackathon/hyperbloom-september-2026); [GitHub: BloomPulse](https://github.com/dgexplores/hyperbloom-bloompulse)
- **Hyperbloom Hacks 2023 (EARLIER EDITION):** existence inferred from the hashtag "#HyperbloomHacks2023" and a Y2 Labs grand prize; no gallery found. — [imginn mirror](https://imginn.com/y2labs/)
- Other entries "Built for HyperBloom Hacks" (edition unspecified, winner status unknown): **MIRAGE**, an AI social-engineering decoy and threat-intel MVP (FastAPI, React 19, Claude, Render/Vercel). — [GitHub: ZincProjects/HyperBloom-Hackathon](https://github.com/ZincProjects/HyperBloom-Hackathon)
- No October 2026 winners exist yet (judging after 19 Oct). — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)

### Inferences
- Visible entries in past galleries are **working, deployed builds tied to a specific user group and a social-impact framing** (rural teachers, Tier 2/3 students), often with an Indian context. This is the strongest available signal of what judges in this community reward, though it is drawn from galleries, not confirmed winners.
- October entries visible so far (Calmly, Clearledger) are coded prototypes with heavy accessibility work, honest scoping and disclosures. That raises the bar above a Figma-only entry.
- **Winning recipe (inference, not stated by organisers):** pick a narrow, real user and problem; show research evidence; deliver a polished interactive prototype plus a deployed frontend (ideally on Deployxa); document an accessibility audit against WCAG; and explain the information architecture and user flows explicitly in the write-up and video, mapped one-to-one to the six criteria.

### Gaps
- Verified winner lists for V2, Summer-bloom '26 and September 2026: not obtainable (Devpost winner tabs unreachable; search extracts did not include them).
- Gallery composition (how many entries were Figma-only vs coded vs video): not obtainable.

## Q9. FAQ / Discord / Updates / Discussions content

### Takeaway
No FAQ, Updates-tab, Discussions or Discord content for October 2026 could be retrieved. All of it sits behind devpost.com and Discord, which were unreachable from this session.

### Cited Findings
- The search engine "couldn't find a separate rules page or a formal list of submission files for this event" and recommended checking "its Rules tab". — [Devpost: Hyperbloom October](https://hyperbloom-october.devpost.com/)
- Devpost's general judging and winner-selection process is documented in its help centre (generic, not event-specific). — [Devpost Help: Ending the judging period](https://help.devpost.com/article/107-ending-the-judging-period-and-selecting-winners)

### Inferences
- Disqualification risks to guard against, inferred from the eligibility line and the September rules:
  - a team member under 18 or not a student;
  - submitting after 02:30 IST on 20 Oct;
  - a missing required field (video or links);
  - private or broken links (Figma not set to "anyone with link can view"; repo private; live URL down during judging);
  - undisclosed AI use or pre-existing work;
  - entering on behalf of a company.

### Gaps
- The October Rules tab (official legal rules, IP clause, AI clause, disqualification clause), the Updates tab, Discussions and Discord announcements: all not retrieved.
