# Industry UX Practices 2024–2026 (catalogue + fact-check of the ChatGPT report)

> Research conditions (read first): Today is 2026-10-10. Partway through, the shared web-search budget for this run ran out, and most sites were blocked by the egress proxy. Only developer.apple.com, microsoft.com, developer.android.com and public GitHub repos could be fetched directly. So the Apple HIG, the WCAG 2.2 spec text (read from the W3C's own GitHub repo), the Microsoft HAX guidelines, Carbon for AI, the web-vitals thresholds and the Shopify Polaris README are **checked against primary sources**. Most other findings come from search-result summaries of the cited pages. The sources are named, but I did not read the full articles, so treat exact wording as approximate. Anything I could not source is in the Gaps sections, labelled "background knowledge, unverified this session".

## Q0. Fact-check of the existing ChatGPT report (claims 1–6)

### Takeaway
Only the WCAG 2.2 numbers (claim 6) and the Spotify Encore "22 systems" figure (claim 2) hold up cleanly. The Airbnb, Duolingo and Stripe claims mix real facts with old or unsourced numbers. Apple's "clarity, deference, depth" is out of date: Apple's current HIG (design principles reintroduced on June 8, 2026) uses different principles. The 44x44 pt figure is correct, but it is Apple's *default* control size, and the HIG lists 28x28 pt as the iOS *minimum*.

### Cited Findings

**Claim 1 – Airbnb (verdict: PARTLY TRUE, with one sub-claim UNVERIFIED and one outdated)**
- *"Embeds UX researchers in product teams for 12–18 months"* → **UNVERIFIED**. I found no source for a 12–18-month embedding period. I ran out of search budget before a dedicated search could finish. Treat it as unsupported.
- *"Photos + verification badges → 2.5x higher bookings in some markets"* → **PARTLY TRUE / OUTDATED and conflated.** The 2.5x figure comes from Airbnb's 2011 professional-photography program: hosts with professional photos were booked "2.5 times more frequently" and earned about $1,025/month on average — [The Next Web, Oct 6 2011](https://thenextweb.com/apps/2011/10/06/airbnb-launches-its-photography-program-with-13000-verified-properties/). The same 2011 launch covered about 13,000 "verified" properties. Here "verified" meant photos taken by Airbnb's photographers, not a trust badge — [TNW](https://thenextweb.com/apps/2011/10/06/airbnb-launches-its-photography-program-with-13000-verified-properties/). Other retellings say the pilot gave "3x" bookings or doubled revenue. Those are vendor accounts, not independent measurements — [Snappr (photo vendor)](https://www.snappr.com/enterprise-blog/photography-that-launched-an-empire-how-airbnb-transformed-their-business-with-professional-photography).
  - **Current official number is much smaller:** Airbnb's own pro-photo page says listings with Airbnb pro photography get **19% more bookings on average**. That compares 2024–2025 data from more than 14,700 listings that used it with more than 62,300 that did not, and Airbnb says results are not guaranteed — [Airbnb Pro Photo Program](https://www.airbnb.com/professional_photography) (seen via search summary).
  - Photography-vendor blogs cite a 2016 Carnegie Mellon study finding that professional photos raised yearly revenue by about $2,455 per unit on average — [Snappr (vendor)](https://www.snappr.co/enterprise-blog/photography-that-launched-an-empire-how-airbnb-transformed-their-business-with-professional-photography). I did not check the primary paper.
- *"Design system with the 'Cereal' font"* → **VERIFIED (2018, older fact).** Airbnb Cereal launched on May 15, 2018 across product and brand. It was developed with the foundry Dalton Maag — [Airbnb Design: Working Type](https://airbnb.design/working-type); [Dezeen, May 2018](https://www.dezeen.com/2018/05/16/airbnb-new-scaleable-typeface-dalton-maag-design/). It comes in six weights with a taller x-height. Karri Saarinen, then design lead for Airbnb's Design Language System (DLS) team and later a Linear co-founder, tuned the Book weight for small UI text — [Dezeen](https://www.dezeen.com/2018/05/16/airbnb-new-scaleable-typeface-dalton-maag-design/). Airbnb publishes no official public DLS documentation site. Third-party teardowns describe the DLS tokens from observation — [superdesign.dev](https://superdesign.dev/blog/airbnb-design-system).

**Claim 2 – Spotify Encore consolidated ~22 UI systems (verdict: VERIFIED, with nuance; 2019–2020 fact)**
- Spotify's own write-ups say Spotify had 22 separate design systems before Encore. Encore was introduced in November 2019 — [Figma blog / Spotify designers: "Creating coherence"](https://www.figma.com/blog/creating-coherence-how-spotifys-design-system-goes-beyond-platforms/); [designsystems.com](https://designsystems.com/how-spotifys-design-system-goes-beyond-platforms/); [notes on "Reimagining design systems at Spotify"](https://rogerswannell.com/notes/reimagining-design-systems-at-spotify/).
- Nuance: Encore is a "family of systems" or "system of systems", not one monolith. Distributed teams own the parts, which inherit from a shared Foundation and are linked by design tokens. The older systems were rebranded or partly extracted rather than thrown away — [Figma blog](https://www.figma.com/blog/creating-coherence-how-spotifys-design-system-goes-beyond-platforms/). A later retrospective (about 2022) says Spotify had to push for more standardization because the flexibility caused drift — [search summary of "Can I get an Encore? Three years on"](https://cur.at/q8afwkA?m=web).

**Claim 3 – Duolingo heavy A/B testing + gamification; "~70% dropoff" (verdict: A/B + gamification VERIFIED; 70% figure UNVERIFIED)**
- Showing the streak at the top of the app gave **+3% DAU and +1% day-14 retention**. Showing it after each lesson gave +1% DAU and +3% D14. These are older tests, roughly 2018–19 — [Econsultancy: six A/B tests used by Duolingo](https://www.econsultancy.com/six-a-b-tests-used-by-duolingo-to-tap-into-habit-forming-behaviour).
- Duolingo's retention team ran **600+ experiments on the streak feature over about 4 years**. One test made streaks easier to extend (a single exercise counted) and did *not* raise DAU — [Lenny's Podcast summary, Jackson Shuttleworth](https://www.recall.it/summary/lennys-podcast/behind-the-product-duolingo-streaks-or-jackson-shuttleworth-group-pm-retention-team).
- Former CPO Jorge Mazal: by mid-2018 DAU growth was in single digits year over year. Leaderboards, reworked push notifications and streak optimization drove up the "current user retention rate" (CURR), and DAU then grew **4.5x** over about four years — [Lenny's Newsletter: How Duolingo reignited user growth](https://www.lennysnewsletter.com/p/how-duolingo-reignited-user-growth); [Reach Capital](https://www.reachcapital.com/?p=5907).
- A secondary source claims "at least 500 A/B tests per quarter, ~40% fail". It has no primary citation, so treat it as weak — [DataPulse Weekly (Substack)](https://datapulseweekly.substack.com/p/how-duolingo-skyrocketed-its-growth).
- Current scale: **50M+ DAU, +36% YoY in Q3 2025** — [Duolingo Q3 FY25 shareholder letter (SEC 8-K)](https://www.sec.gov/Archives/edgar/data/1562088/000162828025049514/q3fy25duolingo9-30x25share.htm). In FY2025 bookings passed **$1B**, and management talks about a medium-term goal of 100M DAU — [Duolingo FY2025 results](https://investors.duolingo.com/news-releases/news-release-details/duolingo-reports-fourth-quarter-and-full-year-2025-results).
- **"~70% dropoff": no source found.** The closest numbers are Sensor Tower's estimate of 28% churn and 68% retained users in Western markets as of Oct 2023 — [Sensor Tower](https://sensortower.com/blog/duolingo-redefining-engagement-in-the-ed-tech-space) — and a student project reporting 28% 30-day retention, which is not authoritative — [NextLeap student PDF](https://assets.nextleap.app/submissions/DATAANALYSISOFDUALINGO-cfa09e78-96db-4653-9cc7-59f9659c88f4.pdf). Drop this figure or reword it.

**Claim 4 – Stripe MVP "paste seven lines of code and accept payments" (verdict: PARTLY TRUE)**
- "Seven lines of code" was Stripe's widely used early pitch line. It is also the headline of Bloomberg Businessweek's 2017 profile, "How Two Brothers Turned Seven Lines of Code Into a $9.2 Billion Startup" — [Longform listing of the Businessweek piece](https://longform.org/posts/how-two-brothers-turned-seven-lines-of-code-into-a-9-2-billion-startup).
- It is a positioning line, not a technical spec. Patrick Collison has noted that Payment Links now need "0 lines of code" — [Stratrix analysis](https://www.stratrix.com/moat-anatomy/stripe-s-api-moat-in-online). The "Collison installation" anecdote (installing Stripe for YC founders on the spot) circulates mostly in secondary blogs — [Stacksync](https://www.stacksync.com/blog/seven-lines-of-code-from-rural-ireland-the-origin-story-of-stripe).
- Better wording for the report: "Stripe's early developer-experience pitch was that integrating payments took about seven lines of code, versus weeks of merchant-account setup." Do not call it "the MVP spec."

**Claim 5 – Apple HIG: 44x44 pt minimum tap targets; "clarity, deference, depth" (verdict: 44x44 PARTLY TRUE; "clarity, deference, depth" OUTDATED / WRONG for 2026)**
- Buttons page: "a button needs a hit region of at least **44x44 pt** — in visionOS, **60x60 pt**" — [Apple HIG: Buttons](https://developer.apple.com/design/human-interface-guidelines/buttons) (fetched).
- The Accessibility page now separates **default** and **minimum** control sizes: iOS/iPadOS 44x44 pt default and **28x28 pt minimum**; macOS 28x28 / 20x20; tvOS 66x66 / 56x56; visionOS 60x60 / 28x28; watchOS 44x44 / 28x28. It also recommends about **12 pt padding** around bezeled elements and **about 24 pt** around unbezeled ones — [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) (fetched). So "44x44 is the minimum" is a simplification. 44x44 is the default and recommended size.
- "Clarity, deference, depth" does not appear in the current HIG pages I fetched (Accessibility, Buttons, Materials, Design principles). On **June 8, 2026** Apple "reintroduced design principles" — [Apple Design: What's new](https://developer.apple.com/design/whats-new/) (fetched). The eight current principles are: *Make something meaningful; Let people do things their own way; Act in people's best interest; Build on what people know; Adapt to diverse contexts and needs; Be clear and direct; Care about every detail; Make it human* — [Apple HIG: Design principles](https://developer.apple.com/design/human-interface-guidelines/design-principles) (fetched).
- The Liquid Glass-era (WWDC25) design-system talk frames the new system as "dynamic, harmonious, and consistent", "more cohesive, adaptive and expressive", built on "concentricity" — [WWDC25 "Get to know the new design system"](https://developer.apple.com/videos/play/wwdc2025/356/) (transcript fetched).

**Claim 6 – WCAG 2.2 AA: contrast 4.5:1 / 3:1; Target Size minimum 24x24 CSS px (verdict: VERIFIED)**
- SC 1.4.3 Contrast (Minimum), AA: text needs **4.5:1**; large-scale text needs **3:1** — [WCAG source, w3c/wcag repo](https://github.com/w3c/wcag/blob/main/guidelines/sc/20/contrast-minimum.html) / [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/#contrast-minimum). "Large scale" means at least **18 pt, or 14 pt bold** — [WCAG term definition](https://github.com/w3c/wcag/blob/main/guidelines/terms/20/large-scale.html).
- SC 1.4.11 Non-text Contrast, AA: UI components and meaningful graphics need **3:1** against adjacent colours. The report should mention this; "3:1" covers more than large text — [WCAG source](https://github.com/w3c/wcag/blob/main/guidelines/sc/21/non-text-contrast.html).
- SC 2.5.8 Target Size (Minimum), AA, **new in 2.2**: pointer targets must be at least **24 by 24 CSS pixels**. Exceptions: Spacing (a 24 px circle centred on an undersized target doesn't intersect other targets), Equivalent, Inline, User-agent control, Essential — [WCAG source](https://github.com/w3c/wcag/blob/main/guidelines/sc/22/target-size-minimum.html). AAA SC 2.5.5 Target Size (Enhanced) keeps **44x44 CSS px** — [WCAG source](https://github.com/w3c/wcag/blob/main/guidelines/sc/21/target-size-enhanced.html).

### Inferences
- In the corrected report, say "44x44 pt recommended (Apple) / 24x24 CSS px legal-floor minimum (WCAG 2.2 AA) / 44x44 CSS px AAA". Designing to 44–48 px satisfies all three, and Material's long-standing 48dp guidance as well, though I did not re-verify 48dp this session.
- "Clarity, deference, depth" were Apple's iOS 7-era (2013) themes. That is background knowledge, not verified this session. A 2026 report quoting them signals stale training data.
- Replace the old 2.5x Airbnb number with the current **19%** official figure. It is more credible and more recent.

### Gaps
- No source found for Airbnb's "12–18 month" researcher embedding.
- No source found for Duolingo's "~70% dropoff."
- I could not read the original Bloomberg Businessweek Stripe article; the headline and listing were all I could see.

## Q1. Newest design-system moves (Material 3 Expressive, Liquid Glass, Fluent 2, Carbon, Polaris, Primer, Atlassian)

### Takeaway
2025–2026 design systems moved in two directions at once. One was **expressiveness backed by research**: Google's M3 Expressive and Apple's Liquid Glass, with springs, shape morphing and translucent materials. The other was **consolidation and platform-neutral delivery**: Shopify's framework-agnostic Polaris web components, Atlassian's refreshed foundations and navigation, Fluent 2's token layers, and IBM's dedicated "Carbon for AI" layer. Apple's Liquid Glass shows the risk: the accessibility backlash forced Apple to add user-facing opacity controls after launch.

### Cited Findings
**Google Material 3 Expressive (announced May 2025; shipped on Pixel with Android 16 QPR1, Sept 2025)**
- Google calls it research-backed: **46 research studies, hundreds of designs, 18,000+ participants**. Methods included eye tracking, surveys, focus groups, experiments and usability tests. Outlets disagree on the country count (one says 8 countries) — [Android Authority](https://www.androidauthority.com/google-material-3-expressive-details-3554486/); [9to5Google](https://9to5google.com/?p=671309); [Phandroid](https://phandroid.com/2025/05/13/material-3-expressive-makes-google-apps-feel-less-robotic/).
- Reported findings, all self-reported by Google: participants spotted key UI elements **up to 4x faster**. Older users performed as well as younger ones. Expressive designs were rated more "energetic," "creative," and "friendly." One outlet reports that **87%** of younger users preferred them. Animated indicators eased frustration, and button size affected confidence — [Android Authority](https://www.androidauthority.com/google-material-3-expressive-details-3554486/); [Phandroid](https://phandroid.com/2025/05/13/material-3-expressive-makes-google-apps-feel-less-robotic/). No peer-reviewed methodology has been published.
- What changed: a new shape library with **35 shapes** and shape-morphing (for example square to squircle), a **spring-based motion system**, and about **15 new or refreshed components** (button groups, split buttons, toolbars, loading indicators, FAB menu). It debuted on Pixel with Android 16 QPR1 in **September 2025** — [Android Authority](https://www.androidauthority.com/google-material-3-expressive-features-changes-availability-supported-devices-3556392/).
- Android's developer docs: "M3 Expressive is an expansion of Material Design 3, including research-backed updates to theming, components, motion, typography… The M3 shape scale is more like the type scale" — [Android Developers: Material 3 in Compose](https://developer.android.com/develop/ui/compose/designsystems/material3) (fetched).

**Apple Liquid Glass (WWDC, June 9 2025; iOS 26)**
- Apple says Liquid Glass "marks the most extensive software design update we've made" — [WWDC25 session 356](https://developer.apple.com/videos/play/wwdc2025/356/) (fetched).
- What it is: a dynamic material that forms a separate functional layer for controls and navigation (tab bars, sidebars), floating above content. The HIG says: "Don't use Liquid Glass in the content layer" and "Use Liquid Glass effects sparingly." It has two variants. **Regular** blurs and adjusts luminosity for legibility and suits text-heavy alerts and sidebars. **Clear** is highly translucent and meant for use over media, with an optional dimming layer — [Apple HIG: Materials](https://developer.apple.com/design/human-interface-guidelines/materials) (fetched).
- Apple's stated accessibility support: Liquid Glass responds to Reduce Transparency, Increase Contrast and Reduce Motion "automatically… when system-level settings are enabled" — [WWDC25 "Meet Liquid Glass"](https://developer.apple.com/videos/play/wwdc2025/219/) (transcript fetched). System colours were retuned across Light, Dark and Increased Contrast to improve hue differentiation — [WWDC25 session 356](https://developer.apple.com/videos/play/wwdc2025/356/).
- Criticism: one agency's beta testing measured some screens at about **1.5:1 contrast**, against the 4.5:1 benchmark — [Infinum](https://infinum.com/blog/apples-ios-26-liquid-glass-sleek-shiny-and-questionably-accessible/). Users on Apple's developer forums asked for a system-wide off switch — [Apple Developer Forums thread](https://developer.apple.com/forums/thread/811219). Advocates for people with sensory conditions reported disorienting motion behind translucent bars — [Misophonia International (advocacy)](https://misophoniainternational.com/apple-delivers-a-welcome-fix-new-liquid-glass-toggle-in-ios-26-1-beta-addresses-critical-accessibility-flaws/).
- Apple's response: it reduced transparency during the betas before the September launch. **iOS 26.1** added a **Clear / Tinted** choice under Display & Brightness, where Tinted raises opacity and contrast. **iOS 26.4 beta 4** added a "**Reduce Bright Effects**" accessibility toggle — [PhoneArena](https://www.phonearena.com/news/liquid-glass-was-so-bad-that-apple-will-give-you-another-way-to-tone-it-down_id178795). The HIG now says Liquid Glass's look can change "if people choose a preferred look for Liquid Glass in their device's settings" — [HIG Materials](https://developer.apple.com/design/human-interface-guidelines/materials).
- Ongoing iteration: the HIG got Liquid Glass updates on Sept 9 2025 (Materials, Motion), Dec 16 2025 (Color, Buttons, Toolbars, Tab bars), June 8 2026 (scroll edge effects, app icons) and Sept 9 2026 (new "Designing for iPhone Duo" page for Apple's first folding iPhone) — [Apple Design: What's new](https://developer.apple.com/design/whats-new/) (fetched).

**Microsoft Fluent 2**
- Fluent 2 uses two token layers. **Global tokens** hold raw values such as hex codes. **Alias tokens** carry semantic meaning. Together they support light, dark, high-contrast and branded themes — [Fluent 2: Design tokens](https://fluent2.microsoft.design/design-tokens). Teams was an early adopter. It was announced in 2023, so it is not new for 2025 — [i-programmer](https://www.i-programmer.info/news/90-tools/16386-microsoft-announces-fluent-2.html).
- A report of an internal "Copilot Design System" relies on unnamed sources and is unconfirmed — [windowsnews.ai](https://windowsnews.ai/article/microsoft-365-copilot-gets-a-unified-design-system-to-end-clunky-ai-pop-ups.419644).

**IBM Carbon – "Carbon for AI"**
- "An extension of the Carbon system, designed to give AI instances in IBM products a visually and behaviorally distinct identity." Its rules: mark *every* AI instance with the **AI label**, show how pervasive the AI is at each level (from a single word to a whole page), and integrate explainability without distraction. It also says: "Don't use the Carbon for AI styling as decoration." The styling uses "light as a metaphor to 'illuminate' AI-generated content" (glow, gradients) with dedicated AI colour tokens. Status: style elements and AI components are Stable; AI chat is in Preview — [Carbon for AI](https://carbondesignsystem.com/guidelines/carbon-for-ai/) (source read via [GitHub](https://github.com/carbon-design-system/carbon-website/blob/main/src/pages/guidelines/carbon-for-ai/index.mdx)).
- **"Revert to AI"** pattern: once a user overrides AI-suggested content, the component switches from the AI variant to the default variant, and a "revert to AI" button lets the user switch back — [Carbon for AI](https://carbondesignsystem.com/guidelines/carbon-for-ai/).
- The AI label (formerly "AI Slug") is the trigger for an explainability popover, the "first layer of explanation" — [Carbon AI label usage](https://carbondesignsystem.com/components/ai-label/usage/). Carbon for AI won an iF Design Award — [iF Design](https://ifdesign.com/en/winner-ranking/project/carbon-for-ai/688500).

**Shopify Polaris**
- **May 21 2025:** Polaris was reworked as a single framework-agnostic **web component** toolkit across Admin, Checkout and Customer Accounts. It is served from Shopify's CDN, so apps get design updates automatically — [Shopify changelog (early access)](https://shopify.dev/changelog/polaris-unified-web-components-are-now-available-early-access).
- **Oct 1 2025:** stable, now including POS, with 14 App Home components added — [Shopify changelog (stable)](https://shopify.dev/changelog/polaris-unified-web-components-are-now-stable). The Polaris React repo is **archived and deprecated**. Shopify's reason: web components are "a more technology-agnostic foundation" that works with every framework, plain JS and server-rendered sites — [Shopify/polaris README](https://github.com/Shopify/polaris) (fetched). Dropping React's runtime in UI extensions also shrinks bundles — [Shopify Partners blog](https://www.shopify.com/partners/blog/polaris-unified-and-for-the-web).

**GitHub Primer**
- Primer's contrast overhaul fixed hundreds of contrast issues across 1,000+ use cases in light and dark modes. Each mode has default, dimmed, high-contrast and colour-vision-deficiency themes. This is a 2023 fact — [GitHub Blog](https://github.blog/engineering/user-experience/unlocking-inclusive-design-how-primers-color-system-is-making-github-com-more-inclusive/); [GitHub changelog 2023-03-28](https://github.blog/changelog/2023-03-28-light-and-dark-theme-color-contrast-improvements/). I found no 2025–26 Primer update.

**Atlassian Design System**
- It followed the Team '24 rebrand with a "visual refresh of UI foundations": new **Atlassian Sans / Atlassian Mono** fonts with more distinct heading levels for scanning, line-based icons with consistent sizes (RFC-81, planned for Jan 2025), and new colours still in trial — [Atlassian developer community](https://community.developer.atlassian.com/t/a-visual-refresh-of-our-ui-foundations-is-coming/84949); [RFC-81](https://community.developer.atlassian.com/t/rfc-81-upcoming-changes-to-iconography/87753); [atlassian.design what's new](https://atlassian.design/whats-new/atlassian-ui-refresh-updates).
- The **new navigation** was built on the refreshed foundations, with a personalisable, resizable, collapsible left sidebar. It rolled out first to Jira, JSM, Jira Product Discovery, Home and Confluence — [Atlassian blog](https://www.atlassian.com/blog/announcements/introducing-new-navigation).

**Linear (as a product-level design system)**
- In the March 2024 redesign, Linear rebuilt its theme generator in the **LCH** colour space instead of HSL. It went from **98 per-theme variables to 3 inputs: base colour, accent colour, contrast**. LCH is perceptually uniform, so any base colour produces consistent themes. The default themes also got more contrast — [Linear: How we redesigned the Linear UI](https://linear.app/blog/how-we-redesigned-the-linear-ui); [Linear changelog 2024-03-20](https://linear.app/changelog/2024-03-20-new-linear-ui); [Linear: Behind the latest design refresh](https://linear.app/blog/behind-the-latest-design-refresh).

### Inferences
- For a hackathon: take Linear's **3-input theme model** (base, accent, contrast in LCH or OKLCH) and Fluent's **global → alias token layering**. Both let a small team ship light, dark and high-contrast themes cheaply.
- Liquid Glass is a cautionary tale for judges and teams. Expressive translucency needs a **user-controllable opacity or contrast fallback** from day one. Apple had to add one after launch.
- Material 3 Expressive's "4x faster to find key elements" claim is a usable argument for **bigger, more distinctive primary actions** (size, shape and colour contrast on the main CTA), but cite it as Google's self-reported figure.

### Gaps
- I could not fetch Google's primary M3 Expressive research article on design.google (domain blocked). The figures come via press.
- I could not reach fluent2.microsoft.design's "What's new" for 2025–26 changes to Fluent 2.
- No 2025–26 Primer changes found.

## Q2. AI-native interface design (2025–2026)

### Takeaway
The big companies' guidance converges on the same set of patterns:
- disclose and label AI
- set expectations about what it can and cannot do
- keep the human in control (Edit, Undo, Retry, Revert)
- ask for confirmation before irreversible actions
- describe what is happening during generation instead of showing a vague spinner
- offer alternative results
- collect lightweight feedback
- explain on demand, in layers

Apple (2025 page, expanded in June 2026), Microsoft HAX (18 guidelines) and IBM Carbon for AI are the most concrete primary sources.

### Cited Findings
**Apple HIG – Generative AI (new June 9 2025; updated June 8 2026)** — [Apple HIG: Generative AI](https://developer.apple.com/design/human-interface-guidelines/generative-ai) (fetched)
- "Keep people in control… Give them the ability to dismiss new content they don't want, and revert or retry… Clearly identify when and where you use AI."
- "When possible, consider offering a non-AI fallback" (examples: Genmoji next to regular emoji; notification summaries next to the full notifications).
- "Never trick someone into thinking they're interacting with… content authored by a human."
- For open-ended prompts, "offer curated suggestions" and "diverse, predefined example inputs."
- "Ask for confirmation before performing a significant action on someone's behalf"; "Avoid automating destructive actions."
- **New in 2026:** "surfacing controls like Edit, Undo, Retry, or Adjust near generated content… provide a clear signal that their action had an effect."
- **New in 2026:** specific progress copy. "Instead of 'Processing…', say 'Finding substitutions for ingredients' or 'Summarizing key themes from your notes.'"
- When blocked, coach the user (Image Playground says "Unable to use that description") and suggest better example requests.
- "Consider offering alternate versions of results" (Image Playground generates several images).
- Feedback should be voluntary, unobtrusive, and thumbs up/down with an optional detailed form.
- "Separate your model from your user experience so you can swap out the model."
- Be transparent about on-device versus server processing and what data is sent.

**Microsoft HAX Toolkit – 18 Guidelines for Human-AI Interaction** (from the 2019 CHI paper, Amershi et al., so older but still Microsoft's current guidance) — [HAX guidelines](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/); [HAX Design Library](https://www.microsoft.com/en-us/haxtoolkit/library/) (fetched)
- Grouped by phase. **Initially:** G1 Make clear what the system can do; G2 Make clear how well it can do it. **During interaction:** G3 Time services based on context; G4 Show contextually relevant info; G5 Match social norms; G6 Mitigate social biases. **When wrong:** G7 Support efficient invocation; G8 Efficient dismissal; G9 Efficient correction; G10 Scope services when in doubt; G11 Make clear why the system did what it did. **Over time:** G12 Remember recent interactions; G13 Learn from user behaviour; G14 Update and adapt cautiously; G15 Encourage granular feedback; G16 Convey consequences of user actions; G17 Provide global controls; G18 Notify users about changes.
- Validation: a user study with **49 design practitioners** testing the guidelines against **20 AI-infused products** — [Microsoft Research publication](https://www.microsoft.com/en-us/research/publication/guidelines-for-human-ai-interaction/). The toolkit adds a Workbook for prioritising, Design Patterns, a Design Library and a Playbook for planning failures — [Microsoft blog](https://blogs.microsoft.com/ai-for-business/hax-toolkit/).

**IBM Carbon for AI** — the AI label on every AI instance, a layered explainability popover and "revert to AI" (see Q1) — [Carbon for AI](https://carbondesignsystem.com/guidelines/carbon-for-ai/).

**Shape of AI (Emily Campbell) pattern library**
- Pattern categories include **identifiers, wayfinders, prompts, tuners, trust indicators**. Wayfinders cover follow-up questions, nudges, prompt suggestions and templates — [Shape of AI: Wayfinders](https://www.shapeof.ai/pattern-types/wayfinders); [summary](https://nikitisza.substack.com/p/ai-ux-design-patterns). It is a living, CC-BY-NC-SA resource — [Smashing newsletter](https://www.smashingmagazine.com/the-smashing-newsletter/smashing-newsletter-issue-533/).

**Agentic UX**
- Greg Nudelman frames agent UX around four agent capabilities: perception, reasoning, memory and agency — [UX Magazine](https://uxmag.com/articles/secrets-of-agentic-ux-emerging-design-patterns-for-human-interaction-with-ai-agents). Commentators summarise the core design job as "trust, control and visibility" — [Towards AI](https://pub.towardsai.net/designing-for-ai-agents-8-ux-patterns-that-build-trust-in-2026-713a0c926933). These are secondary or opinion sources.

**Indian voice and conversational commerce (AI-native in practice):** Swiggy and Sarvam AI voice ordering in 11 languages, including a phone-call channel that works with no app or internet — see Q5 — [Techloy](https://www.techloy.com/swiggy-introduces-ai-voice-ordering-with-sarvam-ai-across-11-indian-languages/).

### Inferences
Hackathon-ready AI UX checklist, combining Apple, HAX and Carbon:
1. AI label or badge on generated content.
2. Example prompts or chips on empty state.
3. Streaming output with *specific* status copy.
4. Edit / Retry / Undo / "Revert to AI" next to output.
5. A confirmation step before any irreversible agent action, with a plan preview the user can edit.
6. Two or three alternative results.
7. Thumbs up/down.
8. A "Why this?" popover (sources and reasoning).
9. A non-AI fallback path.
10. A global AI on/off control (HAX G17).

### Gaps
- I could not search for or fetch product-specific write-ups on ChatGPT (agent/Deep Research progress UIs), Perplexity (inline citations), Notion AI, Figma AI (Make/First Draft), Arc or Linear agents. The search budget was used up and the domains were blocked. These patterns are widely known (streaming, numbered citations, step-by-step agent activity logs, "take over" controls), but I did not verify them this session.
- Google's People + AI Guidebook (pair.withgoogle.com) was blocked. Background knowledge, unverified this session: its chapters cover user needs, mental models, explainability and trust, feedback and control, and errors and graceful failure.

## Q3. Accessibility and inclusive design programs

### Takeaway
Accessibility is now enforced by **law** (the European Accessibility Act, enforceable since June 28 2025) and **marketplaces** (Apple's App Store Accessibility Nutrition Labels, 2025). WCAG 2.2 AA is the working baseline. Its new criteria (24 px targets, focus not obscured, no cognitive-test logins, drag alternatives, redundant entry) translate directly into concrete UI requirements.

### Cited Findings
- **WCAG 2.2's 9 new success criteria** (from the W3C repo's `sc/22` folder): Target Size (Minimum) AA; Focus Not Obscured (Minimum) AA ("not entirely hidden due to author-created content", e.g. sticky headers); Focus Not Obscured (Enhanced) AAA; Focus Appearance AAA (an indicator at least as large as a 2 CSS px perimeter, with 3:1 change contrast); Dragging Movements AA (every drag action must also work with a single pointer); Accessible Authentication (Minimum) AA (no cognitive-function tests such as remembering a password or solving a puzzle unless an alternative is available) and Enhanced AAA; Consistent Help A (help in the same relative order across pages); Redundant Entry A (previously entered info is auto-populated or selectable). SC 4.1.1 Parsing is "Obsolete and removed" — [w3c/wcag repo, guidelines/sc/22](https://github.com/w3c/wcag/tree/main/guidelines/sc/22); [Parsing](https://github.com/w3c/wcag/blob/main/guidelines/sc/20/parsing.html).
- **European Accessibility Act:** enforceable since **June 28, 2025**. It covers consumer e-commerce, banking, e-books, transport booking, and smartphones including mobile apps. It applies to non-EU firms selling into EU markets. Each member state's market-surveillance authority enforces it, so penalties vary by country — [Taylor Wessing](https://www.taylorwessing.com/en/interface/2025/accessibility/the-european-accessibility-act-and-its-implementation); [Davis Wright Tremaine, July 2025](https://www.dwt.com/insights/2025/07/european-accessibility-act-digital-products); [Clifford Chance, May 2026](https://www.cliffordchance.com/content/dam/cliffordchance/briefings/2026/05/bridging-the-accessibility-gap-the-strategic-imperative-of-the-european-accessibility-act.pdf).
- The technical benchmark is usually **EN 301 549**, which references WCAG 2.1 AA and adds requirements for native apps. Some existing products have transition periods to **June 28 2030**. Microenterprises (fewer than 10 staff, under €2M turnover) are partly exempt. "Up to €100,000 per violation in Germany" is a vendor claim and unverified — [Raftlabs (vendor)](https://www.raftlabs.com/blog/european-accessibility-act-guide); [TestParty (vendor)](https://testparty.ai/blog/european-accessibility-act-guide).
- **Apple Accessibility Nutrition Labels** (added to the HIG June 9 2025): App Store listings declare support for **nine features: VoiceOver, Voice Control, Larger Text, Dark Interface, Differentiate Without Color Alone, Sufficient Contrast, Reduced Motion, Captions, Audio Descriptions**. Each has its own evaluation criteria — [App Store Connect Help: Accessibility Nutrition Labels](https://developer.apple.com/help/app-store-connect/manage-app-accessibility/overview-of-accessibility-nutrition-labels/) (fetched); [Apple Design: What's new](https://developer.apple.com/design/whats-new/).
- **Apple HIG Accessibility** (rewritten Mar 7 2025): accessible means *Intuitive, Perceivable, Adaptable*. Let text enlarge by **at least 200%** (140% on watchOS). Uses the WCAG AA contrast table (up to 17 pt: 4.5:1; 18 pt and above: 3:1) and mentions APCA as an alternative measure. Pair audio cues with haptics, respond to Reduce Motion, Dim Flashing Lights, and avoid autoplay without controls — [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) (fetched). In the Dec 2025 update, Dynamic Type gained "emphasized weights" — [What's new](https://developer.apple.com/design/whats-new/).
- **GitHub Primer** ships dedicated high-contrast and colour-vision-deficiency themes (2023) — [GitHub Blog](https://github.blog/engineering/user-experience/unlocking-inclusive-design-how-primers-color-system-is-making-github-com-more-inclusive/).
- **Liquid Glass shows the cost of retrofitting accessibility after launch** (see Q1) — [PhoneArena](https://www.phonearena.com/news/liquid-glass-was-so-bad-that-apple-will-give-you-another-way-to-tone-it-down_id178795).

### Inferences
- A hackathon project can make a credible "EAA/WCAG 2.2-ready" claim by checking 8 things: 4.5:1 text contrast, 3:1 UI contrast, 24 px or larger targets (aim for 44), visible focus that sticky headers don't cover, no CAPTCHA or password-only login (offer a passkey, OTP or magic link), a tap alternative to every drag, auto-filled repeat fields, and support for 200% text and reduced motion.
- Shipping a "Tinted / high-contrast" toggle from day one is a cheap differentiator, since it is the exact fix Apple added after launch.

### Gaps
- Microsoft Inclusive Design toolkit (inclusive.microsoft.design) was blocked. Background knowledge, unverified this session: its "Persona Spectrum" covers permanent, temporary and situational disability (for example one arm / arm injury / new parent holding a baby), with the principles "Recognize exclusion, Learn from diversity, Solve for one, extend to many."
- I could not research Google's 2024–26 accessibility features (for example TalkBack with Gemini image descriptions, Expressive Captions, Guided Frame).
- I could not confirm national EAA penalty amounts or enforcement actions from official sources.

## Q4. Measurement and research practices

### Takeaway
Leading teams pair large-scale experimentation (Duolingo's hundreds of streak experiments, Google's 18,000-participant M3 Expressive studies) with standard frameworks such as HEART and SUS. Since March 2024, Google has treated **responsiveness (INP)** as part of UX quality.

### Cited Findings
- **Core Web Vitals: INP replaced FID on March 12, 2024.** INP looks at the latency of all qualifying interactions during a visit and reports roughly the longest. Search Console switched to INP — [Google Search Central blog](https://developers.google.com/search/blog/2023/05/introducing-inp); [web.dev](https://web.dev/blog/inp-cwv-march-12); [Search Engine Land](https://searchengineland.com/google-core-web-vitals-to-add-interaction-to-next-paint-on-march-12-437072).
- **Current thresholds ("good" / "poor"):** INP ≤ **200 ms** good, > **500 ms** poor. LCP ≤ **2,500 ms**, > 4,000 ms. CLS ≤ **0.1**, > 0.25. INP isn't reported if the user never interacts — [GoogleChrome/web-vitals README](https://github.com/GoogleChrome/web-vitals) (fetched). Google assesses on a 28-day rolling window — [ppc.land](https://ppc.land/interaction-to-next-paint-inp-to-replace-first-input-delay-fid-on-march-12-2024).
- **Experimentation at scale (Duolingo):** 600+ streak experiments over about 4 years. Wins include +3% DAU from streak visibility. CURR is the North Star retention metric — [Lenny's Podcast summary](https://www.recall.it/summary/lennys-podcast/behind-the-product-duolingo-streaks-or-jackson-shuttleworth-group-pm-retention-team); [Econsultancy](https://www.econsultancy.com/six-a-b-tests-used-by-duolingo-to-tap-into-habit-forming-behaviour); [Lenny's Newsletter](https://www.lennysnewsletter.com/p/how-duolingo-reignited-user-growth). The best reminder timing was **about 23.5 hours** after the last lesson — [Econsultancy](https://www.econsultancy.com/six-a-b-tests-used-by-duolingo-to-tap-into-habit-forming-behaviour).
- **Mixed-method research at scale (Google M3 Expressive):** 46 studies combining eye tracking, surveys, focus groups, experiments and usability testing, with 18,000+ participants — [Android Authority](https://www.androidauthority.com/google-material-3-expressive-details-3554486/).
- **Validated design heuristics:** HAX guidelines validated with 49 practitioners across 20 products — [Microsoft Research](https://www.microsoft.com/en-us/research/publication/guidelines-for-human-ai-interaction/).
- **Measuring real outcomes at scale (Airbnb):** the pro-photography uplift (19%) measured across 14,700 versus 62,300 listings — [Airbnb](https://www.airbnb.com/professional_photography).

### Inferences
- Hackathon measurement kit:
  - a 5-user think-aloud usability test, which finds most issues (Nielsen's heuristic; background, unverified this session)
  - a SUS questionnaire before and after the redesign
  - task success rate and time on task for 2–3 core tasks
  - Lighthouse or web-vitals showing INP ≤ 200 ms, LCP ≤ 2.5 s, CLS ≤ 0.1
  - a HEART table of goals, signals and metrics

  This gives judges numbers instead of adjectives.

### Gaps
- Background knowledge, unverified this session (sources blocked):
  - **HEART** (Happiness, Engagement, Adoption, Retention, Task success, used with Goals→Signals→Metrics) comes from Rodden, Hutchinson & Fu, Google, CHI 2010.
  - **SUS** is a 10-item questionnaire (Brooke, 1986). A score of about 68 is commonly cited as average.
  - **Continuous discovery** (weekly customer touchpoints, opportunity solution trees) comes from Teresa Torres' *Continuous Discovery Habits* (2021).
  - Baymard Institute's checkout-usability benchmarks are also relevant.
- I could not reach any company-specific design QA process docs.

## Q5. Craft-level patterns praised in top products

### Takeaway
The 2024–26 craft "canon" includes:
- keyboard-first command menus (cmdk powers Vercel's)
- perceptually uniform, user-tunable theming (Linear)
- spring physics and shape morphing (M3 Expressive)
- specific progress messaging and in-button activity states (Apple)
- streak and feedback loops (Duolingo)
- photo-led trust (Airbnb)

### Cited Findings
- **Command palette:** `cmdk` was "used for the Vercel command menu and autocomplete" from 2020 and rewritten in 2022 — [pacocoursey/cmdk README](https://github.com/pacocoursey/cmdk) (fetched). Third-party analysis describes Linear's style as keyboard-first UX, optimistic UI, command palette, dense layouts and dark mode — [BuildMVPFast (secondary)](https://www.buildmvpfast.com/blog/linear-aesthetic-tokens-density-keyboard-first-ux-2026).
- **Theming / dark mode done properly:** Linear's LCH theme generator (3 inputs instead of 98 variables) and higher-contrast defaults — [Linear blog](https://linear.app/blog/how-we-redesigned-the-linear-ui). Primer's dimmed, high-contrast and colour-vision-deficiency themes — [GitHub Blog](https://github.blog/engineering/user-experience/unlocking-inclusive-design-how-primers-color-system-is-making-github-com-more-inclusive/).
- **Motion and micro-interactions:** M3 Expressive's spring-based motion and 35-shape morphing library — [Android Authority](https://www.androidauthority.com/google-material-3-expressive-features-changes-availability-supported-devices-3556392/). Apple's Liquid Glass motion guidance (Sept 2025) and SF Symbols 7 "Draw" animations — [Apple Design: What's new](https://developer.apple.com/design/whats-new/).
- **Loading and progress states:** Apple recommends showing an activity indicator *inside* the button and changing the label, e.g. "Checkout" → "Checking out…" — [Apple HIG: Buttons](https://developer.apple.com/design/human-interface-guidelines/buttons). For AI waits, specific status copy instead of "Processing…" — [Apple HIG: Generative AI](https://developer.apple.com/design/human-interface-guidelines/generative-ai).
- **Forgiveness and undo as a principle:** "Help people recover from mistakes… Build forgiveness into your design" and "When a guided flow is necessary, make it easy to skip or escape" (relevant to onboarding) — [Apple HIG: Design principles](https://developer.apple.com/design/human-interface-guidelines/design-principles).
- **Reachability:** "it tends to be easier… to reach a control when it's located in the middle or bottom area of the display" — [Apple HIG: Designing for iOS](https://developer.apple.com/design/human-interface-guidelines/designing-for-ios). Apple also prefers full-width primary buttons — [HIG Buttons](https://developer.apple.com/design/human-interface-guidelines/buttons).
- **Gamified habit loops:** Duolingo's streaks, leaderboards and notifications (see Q0/Q4) — [Lenny's Newsletter](https://www.lennysnewsletter.com/p/how-duolingo-reignited-user-growth).
- **Photo-first trust:** Airbnb's professional photos, +19% bookings — [Airbnb](https://www.airbnb.com/professional_photography).
- **Developer onboarding as UX:** Stripe's "seven lines of code" time-to-first-transaction pitch — [Stratrix](https://www.stratrix.com/moat-anatomy/stripe-s-api-moat-in-online).
- **Bold, tactile visual identity (India):** CRED's open-sourced **NeoPOP** design system, its fourth generation, for Web (React), Android, iOS and Flutter. It is Apache-2.0 licensed, but the web repo's last push was Oct 2023 — [Analytics India Mag](https://analyticsindiamag.com/cred-open-sources-its-ui-design-system-neopop/); [CRED-CLUB/neopop-web](https://github.com/CRED-CLUB/neopop-web).

### Inferences
- Five patterns that are cheap to implement and look premium:
  - Cmd/Ctrl+K command palette (cmdk)
  - optimistic UI with undo toasts instead of confirmation dialogs (for reversible actions)
  - skeleton loaders plus specific progress copy
  - spring-based micro-interactions that respect `prefers-reduced-motion`
  - an empty state with example actions or prompts

### Gaps
- Linear, Raycast, Arc, Notion, Figma and Vercel Geist primary docs were blocked. Claims about optimistic UI and sync engines (Linear), Raycast extensions and Arc's spaces and sidebar are not verified this session.
- Background knowledge, unverified: Linear's local-first sync engine makes edits feel instant; Vercel's Geist design system is public at vercel.com/geist.

## Q6. India-specific UX moves (UPI/NPCI, PhonePe, Swiggy, Zomato, CRED, Bhashini)

### Takeaway
Indian UX innovation focuses on **lowering the literacy, language, bandwidth and authentication barriers**:
- voice-first payments and ordering in Indian languages (Hello! UPI with Bhashini, Swiggy with Sarvam)
- PIN-less small payments (UPI Lite)
- on-device biometric approval replacing PINs (NPCI, Oct 2025)
- feature-phone and IVR channels (UPI 123PAY, phone-call ordering)
- vernacular audio confirmations for merchants

### Cited Findings
- **Hello! UPI** (NPCI, launched at Global Fintech Fest, **Sept 2023**): voice payments through UPI apps, telephone calls and IoT devices, starting in Hindi and English. NPCI works with **Bhashini** to bring conversational payments to India's **22 official languages**. The wake phrase is "Hello" plus the app name (e.g. "Hello! BHIM"). Users still enter the PIN manually — [NPCI Hello! UPI](https://npci.org.in/what-we-do/hello-upi/product-overview); [Outlook Money](https://www.outlookmoney.com/banking/ask-and-pay-your-upi-will-work-like-alexa-soon). NPCI's CTO names Bhashini and AI4Bharat as key partners — [NPCI media PDF (Analytics India Mag)](https://www.npci.org.in/PDF/npci/media-coverage/NPCI-is-Exploring-AI-Powered-Futuristic-Payment-Frontiers-CTO_AnalyticsIndiaMag.pdf).
- **UPI 123PAY** (feature-phone UPI): "All current and future experiences for 123Pay on-call shall be using 'Hello! UPI'". Members had to enable Hello! UPI by **March 31, 2024** — [TaxGuru (NPCI circular summary)](https://taxguru.in/rbi/hello-upi-npci-voice-assisted-upi-experience.html). The RBI also raised UPI 123PAY limits in late 2024 — [Outlook Money](https://www.outlookmoney.com/amp/story/news/rbi-enhances-transaction-limits-for-upi-lite-and-upi123pay-know-details).
- **UPI Lite** (PIN-less small payments): the RBI raised limits to **₹1,000 per transaction and ₹5,000 wallet balance**, up from ₹500 and ₹2,000. It was announced Oct 2024 and notified **Dec 4 2024** with immediate effect. No PIN is needed — [Deccan Herald](https://www.deccanherald.com/business/upi-lite-rbi-raises-limit-of-wallet-to-rs-5000-per-transaction-to-rs-1000-3303602); [Outlook Money](https://www.outlookmoney.com/amp/story/banking/rbi-enhances-upi-lite-transaction-limits-rs-1000-per-transaction-and-rs-5000-per-day). NPCI added **auto top-up** for UPI Lite when the balance drops below a threshold — [Outlook Money](https://www.outlookmoney.com/amp/story/banking/changes-in-upi-from-november-auto-top-up-feature-for-upi-lite-wallet-limit-up-to-rs-5000).
- **Biometric UPI** (PIN optional): the NPCI circular of **Oct 7 2025** allows on-device fingerprint or face approval as an optional alternative to the UPI PIN. Biometric data stays on the device, and payments are initially capped at **₹5,000**. Aadhaar face authentication was also enabled for setting or resetting the UPI PIN — [Business Today](https://www.businesstoday.in/amp/personal-finance/news/story/no-more-pins-upi-to-get-face-and-fingerprint-authentication-for-faster-safer-online-payments-497815-2025-10-11); [MobileIDWorld](https://mobileidworld.com/indias-npci-to-launch-biometric-authentication-for-upi-payments-making-pins-optional/). Rollouts: the **BHIM app on March 24 2026** — [IANS](https://ianslive.in/bhim-app-launches-biometric-authentication-for-upi-payments-up-to-rs-5000--20260324134230) — and CRED around March 30 2026 — [Angel One](https://oga-prod.angelone.in/news/personal-finance/cred-launches-biometric-authentication-for-upi-payments). Exact launch dates differ between sources.
- **PhonePe:**
  - The **Indus Appstore** consumer launch (Feb 2024) offered app discovery in **12 Indian languages**, which PhonePe says covers 95% of Indians' language preferences — [Kyodo/PR Newswire](https://kyodonewsprwire.jp/release/202402236945).
  - Indus later added **voice search in 10 Indian languages plus English** — [Outlook Business](https://www.outlookbusiness.com/corporate/phonepes-indus-appstore-launches-voice-search-feature-in-10-indian-languages).
  - Market rationale cited: 57% of Indian users prefer the internet in a vernacular language (IAMAI–Kantar), and vernacular speakers make up about 75% of internet users — [Outlook Business](https://www.outlookbusiness.com/corporate/phonepes-indus-appstore-launches-voice-search-feature-in-10-indian-languages).
  - In 2020 the PhonePe for Business app added **voice payment notifications in 9+ vernacular languages**, so merchants don't need to look at the phone — [PhonePe press](https://www.phonepe.com/press/phonepe-launches-vernacular-voice-notifications-on-its-business-app/).
- **Swiggy × Sarvam AI** (reported March 2026): voice ordering across Food, Dineout and Instamart in **11 Indian languages**. The AI handles discovery, selection and checkout. A **phone-call channel needs no app, download or internet**, and was demoed at the India AI Impact Summit. Swiggy was the first commerce platform on Sarvam's **Indus** chat app, with Razorpay payments inside the conversation. Meesho launched its "Vaani" voice shopping assistant days earlier — [Techloy](https://www.techloy.com/swiggy-introduces-ai-voice-ordering-with-sarvam-ai-across-11-indian-languages/); [Verdict Foodservice](https://www.verdictfoodservice.com/news/swiggy-sarvam-ai-to-launch/); [Yahoo Tech](https://tech.yahoo.com/ai/meta-ai/articles/swiggy-sarvam-ai-launch-multilingual-101651975.html).
- **CRED:** the open-source NeoPOP design system (see Q5) — [Analytics India Mag](https://analyticsindiamag.com/cred-open-sources-its-ui-design-system-neopop/).

### Inferences
- The strongest "Bharat UX" hackathon angle is **voice-first and vernacular, with a non-app fallback** (IVR or WhatsApp), **PIN-less or biometric low-value flows**, and **audio confirmations**. This combines Hello! UPI, UPI Lite, biometric UPI, PhonePe's vernacular notifications and Swiggy's phone-call ordering into one pattern.
- Bhashini (government language APIs) and Sarvam or AI4Bharat models are the natural building blocks for a hackathon prototype that supports 10–22 Indian languages.

### Gaps
- **Zomato:** a search summary said Zomato reported about 150,000 orders per month on its Hindi and regional-language apps in 2022, but I could not tie that to a specific source page. I found no 2025–26 Zomato voice or vernacular launch.
- I could not research **Zepto**, **Google Pay India**, **DigiLocker** or **Bhashini's own usage numbers**. The search budget was used up and Indian government and press domains were blocked.
- Background knowledge, unverified this session:
  - UPI 123PAY launched in March 2022 with four modes: IVR number, app-based feature phones, missed call, and proximity sound-based payments.
  - UPI Lite launched in Sept 2022.
  - The RBI raised the UPI 123PAY per-transaction limit to ₹10,000 in late 2024.
  - DigiLocker is reachable through WhatsApp (MyGov helpdesk).
  - Zepto's UX is built around a 10-minute-delivery promise with a minimal checkout.
  - UPI Circle (2024) lets a primary user delegate payments to family members.
- Verify the latest Hello! UPI language list on NPCI's site.
