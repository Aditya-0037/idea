# UX Problem Spaces for a UI/UX Hackathon (India-focused + global) and Evaluation of the Five Existing Ideas

Research date: 2026-10-10. Method note: ~60 web searches/fetches. Devpost search pages and the GitHub search API were blocked from this environment, so saturation is judged from sampled `site:devpost.com` searches plus inference, not from full result counts. The web-search budget ran out before a few final checks (noted in Gaps).

---

## Q1. How do the five existing ideas hold up? (What exists, where it still fails, originality, evidence of pain, saturation, feasibility, demo-ability)

### Takeaway
None of the five should be built as stated. Each one either goes up against big government products launched in 2025–26 (Samadhan Didi, Mumbai One, RailOne, BHIM 3.0) or fails mostly because of backend problems (fund release, data feeds, content) that a UI can't fix. Ideas 1 and 4 have the strongest evidence of pain. Both become good hackathon projects only if narrowed: Idea 1 to scholarship pre-checks and status transparency, Idea 4 to accessible KYC and onboarding for persons with disabilities, or safe payments for elders.

### Cited Findings

**Idea 1: Unified College Portal (admissions/exams/scholarships wizard)**
- Gujarat Congress (Aug 2026) says over 9 lakh OBC/EBC/DNT students have gone more than six months without PM-YASASVI scholarships. It blames non-receipt of central grants and "technical issues" in the online system and NSP. — [Careers360](https://news.careers360.com/congress-flags-6-month-delay-in-central-scholarships-for-over-9-lakh-gujarat-students-writes-cm)
- In UP's 2025-26 cycle, MP Chandrashekhar Azad wrote that students (including EWS General category) were denied scholarships. He cited disbursement delays, technical glitches and "procedural negligence" as recurring problems. — [The Mooknayak](https://en.themooknayak.com/education/mp-chandrashekhar-azad-writes-to-up-govt-as-2025-26-scholarship-glitches-leave-poor-students-high-and-dry)
- NSP applications go through multi-level verification (institute → district → state → ministry). PFMS can hold a payment even when the status shows "approved". Common blockers: Aadhaar not seeded with the bank account, name mismatch, wrong IFSC, dormant accounts (advisory site, secondary). — [CollegeSimplified](https://www.collegesimplified.in/post/nsp-scholarship-status-stuck-for-30-days-here-s-the-real-reason)
- 2026 cycle: students report "Payment Failed" or stuck statuses, Aadhaar-DBT seeding errors and face-authentication app problems (secondary). — [ValidCollege](https://validcollege.com/news/awareness/nsp-scholarship-portal-2026-students-still-missing-these-benefits-pvj5)
- Bihar post-matric and NMMS scholarships were delayed by tech glitches and staff shortages on the Medhasoft portal (2024). — [Careers360 Bihar](https://news.careers360.com/bihar-post-matric-nmms-sholarship-late-medhasoft-online-application-portal-verification-students-school-documents-required/amp)
- NSP 2025-26 registration for SC/OBC schemes was extended to 19 Dec 2025, which suggests a deadline-driven, last-minute rush. — [Manipur OBC notice](https://manipurobcsc.mn.gov.in/2025/12)

**Idea 2: Government Services Chatbot (voice/text, Hindi/English/regional)**
- **Samadhan Didi**: DARPG launched a CPGRAMS AI voice chatbot built with Bhashini on 30 May 2026. Citizens speak a grievance; it identifies the ministry and category, asks for missing details and routes the grievance. Coverage is reported as the 22 Eighth-Schedule languages, and it targets rural and non-literate users who struggle with forms. — [Drishti IAS](https://www.drishtiias.com/state-pcs-current-affairs/samadhan-didi-ai-voice-chatbot-launched/print_manually); [India Science & Technology (Govt)](https://www.indiascienceandtechnology.gov.in/stihighlights/ai-voice-assistant-%E2%80%98samadhan-didi%E2%80%99-brings-multilingual-access-public-grievance-redressal)
- **Jugalbandi** (OpenNyAI/Microsoft/AI4Bharat) is a WhatsApp assistant that takes text or voice and answers in the user's language. Early reporting: 10 languages and 171 of ~20,000 government programmes. — [Microsoft Source Asia](https://news.microsoft.com/source/asia/features/with-help-from-next-generation-ai-indian-villagers-gain-easier-access-to-government-services/)
- **Bhashini** (MeitY, 2022) offers free translation, ASR and TTS for all 22 scheduled languages; states began integrating it into services by Jan 2026. — [Apolitical](https://apolitical.co/en/navigator/case-studies/india-using-ai-to-make-government-services-available-in-22-languages)
- A government mSeva chatbot already exists. — [mgov ChatBot](https://services.mgov.gov.in/ChatBot)
- **UMANG** had 11.66 crore registered users and ~798 crore transactions over three years, and **DigiLocker** had 72.43 crore registered users (Rajya Sabha, Aug 2026). — [Free Press Journal](https://www.freepressjournal.in/business/digilocker-crosses-7243-crore-users-umang-records-1166-crore-registrations-govt-informs-rajya-sabha). The June 2025 figures were 8.34 crore UMANG users and 53.92 crore DigiLocker users. — [PIB document](https://static.pib.gov.in/WriteReadData/specificdocs/documents/2025/sep/doc2025915636901.pdf)
- UMANG's App Store complaints describe embedded services (especially EPFO) that stop working after you open them. The "UMANG India" iOS listing showed 1.8★ from 30 reviews (thin sample). — [AppFollow UMANG](https://apps.appfollow.io/ios/umang/1236448857?country=in)
- A 2024 study of UMANG (n=252) found ease of use and awareness are key drivers of use. It is an awareness survey, not a task-based usability test. — [SDNBVC paper](https://sdnbvc.edu.in/wp-content/uploads/2024/07/FULLPAPERID03.pdf)
- On Devpost, a search surfaced only one similar project (PolicyPal, a WhatsApp scheme-finder still in the planning stage). — [Devpost PolicyPal](https://devpost.com/software/policypal-x829ds)

**Idea 3: Intuitive Transit Planner (Indian buses/trains/metro)**
- **Mumbai One** (MMRDA) launched 8–9 Oct 2025. It covers 11 operators (suburban rail, Metro 1/2A/3/7, Navi Mumbai Metro, Monorail, BEST, TMT, NMMT, KDMT, MBMT) with a single QR ticket, a multimodal journey planner, live advisories and Marathi/Hindi/English. Suburban season tickets are not included. — [The Week/PTI](https://www.theweek.in/wire-updates/national/2025/10/08/bes22-mh-app-mumbai-one.html); [CurlyTales](https://curlytales.com/india/trending/mumbai-one-app-how-to-use-features-prices-everything-to-know-about-indias-integrated-mobility-app/amp/)
- **RailOne** (CRIS/Indian Railways) launched 1 July 2025. It folds in IRCTC Rail Connect, UTS (unreserved tickets) and NTES (train tracking), plus PNR, coach position, food and Rail Madad. It is rated about 4.7★ on the App Store (~112k reviews). — [Angel One](https://www.angelone.in/news/market-updates/indian-railways-launches-railone-super-app-for-passengers); [AppFollow RailOne](https://apps.appfollow.io/ios/railone/6473384334?country=in)
- **Chalo** offers live bus tracking. Its vendor case study admits "notable gaps in location coverage and the accuracy of key geopoints" in smaller cities, so the limit is data quality, not UI. — [AWS/HERE case study](https://aws.amazon.com/solutions/case-studies/chalo-here/)
- I found no independent, citable dataset of Indian commuter complaints about Chalo, Where is my Train or Google Maps transit (see Gaps).

**Idea 4: Accessible Rural Banking UI (icons, vernacular, voice-over)**
- **BHIM 3.0** (Mar 2025) launched with 15+ languages, growing to 20 by Jul 2025, and is optimised for low connectivity. BHIM still had only 0.23% of UPI volume in Feb 2025. — [Business Standard](https://www.business-standard.com/amp/finance/personal-finance/bhim-3-0-track-manage-split-expenses-with-support-in-15-languages-125032600331_1.html); [ETV Bharat](https://www.etvbharat.com/en/!technology/bhim-1-to-bhim-3-tracking-features-and-functions-of-the-upi-app-enn25072301976)
- **UPI 123PAY** covers ~400M feature-phone users through IVR, missed-call, feature-phone app and sound-based payments. A Nov 2025 Indian Overseas Bank mandate added MissCallPay. — [NPCI](https://npci.org.in/what-we-do/upi-123pay/product-overview); [The Week](https://www.theweek.in/wire-updates/business/2025/11/07/dcm109-biz-brief.html). **Hello! UPI** offers conversational voice payments in English and Hindi. — [TaxGuru](https://taxguru.in/rbi/hello-upi-npci-voice-assisted-upi-experience.html)
- **Supreme Court, 30 Apr 2025** (Pragya Prasun & Ors. v. Union of India): the Court held that digital access is part of the right to life under Article 21. It issued 20 directions to make e-KYC accessible to persons with disabilities. Existing liveness checks (eye-blinking, live photos) exclude blind users and acid-attack survivors. The Court required accessibility audits that include testing with blind users, and the RBI has since amended its KYC Master Direction. — [LiveLaw](https://www.livelaw.in/amp/supreme-court/right-to-digital-access-part-of-article-21-supreme-court-directs-to-make-ekyc-process-accessible-to-persons-with-disabilities-290778); [Vinod Kothari](https://vinodkothari.com/2025/08/supreme-court-mandates-digital-accessibility-action-points-for-banks-and-nbfcs/); [Moneylife](https://moneylife.in/article/supreme-court-issues-20-directions-to-ease-kyc-for-visually-impaired-and-acid-attack-victims/77015.html)
- NCPEDP (Nov 2024): over 90% of Indian finance websites fail accessibility standards. — [People Matters](https://www.peoplematters.in/amp-diversity-over-90-indian-finance-websites-fail-accessibility-standards-43526)
- NSS CAMS 2022–23 (79th round): about 20% of rural and 40% of urban people can send or receive email (secondary summary; verify against MoSPI). — [SuperKalam](https://superkalam.com/current-affairs/17-06-2025/analysing-internet-access-and-digital-skills-in-india-pg7-37c77df9-f396-4b8f-aa00-8e35f94ba86b)
- HCI precedent: in Medhi et al., CHI 2009 (58 Indian participants), non-text money-transfer UIs were strongly preferred, and spoken dialog was faster and needed less help. — [Microsoft Research PDF](https://microsoft.com/en-us/research/wp-content/uploads/2016/02/medhi_chi2009.pdf). Gupta et al. (COMPASS 2022) found that emergent Indian smartphone users often don't understand accounts and passwords, even while doing sophisticated things. — [Microsoft Research](https://www.microsoft.com/en-us/research/?p=839809)
- In a Tamil Nadu study (n=17), seniors named trust in family and usefulness as UPI adoption drivers, and self-efficacy, physical well-being and system complexity as barriers. — [JYX thesis](https://jyx.jyu.fi/jyx/Record/jyx_123456789_95943)

**Idea 5: Localized Learning Hub (story-like vernacular learning)**
- DIKSHA: in a Tamil Nadu survey, only about 40% of secondary students had heard of DIKSHA, and under 35% of those used it to scan textbook QR codes. Teachers used it far more (90% primary, 78% secondary) (opinion piece; undated survey). — [The Bastion](https://thebastion.co.in/politics-and/diksha-the-long-awaited-antidote-to-indias-education-crisis/)
- Delhi NCR (n=180): 15.1% never used DIKSHA and 24.6% rarely did. — [Amity AIJTE 2025](https://www.amity.edu/aien/aijte/articles2025/12%20Exploring%20The%20Utilization%20Of%20The%20Diksha%20Portal%20By%20Pre-Service.pdf). In rural Rajasthan (pandemic-era study), most users had trouble with the portals, mainly because of slow or interrupted internet. — [NCERT IJET](https://journals.ncert.gov.in/IJET/article/view/850)
- ASER 2024: 90% of rural youth have a smartphone at home, 82% know how to use one (31% of those own one), and 76.9% of 14–16-year-olds could set an alarm. — [Ideas for India](https://www.ideasforindia.in/topics/human-development/youth-s-digital-readiness-in-rural-india.html)
- BYJU's entered NCLT insolvency in July 2024, and its valuation fell from $22B (2022) to under $3B. — [Onmanorama](https://www.onmanorama.com/news/business/2024/07/16/startup-byjus-faces-insolvency-proceedings.html). Consumer courts ordered BYJU's to pay damages in refund and deficient-service cases. — [Moneylife/BBC](https://www.moneylife.in/article/bbc-report-questions-byjus-meteoric-rise-in-india/65802.html)

### Inferences

Scorecard (my assessment, 1 = weak and 5 = strong, based on the findings above):

| Idea | Originality | Evidence of pain | Saturation risk (5 = low risk) | Is UX the main lever? | Demo-ability | Verdict |
|---|---|---|---|---|---|---|
| 1. Unified College Portal | 2 | 4 (scholarships) | 2 (college portals/ERPs are common student builds) | 2–3: delays mostly come from fund release, PFMS and verification queues | 4 | **Narrow it**: "Scholarship Pre-flight + Status Explainer" (name/Aadhaar-bank/IFSC consistency check before submission; translate opaque statuses like "Approved at L2, PFMS pending" into plain language with next steps and who to contact) |
| 2. Gov Services Chatbot | 1 | 3 | 1 (Samadhan Didi, Jugalbandi, mSeva chatbot, UMANG, plus "generic chatbot" is a cliché) | 1: the value is in AI and backend integration | 3 | **Avoid**, or reuse only the "conversation design for low-literacy voice" angle inside another idea |
| 3. Transit Planner | 1–2 | 2 (no strong citable complaint data found) | 2 (Mumbai One, RailOne, Chalo, Google Maps) | 1–2: the bottleneck is live data accuracy | 4 | **Avoid** unless narrowed to something like an accessible station-wayfinding flow for first-time or disabled metro riders |
| 4. Accessible Rural Banking | 2 as stated, 4 if narrowed | 5 (SC judgment, NCPEDP, CAMS, HCI literature) | 3 ("vernacular icon banking" is a common pitch; BHIM 3.0/123PAY exist) | 4–5 | 4 | **Pivot**: accessible e-KYC and onboarding for blind/low-vision users and acid-attack survivors (court-mandated, auditable), or a "safe-pay" mode for elders (see P1) |
| 5. Localized Learning Hub | 2 | 3 | 2 (edtech/learning apps are very common student builds) | 2: the impact depends on creating content | 2–3 (story content is hard to show convincingly in a short demo) | **Deprioritize** |

- Overall, the ChatGPT report's ideas are "category labels" rather than sharp problem statements. They map onto spaces where well-funded government products shipped in 2025–26, which makes "we built a cleaner version" hard to defend in front of judges.

### Gaps
- There is no systematic app-store review mining for UMANG, DigiLocker, Chalo, Where is my Train, RailOne or BHIM. Only thin storefront snippets were found; a team could scrape Play Store reviews as primary research.
- No full-text NSP usability study and no official NSP statement on 2025-26 delays were found. The causes come from politicians, the press and advisory sites.
- No independent post-launch reviews of Mumbai One or RailOne were found (coverage is launch-week and promotional).
- PhonePe/Google Pay vernacular strategy and rural usage numbers were not found.
- A reported Delhi High Court notice to ICICI Bank about screen-reader inaccessibility appeared in search summaries but could not be tied to a verified source.

---

## Q2. Which fresh, evidence-backed problem spaces make the strongest shortlist? (8–12 candidates)

### Takeaway
The strongest problem spaces combine (a) hard government or court data on harm, (b) a recent policy trigger that existing apps haven't designed for, and (c) a fix that is mostly flow, clarity, trust or accessibility. Best bets:
- **P1** Digital-arrest/scam interruption for elders and families
- **P2** "Golden-hour" fraud reporting companion
- **P3** Scholarship pre-flight and status transparency
- **P4** Prescription-to-visual-schedule for elders and caregivers
- **P5** DPDP consent-notice design
- **P6** Accessible e-KYC for persons with disabilities
- **P7** Emergency-alert comprehension and trust

These are followed by dark-pattern-free subscriptions, AQI actionability, the ABHA hospital-visit companion, and the grievance case-file builder.

### Cited Findings

**P1/P2. Cyber fraud: digital arrest, elder scams, and reporting (1930 / cybercrime.gov.in)**
- Citizens lost ₹22,845.73 crore to cyber fraud in 2024, up from ₹7,465.18 crore in 2023 (Lok Sabha, Jul 2025). There were 36,37,288 financial-fraud incidents on NCRP+CFCFRMS in 2024 (24,42,978 in 2023) and 22,68,346 cybercrime cases on NCRP in 2024 (+42%). — [The Week/PTI](https://www.theweek.in/wire-updates/business/2025/07/22/del23-lsq-cyber-fraud.html)
- Digital arrest: ₹1,935 crore lost in 2024 across 1.23 lakh complaints; 60,676 incidents/₹339 crore in 2023; 39,925/₹91.14 crore in 2022; 17,718 incidents/₹210.21 crore in Jan–Feb 2025 alone. I4C blocked 83,668 WhatsApp accounts, and 7.81 lakh SIMs and 2.08 lakh IMEIs were blocked by 28 Feb 2025 (MHA in Parliament). — [Inc42](https://inc42.com/?p=504907)
- Typical cases: an 85-year-old retired professor transferred ₹9 crore over 1–22 Dec 2025 after a WhatsApp video call from a man in police uniform. — [The Hitavada](https://www.thehitavada.com/Encyc/2025/12/25/85-yr-old-retired-engineering-professor-loses-rs-9-crore-to-digital-arrest-scam.html). An elderly Chandigarh woman lost ₹2.5 crore to "CBI/Supreme Court" impersonators using forged warrants. — [Tribune](https://www.tribuneindia.com/news/chandigarh/sector-10-elderly-woman-loses-2-5-crore-in-digital-arrest-fraud). A 69-year-old in Gwalior lost ₹1.57 crore over a 33-day "digital arrest" (2026). — [Free Press Journal](https://www.freepressjournal.in/bhopal/69-year-old-retired-health-worker-loses-157-crore-in-33-day-digital-arrest-scam-in-gwalior-fraudsters-posed-as-cbi-officials). A 72-year-old Surat man lost ₹1.47 crore and was kept isolated through continuous video calls. — [Daily Pioneer](https://www.dailypioneer.com/news/72-year-old-surat-man-duped-of-rs-1-47-crore-in-digital-arrest-fraud)
- HelpAge India: the most common scams against seniors in 2025 were digital-arrest threats, AI-generated bank calls, deepfake impersonation of family members, and "OTP forced verification". — [t2online interview](https://t2online.in/tech/interviews/interview-with-helpage-on-cybercrime-and-online-safety-for-senior-citizens-on-safer-internet-day/2003551)
- 45% of surveyed Indian seniors say they struggle to identify online fraud (survey sponsor not named). — [Storyboard18](https://www.storyboard18.com/amp/digital/45-of-indian-seniors-struggle-to-identify-online-fraud-cybercrimes-on-the-rise-58331.htm)
- An RBI discussion paper proposes a one-hour delay on account transfers above ₹10,000, and trusted-person approval for transactions above ₹50,000 by customers aged 70+, with opt-out allowed (proposal, not final). — [Reuters via Yahoo Finance](https://finance.yahoo.com/economy/policy/articles/indias-central-bank-mulls-delay-135740570.html)
- An opinion piece using NSS data describes a "digital safety gap": use is growing faster than people's ability to recognise risk, get help and secure redress. — [ThePrint](https://theprint.in/opinion/from-aadhaar-to-upi-how-indias-digital-rails-can-include-not-exclude-older-adults/3053392/)
- Reporting friction: after 1930 freezes money, Goa victims must still visit a police station to start recovery, and officials say they are "working on simplifying" the return process. — [Herald Goa](https://www.heraldgoa.in/?p=400584). Mumbai police say most unrecovered money is lost because victims realise too late. One firm recovered ₹11.20 crore of ₹11.34 crore because staff called 1930 immediately. — [The Week](https://www.theweek.in/wire-updates/national/2025/04/13/bom9-mh-cyber-crime.amp.html)
- Sanchar Saathi's Chakshu flags suspicious calls, SMS and WhatsApp messages, but actual money fraud must be reported separately via 1930 or cybercrime.gov.in, which splits the reporting journey. The order to pre-install Sanchar Saathi on all phones was withdrawn after privacy objections. — [Tribune explainer](https://www.tribuneindia.com/news/explainers/explainer-the-sanchar-saathi-specifics)
- A parliamentary reply said over ₹1,200 crore had been saved across 4.7 lakh-plus complaints through the CFCFRMS/1930 system (cumulative at reply date). — [eParliament](https://eparlib.nic.in/bitstream/123456789/2974939/1/AU509.pdf)
- Existing student builds (Devpost sample): ScamShield, ElderShield, Cyber Guardian, WiseGuard, ScamShield Seniors, Safebook and ScamSpot. Almost all are "paste a message/URL → get a verdict" checkers or phishing quizzes, mostly Western- or Singapore-framed. — [ScamShield](https://devpost.com/software/scamshield); [ElderShield](https://devpost.com/software/tech-alchemists); [Cyber Guardian](https://devpost.com/software/cyber-guardian); [WiseGuard](https://devpost.com/software/wiseguard); [ScamShield Seniors](https://devpost.com/software/scamshield-seniors)

**P3. Scholarship and document-consistency chaos (NSP, DigiLocker)**
- See the Idea 1 findings (Gujarat 9 lakh students delayed; UP glitches; multi-level verification; Aadhaar-bank seeding and name-mismatch failures).
- DigiLocker fetch failures happen when a document isn't seeded by the issuer, or when roll number, year or board don't match official records exactly. — [Setu support](https://support.setu.co/support/solutions/articles/81000412444-you-are-not-able-to-fetch-a-doc-and-getting-400-bad-request); [Careers360 Q&A](https://www.careers360.com/question-i-want-my-passing-certificate-from-digilocker-but-it-is-not-fetching-and-cannot-find-records-what-should-i-do). A Jul 2026 user account describes unexplained "mismatch" errors for PAN, DL and RC, with a grievance reply that just repeated the refusal (single anecdote). — [Counterview](https://www.counterview.in/2026/07/)

**P4. Prescriptions, medicines and elder care**
- Punjab & Haryana High Court (Oct 2025): legible prescriptions and diagnoses are part of the right to health under Article 21. Doctors must write in capital letters until prescriptions are digitised, and the court set a two-year timeline for digital prescriptions. The IMA says rural practitioners still largely handwrite. — [Business Standard](https://www.business-standard.com/health/fix-handwriting-shift-to-digital-prescriptions-high-court-tells-doctors-125100600501_1.html); [EWN](https://www.ewn.co.za/2025/10/03/indian-high-court-demands-doctors-fix-illegible-handwriting)
- Polypharmacy affects 33.7% of 600 older adults across six Indian cities, linked to multimorbidity, care transitions and hospitalisation. — [PubMed 39900582](https://pubmed.ncbi.nlm.nih.gov/39900582/). In rural Kerala it is 14.6%, with 86.5% "good" adherence (Morisky scale). — [IJCM via DOAJ](https://doaj.org/article/510aff8304e44b039ac517b067c40709). The national SAGE analysis (n=2,840 NCD patients) found 51% average medication adherence, with multimorbidity the strongest predictor of non-adherence. — [Frontiers in Pharmacology 2023](https://public-pages-files-2025.frontiersin.org/journals/pharmacology/articles/10.3389/fphar.2023.1183818/text)
- UNFPA India Ageing Report 2023: people aged 60+ will grow from 149M (10.5%) in 2022 to 347M (20.8%) in 2050, and will outnumber children by 2046. The 80+ group grows about 279% (2022–2050) and is mostly widowed, dependent women. Over 40% of elders are in the poorest wealth quintile and 18.7% have no income. — [Scroll](https://scroll.in/latest/1056724/indias-ageing-population-to-double-by-2050-says-un-report); [Drishti IAS](https://www.drishtiias.com/daily-updates/daily-news-analysis/india-ageing-report-2023/print_manually)

**P5. Consent and privacy-notice comprehension (DPDP Rules 2025)**
- The DPDP Rules were notified on 14 Nov 2025. Rule 3 requires the consent notice to be understandable on its own, written in clear and plain language, list the personal data item by item, state specific purposes, and link to withdrawal, rights and complaint routes. Withdrawing consent must be comparable in ease to giving it. Rule 4 (consent managers) takes effect after 1 year, and Rule 3 after 18 months. — [Mondaq](https://www.mondaq.com/india/data-protection/1708164/digital-personal-data-protection-rules-2025-notified); [The Leaflet](https://theleaflet.in/amp/story/explainer/indias-new-digital-personal-data-protection-rules-2025-a-detailed-reading); [KPMG](https://assets.kpmg.com/content/dam/kpmgsites/in/pdf/2025/11/dpdp-rules-2025-guidance-to-dpdp-act-implementation.pdf)
- Under Section 6(3) of the DPDP Act, consent requests must offer English or any of the 22 Eighth-Schedule languages. — [Certinal](https://www.certinal.com/blog/multilingual-consent-under-dpdp-act)

**P6. Dark patterns, subscription traps and checkout drip pricing (consumer protection)**
- The CCPA dark-pattern guidelines define a subscription trap as making cancellation impossible, lengthy or hidden, and drip pricing as price elements revealed late or after confirmation. In June 2025 the CCPA told platforms to self-audit within 3 months; 26 platforms submitted declarations by Nov 2025. Penalties against 7 platforms total about ₹20 lakh (e.g., Zepto ₹7 lakh for basket sneaking and drip pricing), and analysts say self-regulation has had limited effect. — [The Policy Edge](https://www.policyedge.in/p/ccpa-dark-pattern-cases-bring-20-lakh-in-penalties-and-interface-changes); [Outlook Business](https://www.outlookbusiness.com/amp/story/news/inside-indias-dark-pattern-crackdown-why-zepto-bookmyshow-and-others-are-under-ccpa-scanner); [Bar & Bench](https://www.barandbench.com/amp/story/law-firms/view-point/from-nudge-to-notice-what-indias-dark-pattern-orders-mean-for-digital-business)
- E-commerce made up 36.1% of National Consumer Helpline grievances in 2023-24 (4.45 lakh, up from 2.05 lakh in 2020-21). Flipkart had over 1.6 lakh, Amazon 58,875 and Meesho 20,953. — [MediaNama](https://www.medianama.com/2025/07/223-national-consumer-helpline-8500-e-commerce-complaints/). Between Apr and Dec 2025 the NCH handled 67,265 refund complaints, about 40,000 of them e-commerce. — [Storyboard18](https://www.storyboard18.com/how-it-works/consumer-affairs-dept-facilitates-rs-45-cr-refunds-in-8-months-as-e-commerce-tops-complaints-86672.htm)

**P7. Accessible e-KYC and onboarding for persons with disabilities**
- See the Idea 4 findings: the SC judgment of 30 Apr 2025 (digital access under Art. 21; 20 directions; liveness and blink checks exclude users; accessibility audits with blind users), RBI's KYC amendment, and NCPEDP's finding that over 90% of finance websites fail. — [LiveLaw](https://www.livelaw.in/amp/supreme-court/right-to-digital-access-part-of-article-21-supreme-court-directs-to-make-ekyc-process-accessible-to-persons-with-disabilities-290778); [Vinod Kothari](https://vinodkothari.com/2025/08/supreme-court-mandates-digital-accessibility-action-points-for-banks-and-nbfcs/); [People Matters](https://www.peoplematters.in/amp-diversity-over-90-indian-finance-websites-fail-accessibility-standards-43526)

**P8. Emergency alert comprehension and trust (SACHET cell broadcast)**
- India's nationwide cell-broadcast test on 2 May 2026 caused confusion. Many users wondered if the "Emergency Alert" was a scam, and the advance advisory wasn't widely seen. The message read "Please ignore these message(s); no action is required." SACHET geo-targeted SMS is live in all 36 states and UTs for cyclones, floods and earthquakes. — [Inc42](https://inc42.com/buzz/what-is-the-cell-broadcast-alert-system-tested-by-india/); [The Statesman](https://www.thestatesman.com/india/phones-blare-loud-alert-govt-says-dont-panic-its-just-a-nationwide-safety-test-1503588643.html); [Patna Press](https://patnapress.com/india-emergency-alert-test-siren-message-mobile-phones-ndma/)

**P9. Air quality actionability (AQI)**
- Gaps in CPCB Sameer app data led many Delhi users to delete it and look for alternatives (Nov 2025). — [Newslaundry](https://www.newslaundry.com/amp/story/2025%2F11%2F05%2Fdelhis-double-whammy-air-getting-toxic-aqi-data-under-cloud)
- People deliberately ignore bad news when they feel they can't act on it; air pollution is a cited example. Evidence from India shows people with a sense of control are less likely to avoid the information. — [VoxDev (Apr 2026)](https://voxdev.org/topic/health/why-bad-news-ignored-and-how-effectively-communicate-risk)
- An IIIT survey reports 88% awareness of AQI but only 33% understanding of PM2.5 and its health effects (blog with a placeholder title; verify). — [IIIT Hyderabad blog](https://blogs.iiit.ac.in/?p=28779)
- People often don't follow air-quality advice, and simply telling them about high-pollution episodes doesn't work (KCL trial protocol). — [ClinicalTrials.gov protocol](https://ClinicalTrials.gov/ProvidedDocs/98/NCT03552198/Prot_SAP_000.pdf). In a UK Defra study, users wanted advice that is focused, concise and jargon-free, without being vague. — [Defra report](https://uk-air.defra.gov.uk/assets/documents/reports/cat14/1210261047_Individuals_interpretation_of_air_quality_information_customer_insight_&_awareness_study.pdf)

**P10. Hospital visits and health records (ABHA/ABDM)**
- More than 104 crore health records are linked to over 93 crore ABHA accounts (Jul 2026). Doctors can see past records only with time-bound, revocable patient consent. — [Drishti IAS](https://www.drishtiias.com/daily-updates/daily-news-analysis/ayushman-bharat-health-accounts-abha/print_manually)
- ABHA "Scan & Register" (formerly Scan and Share) has crossed 25 crore OPD registrations across 30,800 facilities in 756 districts. — [BioVoice News](https://biovoicenews.com/abha-scan-register-25-crore-opd-registrations/). An IIHMR study, as reported, found OPD wait fell from about 1 hour to 2–5 minutes (secondary). — [RAU's IAS Compass](https://compass.rauias.com/current-affairs/abha-based-scan-and-share-service/). Some hospitals now require ABHA-based OPD registration, e.g., G.B. Pant Hospital, Andaman & Nicobar, Apr 2026. — [Nicobar Times](https://nicobartimes.com/?p=27005)

**P11. Grievance and complaint filing (CPGRAMS, consumer, municipal)**
- Samadhan Didi (May 2026) covers voice-based CPGRAMS filing (see Idea 2). The NCH volumes above show the scale of consumer grievances. The 1930 journey splits into Chakshu, then 1930/portal, then a police-station visit (see P1/P2).

**Lower-evidence spaces checked (not shortlisted)**
- Women's safety apps: in the 2016 Chennai "Shakthi" field test (n=50), 7% never opened the app and 61.5% opened it only 1–2 times a week. — [OII paper](https://blogs.oii.ox.ac.uk/ipp-conference/sites/ipp/files/documents/HARSHINI_DR_VELAYUTHAM_SHAKTHI_INDIA.pdf). 112 India is the unified emergency app. — [NavBharat Live](https://navbharatlive.com/technology/womens-day-2026-every-woman-should-have-these-3-safety-apps-himmat-app-e-rakshak-app-112-india-app-1596412.html). No national usage data was found.
- Blue-collar jobs: e-Shram had 31.78 crore registered workers (Jul 2026) and integrates with the NCS job portal. — [Corpseed](https://www.corpseed.com/news/e-shram-platform-registers-31-crore-workers). No citable data on job scams was found.

### Inferences

**Shortlist: one card per problem space.** "Wow UX" ideas are my design suggestions. Saturation ratings come from sampled Devpost searches where available and are otherwise inferred.

**P1. "Pause & Verify": interrupting a digital-arrest or scam call while it's happening (elders + family)**
- Users: people aged 60+ (especially those living alone, retired or pensioned) and their adult children.
- Evidence: very strong (₹1,935 crore lost to digital arrest in 2024, roughly 7x the 2022 number of cases; crore-level losses by retired people; HelpAge's scam list).
- What existing tools get wrong: Chakshu and 1930 are report-after-the-fact. Student builds are "paste message → verdict" checkers that assume the victim is calm and doubtful. Digital-arrest victims are kept on continuous video calls, isolated and frightened.
- Wow UX:
  - A one-tap "Is this real?" panic card ("No police/CBI ever arrests on video call") in big type, the user's language and voice.
  - A silent "call my person" trusted-contact ping, in the spirit of the RBI's trusted-person proposal.
  - A friction screen before large transfers that names the scam script ("They told you to keep this secret? That is the scam").
  - A scenario simulator so families can rehearse.
- Saturation: medium overall, low for the India-specific "during-the-scam" and family-loop angle.
- Demo-ability: very high (role-play a live scam call on stage).

**P2. "Golden Hour" fraud reporting companion (after the scam)**
- Users: fraud victims in their first hour, often panicking.
- Evidence: strong (36.4 lakh financial-fraud incidents in 2024; Mumbai's ₹11.2 crore recovered thanks to an immediate call; the Goa recovery bottleneck).
- What existing tools get wrong: the journey is split across Chakshu, 1930, cybercrime.gov.in and a police-station visit. Victims don't know what evidence to collect (transaction IDs, UTRs, screenshots), and the steps after a freeze are opaque.
- Wow UX:
  - A calm countdown step-by-step flow (call 1930 now, then collect these 5 items, then file at the portal).
  - An auto-assembled "complaint pack" PDF.
  - A status-explainer timeline (freeze → police → refund order).
  - Pairs naturally with P1 as one "before/during/after" fraud journey.
- Saturation: low.
- Demo-ability: high.

**P3. Scholarship "Pre-flight & Pipeline" (narrowed Idea 1)**
- Users: SC/ST/OBC/EWS/minority students, often first-generation college students.
- Evidence: strong (9 lakh students delayed in Gujarat; recurring glitches in UP and Bihar).
- What existing tools get wrong: errors surface weeks later, through multi-level verification and PFMS. Statuses are opaque, and the root causes (name mismatch across Aadhaar, bank and marksheet; unseeded accounts) can be prevented.
- Wow UX:
  - A document-consistency checker that highlights a mismatched spelling before submission.
  - A visual pipeline (Institute → District → State → Ministry → PFMS) with a "who to call" at each stage.
  - Status jargon translated into plain Hindi or English.
- Saturation: medium (scholarship finders exist; pre-flight and status design is rarer).
- Demo-ability: high.

**P4. Prescription → visual dose schedule for elders and caregivers**
- Users: elders with multiple conditions and their caregivers.
- Evidence: strong (P&H HC order; 33.7% urban polypharmacy; 51% adherence in SAGE; 347M elders by 2050).
- What existing tools get wrong: generic reminder apps assume the user can read and type prescriptions. Pharmacist and doctor instructions stay text-only and English.
- Wow UX:
  - A pill-photo plus time-of-day "dose card" (sun/moon icons, before/after food) printable for the fridge.
  - A multilingual audio explanation.
  - A caregiver dashboard with "missed dose" alerts.
  - Can use mock digital prescriptions, since the HC is pushing digitisation.
- Saturation: high for "medicine reminder" (inferred; very common student app), low for the prescription-comprehension plus caregiver angle.
- Demo-ability: high.

**P5. "Consent you can actually read": a DPDP Rule 3 consent-notice pattern kit**
- Users: every Indian app user, with app teams as the secondary audience.
- Evidence: strong regulatory trigger (Rules notified 14 Nov 2025). By my calculation Rule 3 takes effect around May 2027, so apps are redesigning now.
- What existing tools get wrong: walls of legal text, English-only, consent bundled together, and withdrawal harder than giving consent.
- Wow UX:
  - A layered notice (itemised data chips → purpose → "withdraw anytime" mirror button).
  - A 22-language toggle.
  - A personal "consent dashboard".
  - A before/after comparison of a real app's consent screen.
- Saturation: low.
- Demo-ability: high. Pure design, little backend, which suits a UX hackathon very well.

**P6. Dark-pattern X-ray / "Cancel as easy as subscribe"**
- Users: online shoppers and subscribers.
- Evidence: medium-strong (CCPA guidelines, self-audits and penalties; e-commerce is 36% of NCH grievances).
- What existing tools get wrong: drip pricing, basket sneaking and buried cancellation still persist, and the penalties are small.
- Wow UX:
  - Side-by-side redesigns of real Indian checkout and cancel flows, scored against the CCPA list.
  - Optionally a browser-overlay concept that annotates dark patterns.
- Saturation: low-medium.
- Demo-ability: high (before/after is very visual).

**P7. Accessible e-KYC & onboarding (narrowed Idea 4)**
- Users: blind and low-vision users, acid-attack survivors, people with motor disabilities.
- Evidence: very strong (Supreme Court directions; NCPEDP over 90% failure; RBI KYC amendment).
- What existing tools get wrong: blink and selfie liveness checks, CAPTCHA and OTP timeouts, and unlabeled buttons.
- Wow UX: a screen-reader-first KYC flow with alternative liveness (voice or thumb-impression image, as the SC directions allow), long timeouts and haptic guidance, demoed with TalkBack/VoiceOver live.
- Saturation: low.
- Demo-ability: high (run a screen reader on stage), and it maps directly to "accessibility" judging criteria.

**P8. Trustworthy emergency alerts (SACHET/cell-broadcast message design)**
- Users: everyone, especially non-English speakers and elders.
- Evidence: medium (the May 2026 test caused panic and "is this a scam?" confusion).
- What existing tools get wrong: alerts are text-heavy, hard to verify and don't tell you what to do.
- Wow UX:
  - An alert design system: severity colour and icon, one action verb, multilingual audio, and a "how to verify this alert is official" panel.
  - A companion "what to do now" card for flood, cyclone or heatwave.
- Saturation: low (disaster apps exist, inferred; alert-message design is rarely attempted).
- Demo-ability: high (simulate an alert).

**P9. AQI → "What should I do today?"**
- Users: urban parents, outdoor workers, people with asthma.
- Evidence: medium (Sameer trust gaps; information avoidance; 88% aware vs 33% understanding).
- What existing tools get wrong: they show numbers first, with no personal action. Hopelessness drives people to ignore them.
- Wow UX: action-first cards ("Walk to school before 8am; mask N95; keep windows shut 4–8pm"), "control" framing, and a household profile.
- Saturation: medium-high (AQI dashboards are a common student build, inferred; e.g., seeO2 on GitHub — [GitHub seeO2](https://github.com/narmis99/seeO2)).
- Demo-ability: high.

**P10. ABHA "visit companion" (OPD wayfinding + records + consent)**
- Users: patients and attendants at government hospitals.
- Evidence: medium-strong on scale (25 crore scan registrations; 104 crore records), weak on citable usability complaints.
- What existing tools get wrong: they stop at the token, so the department hunt, test queues, reports and consent requests stay confusing.
- Wow UX: a single visit timeline (token → room → tests → pharmacy) and a plain-language consent request card ("Dr X wants 30 days of access to your lab reports").
- Saturation: medium (hospital-queue apps are common, inferred).
- Demo-ability: medium-high.

**P11. Grievance "case file" builder & tracker**
- Users: citizens filing consumer, municipal or CPGRAMS complaints.
- Evidence: medium (NCH volumes; the fragmented 1930 flow).
- What existing tools get wrong: they don't help users structure evidence, there's no single tracker across portals, and replies are jargon.
- Wow UX: a guided "what happened → evidence → desired outcome" builder that outputs a portal-ready text, plus a reply translator.
- Saturation: medium (grievance portals are common in SIH-style hackathons, inferred). Samadhan Didi now covers voice filing.
- Demo-ability: medium.

**Suggested ranking for a UI/UX hackathon (inference):**
1. P1+P2 combined fraud journey
2. P7 accessible e-KYC
3. P5 DPDP consent kit
4. P3 scholarship pre-flight
5. P4 prescription dose cards
6. P8 emergency alerts
7. P6 dark-pattern X-ray
8. P9 AQI actions
9. P10 ABHA visit companion
10. P11 grievance builder

Women's safety, blue-collar jobs and hostel/mess admin aren't shortlisted because of weak citable evidence or saturation.

### Gaps
- An unverified claim that the Supreme Court observed more than ₹3,000 crore siphoned through digital-arrest scams by Nov 2025 (and ordered a CBI probe in Dec 2025) appeared in search summaries. It couldn't be confirmed against a primary source before the search budget ran out.
- No official full-year 2025 digital-arrest or NCRP total was found. The latest firm figures are for calendar 2024 and Jan–Feb 2025.
- There is no data on the share of frozen 1930 money eventually returned to victims.
- No India-specific study of consent-notice comprehension, AQI app behaviour, or SACHET alert comprehension was found.
- Fake-job scams targeting blue-collar workers (Apna, NCS) and campus hostel/mess admin had no citable evidence in this pass.
- Saturation counts are qualitative. Devpost and GitHub search APIs were blocked, so counts of similar projects per idea couldn't be measured.
- A reported Himmat app figure of about 31,000 users and claims that "lack of awareness" limits women's-safety apps appeared in summaries but couldn't be pinned to verified sources.

---

## Q3. What are the documented global UX pain areas in 2025–2026?

### Takeaway
Globally, the documented pain clusters are: fraud against older adults, digital accessibility (lawsuits and the EU's new legal mandate), AI-generated answers replacing source-checking, subscription-cancellation dark patterns (with US federal regulation stalled), and patient portals that older adults find low-value and hard to use. All five have Indian counterparts, which lets an India-focused project also cite global relevance.

### Cited Findings
- **Elder fraud (US):** the FBI IC3 2024 report recorded $16.6B in losses across about 859,000 complaints (+33%). — [CyberInsider](https://cyberinsider.com/fbi-reports-record-breaking-16-6-billion-in-cybercrime-losses-in-2024/). People aged 60+ filed 147,127 complaints with $4.885B in losses, up about 46% and 43% (FBI data as reported). — [Erie News Now](https://www.erienewsnow.com/story/52849817/fbi-warns-of-rising-elder-fraud-ahead-of-awareness-day)
- **Digital accessibility lawsuits (US):** UsableNet counted 2,019 filings in H1 2025 and projected about 20% growth over 2024. The 2025 year-end total was reported as over 5,000 (federal + state), with e-commerce the target in 69%. — [Newswire / UsableNet](https://www.newswire.com/news/digital-accessibility-lawsuits-surge-in-2025-22618502); [Fox Rothschild](https://www.foxrothschild.com/events/ada-website-lawsuit-trends-what-2025-filings-mean-for-2026)
- **European Accessibility Act:** enforceable since 28 June 2025 for e-commerce, consumer banking, e-communications and transport ticketing. Some self-service terminals have until 2030. — [Davis Wright Tremaine](https://www.dwt.com/insights/2025/07/european-accessibility-act-digital-products)
- **AI summaries replacing verification:** Pew (Mar 2025 browsing data; 900 US adults; 68,879 searches) found click-through falls from 15% to 8% when a Google AI summary appears. Only 1% of visits clicked a cited source, and 26% of sessions ended after an AI summary vs 16% without. — [Pew Research](https://www.pewresearch.org/short-reads/2025/07/22/google-users-are-less-likely-to-click-on-links-when-an-ai-summary-appears-in-the-results/)
- **Subscription dark patterns (US):** the Eighth Circuit vacated the FTC "Click-to-Cancel" rule on 8 Jul 2025, on procedural grounds, days before it took effect. State laws such as California's still apply. — [Morgan Lewis](https://www.morganlewis.com/pubs/2025/07/ftcs-click-to-cancel-rule-vacated-ahead-of-planned-july-14-effective-date); [Womble Bond Dickinson](https://www.womblebonddickinson.com/us/insights/alerts/ftcs-click-cancel-rule-vacated-remember-it-was-not-alone)
- **Patient portals and older adults:** in interviews with 19 adults aged 65+ (spring 2025), participants saw low usefulness and felt portals serve providers' efficiency more than patients' needs. — [PMC12763363](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12763363/). A dental-hospital portal scored a mean SUS of 63.3, with older and culturally/linguistically diverse users doing worse. — [PMC12352587](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12352587/). In a Michigan poll, 78% of people aged 50–80 had used a portal, but only 57% felt very confident navigating one. — [LeadingAge](https://leadingage.org/?p=358340)
- **Older adults generally:** NN/g's newer research on people aged 65+ notes that digital literacy is rising, but designs must still accommodate age-related challenges. — [NN/g author listing](https://www.nngroup.com/articles/author/lexie-kane/)

### Inferences
- A project that cites both Indian and global data (e.g., P1 elder fraud: I4C plus FBI IC3; P7 accessibility: the SC judgment plus the EAA and ADA lawsuits; P5 consent: DPDP plus dark-pattern law) can argue it is "locally grounded, globally relevant", which tends to impress judges.
- "AI answer trust" (Pew) suggests a possible differentiator: any AI-assisted feature (e.g., a prescription explainer) should show sources and confidence visibly. That is a UX-craft talking point.

### Gaps
- I didn't pull Baymard checkout statistics, global government-form usability data (e.g., US/UK digital service reports), or 2025–26 trust surveys on AI answers. Pew measured behaviour, not trust.
- I couldn't read the full NN/g 2025 older-adults article (only listings).

---

## Q4. Which ideas best fit a UI/UX hackathon judged on research, empathy, accessibility, usability and visual craft?

### Takeaway
The best fits are problems where (1) the harm is human and vivid (empathy), (2) a recent law or court order defines what "good" looks like (a research hook), (3) the solution is a flow redesign that can be prototyped in Figma or the front end without real integrations, and (4) a live before/after or role-play demo is possible. P1/P2, P7, P5, P3 and P4 meet all four. The original Ideas 2, 3 and 5 meet the fewest.

### Cited Findings
- Court and regulatory definitions of good UX that a team can audit against:
  - SC e-KYC accessibility directions (Apr 2025) — [LiveLaw](https://www.livelaw.in/amp/supreme-court/right-to-digital-access-part-of-article-21-supreme-court-directs-to-make-ekyc-process-accessible-to-persons-with-disabilities-290778)
  - DPDP Rule 3 plain-language, itemised notice with easy withdrawal — [Mondaq](https://www.mondaq.com/india/data-protection/1708164/digital-personal-data-protection-rules-2025-notified)
  - CCPA dark-pattern list, where visually equivalent cancel/decline options are expected — [The Policy Edge](https://www.policyedge.in/p/ccpa-dark-pattern-cases-bring-20-lakh-in-penalties-and-interface-changes)
  - P&H HC legible-prescription order — [Business Standard](https://www.business-standard.com/health/fix-handwriting-shift-to-digital-prescriptions-high-court-tells-doctors-125100600501_1.html)
- HCI evidence for low-literacy design choices: non-text and spoken interfaces are preferred and faster. — [Medhi et al., CHI 2009](https://microsoft.com/en-us/research/wp-content/uploads/2016/02/medhi_chi2009.pdf)
- Literacy constraints to design for: about 20% of rural and 40% of urban people can email (CAMS, secondary). — [SuperKalam](https://superkalam.com/current-affairs/17-06-2025/analysing-internet-access-and-digital-skills-in-india-pg7-37c77df9-f396-4b8f-aa00-8e35f94ba86b)

### Inferences
- Judging alignment (my mapping):
  - **Research**: P1/P2 (I4C/MHA data), P3 (news + verification-chain analysis), P5/P6/P7 (laws as heuristics).
  - **Empathy**: P1 (retirees losing their life savings), P3 (students without fees), P4 (elders and caregivers).
  - **Accessibility**: P7 (screen-reader demo), P4/P8 (multilingual, audio, icons).
  - **Usability**: P2/P3 (task flows with measurable time and error reduction).
  - **Visual craft**: P5, P6 and P8 lean on information design (layered notices, severity systems, before/after).
- Recommended research artifacts per project: 5–8 quick interviews (grandparents, scholarship students, hostel peers), a Play Store review-mining table for incumbents (UMANG, DigiLocker, BHIM, Sanchar Saathi), a heuristic audit against the relevant law, and a SUS or task-time test of the prototype against the incumbent flow.
- Feasibility: all shortlisted ideas can be demoed with mock data. None needs real bank, UPI, 1930 or ABHA integration, which keeps the team's effort on design quality rather than backend.

### Gaps
- The actual Hyperbloom judging rubric wasn't available in this research. The alignment above assumes the criteria given in the brief.

---

## Q5. Which ideas are over-saturated in student hackathons and should be avoided or differentiated?

### Takeaway
Sampled Devpost searches confirm heavy saturation for food-waste apps and mental-health journaling/mood trackers. Elder-scam projects are already moderately common, but they cluster as generic "paste text → verdict" checkers. Government chatbots are few on Devpost, but in India they are now directly duplicated by official tools (Samadhan Didi, Jugalbandi). Avoid generic to-do, fitness, campus-event, food-waste, journaling and chatbot apps. If you enter a moderately saturated space (scams, medicine reminders, AQI), differentiate on a specific Indian user moment and a policy hook.

### Cited Findings
- Food waste: one `site:devpost.com` search returned at least 9 distinct projects (No Food Waste, Bungkus-in, uFood, Consume, Pantry Pal, Zero-Waste Recipes, Nourpact, Wasteless, FoodStop), mostly expiry trackers, recipe generators and donation matchers. — [Devpost No Food Waste](https://devpost.com/software/no-food-waste-ifvjcz); [Pantry Pal](https://devpost.com/software/pantry-pal-0u8y67); [Wasteless](https://devpost.com/software/wasteless-fxsoj4)
- Mental-health journaling: one search returned at least 8 projects (CalmMate, journa, ReflectAI, Jot, My Journal, JournAll, Gratreat, MoodLogger), almost all mood-emoji + journal + chart, often with GPT prompts. — [CalmMate](https://devpost.com/software/calmmate); [ReflectAI](https://devpost.com/software/reflectai-64j25i); [MoodLogger](https://devpost.com/software/moodlogger-reflect-record-your-day)
- Elder scam protection: at least 7 projects, mostly message/URL verdict checkers or phishing quizzes. — [ScamShield Seniors](https://devpost.com/software/scamshield-seniors); [Cyber Guardian](https://devpost.com/software/cyber-guardian); [ScamSpot](https://devpost.com/software/scampot)
- Government scheme chatbot: only one Devpost hit (PolicyPal, planning stage). — [Devpost](https://devpost.com/software/policypal-x829ds). Official equivalents now exist: Samadhan Didi (May 2026) and Jugalbandi. — [Drishti IAS](https://www.drishtiias.com/state-pcs-current-affairs/samadhan-didi-ai-voice-chatbot-launched/print_manually); [Microsoft](https://news.microsoft.com/source/asia/features/with-help-from-next-generation-ai-indian-villagers-gain-easier-access-to-government-services/)
- Smart India Hackathon scale: over 250 problem statements from 54 ministries and organisations in SIH 2024, and institute-level internal hackathons grew from over 900 (2023) to over 2,247 (2024). This means a large pool of Indian student teams building gov-service and portal ideas. — [News On AIR](https://www.newsonair.gov.in/7th-smart-india-hackathon-to-begin-on-dec-11); [PIB/Education Ministry](https://education.gov.in/sites/upload_files/mhrd/files/PIB2081437.pdf)
- SIH has included women's-safety and fraud-against-women problem statements (e.g., 2020). — [AICTE SIH 2020](https://aicte.gov.in/sites/default/files/sih2020.pdf)

### Inferences
- Avoid outright:
  - to-do and productivity apps
  - generic fitness trackers
  - mental-health journaling/mood trackers
  - food-waste/expiry trackers
  - campus event apps
  - generic multilingual gov chatbots
  - generic women's-safety SOS apps (SOS button + location share is the default student pattern, and usage evidence is poor)
  - generic transit planners
  - generic "learning app for rural students"
- Differentiation rules for moderately saturated spaces:
  1. Anchor to a specific Indian moment, e.g., "during a digital-arrest video call", not "scam detection".
  2. Anchor to a new law or court order (SC e-KYC, DPDP Rule 3, CCPA, P&H HC prescriptions) and use it as the evaluation heuristic.
  3. Design for a second actor (family member, caregiver, trusted person), since most student builds are single-user.
  4. Show measured usability gains against the incumbent (task time, errors, SUS), not just a pretty UI.
  5. Make AI optional and transparent rather than the headline.
- Saturation summary (inferred for unsampled items):
  - High: food waste, journaling, to-do, fitness, campus events, generic chatbots, medicine reminders, AQI dashboards, women's-safety SOS.
  - Medium: elder scam checkers, scholarship finders, hospital queue apps, grievance portals.
  - Low: digital-arrest interruption plus family loop, golden-hour fraud reporting, DPDP consent design, accessible e-KYC, emergency-alert message design, dark-pattern redesign audits, prescription-to-dose-card for caregivers.

### Gaps
- No quantitative per-theme project counts (Devpost and GitHub search were blocked from this environment). A team could run Devpost searches manually to confirm before committing.
- No published analysis of the most repeated SIH or Indian college-hackathon themes was found. Saturation claims for Indian hackathons are inferred from SIH scale and common student patterns.
