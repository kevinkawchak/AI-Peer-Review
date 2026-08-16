## Claude-Code-Opus-5-15Aug26.md

The Status of AI Peer Review as a Replacement for Human Review in Journal Publishing
A SMART-Framed Review of the 2026 Evidence (through mid-August 2026)

Preliminary Note on the Premise
Before applying the SMART framework, one finding must be stated plainly, because it conditions everything that follows: as of mid-August 2026, no established, indexed scholarly journal has replaced human peer review with an artificial intelligence (AI) process. What has been replaced — substantially, measurably, and in some cases without editorial consent — are the ancillary functions surrounding review: integrity screening, manuscript triage, reviewer identification and invitation, error detection, and review-quality coaching. The evaluative judgment itself, and the accept/reject decision, remain human at every venue of consequence.
The fully autonomous venues that do exist in 2026 (discussed in Section 6) are new entrants built from scratch, not conversions of existing titles. This distinction matters for any strategic planning built on this review, and it is treated as a finding rather than a caveat.

The SMART Framework Applied
Criterion
Question posed
2026 verdict
Specific
What exactly is proposed for replacement?
Partially specified. Four distinct layers are conflated in public discourse; only layers 1–2 have been genuinely automated.
Measurable
Is there quantitative evidence of parity?
Yes, and it is now substantial — the single largest change since 2025. Evidence is mixed but no longer anecdotal.
Achievable
Is full replacement technically and institutionally attainable?
Technically approaching feasibility on detection; institutionally blocked on accountability, and actively undermined by demonstrated gameability.
Relevant
Does replacement address the actual bottleneck?
Partially. The bottleneck is reviewer supply against submission volume — which AI both relieves and worsens.
Time-bound
Is there a dated pathway to replacement?
No venue or publisher has published a target date for autonomous decision-making. The 2027 pipeline is explicitly supplementary.


1. SPECIFIC — Defining What "Replacement" Means
The 2026 literature has converged on a layered taxonomy, articulated most cleanly in Google's Paper Assistant Tool (PAT) work, which situates AI review tools on a four-level scale from author-side pre-submission tools (Level 1) upward toward decision-making authority [2]. Synthesizing across the year's deployments, four distinct functions are at stake:
Layer 1 — Integrity and desk screening. Detection of image manipulation, fabricated references, paper-mill signatures, and undisclosed generative content. Status: substantially replaced. Springer Nature reported that more than 1.5 million papers passed through workflows supported by nearly 60 AI tools during 2025, with a further 25 percent increase projected for 2026; its Snapp peer-review platform is now used by more than half of its journals, and the Geppetto and SnappShot tools pre-screen the majority of submissions [5].
Layer 2 — Reviewer identification and matching. Status: substantially replaced at some publishers, in one documented case over the objection of the handling editor (Section 6) [21].
Layer 3 — Generation of the review report itself. Status: piloted at very large scale, always as a labeled supplement.This is the layer where 2026's decisive experiments occurred [1][23][24].
Layer 4 — The accept/reject decision. Status: not replaced anywhere in mainstream publishing. AAAI states explicitly that it "will continue to rely solely on humans for paper decisions," in compliance with its Code of Professional Ethics and Conduct [22].
The policy literature confirms that publishers themselves draw the line at Layers 3–4. A cross-disciplinary analysis of 439 high-impact-factor and 363 middle-impact-factor journals found that the proportion holding an explicit position on AI in peer review rose from 77 to 83 percent, with 24.5 percent of high-impact journals revising their policies within a single six-month window [4]. A parallel survey of 111 leading AI/NLP conferences and medical journals found substantial divergence between communities but convergence within them on the principle that AI must not author the evaluative judgment [3]. Among top medical journals prohibiting AI in review, 96 percent cite confidentiality as the governing reason [3]. Nature Portfolio's specialty editorials reinforce the same principle: the user of an AI tool "is always accountable," every output "requires human validation," and use must be declared transparently in the review report [6].
Assessment against S: Partially met. The functions being automated are now well specified in the technical literature, but public and institutional discourse continues to conflate Layer 1 automation with Layer 4 replacement — a conflation that inflates perceived progress.

2. MEASURABLE — The 2026 Evidence Base
This is where 2026 differs categorically from prior years. Three large studies, one randomized field trial, and two adversarial evaluations now permit quantitative assessment.
2.1 The AAAI-26 AI Review Pilot — the largest deployment on record
The AAAI-26 pilot remains the reference implementation and the most effective large-scale deployment to date [1]:
Scale: an AI review was generated for every one of the 22,977 papers that entered the full-review stage of the main technical track, drawn from close to 30,000 initial submissions against a program committee scaled to over 28,000 members.
Throughput and cost: the full corpus was processed in under 24 hours at under $1 per paper.
Architecture: a frontier OpenAI reasoning model (gpt-5, "high" reasoning effort) under a Zero Data Retention agreement, with olmOCR preprocessing of PDFs to Markdown and five parallel review modules inspecting story, presentation, and evaluations, the last executed against a Python code sandbox. Output followed a fixed structure and carried APA-formatted references.
Guardrails: every report was explicitly labeled as AI-generated, contained no numeric scores and no accept/reject recommendation, and Senior Program Committee members and Area Chairs were instructed to cross-check AI-surfaced issues against human reviews rather than defer to them.
Reception: across 5,834 survey responses from authors, PC, SPC, and AC members, AI reviews were preferred to human reviews on 6 of 9 criteria, with statistically significant advantages (p < 0.01) in identifying technical errors and raising previously unconsidered points. Preference was strongest among authors and weaker among decision-makers.
Failure profile: the pipeline's advantage was largest on "story" flaws (+0.3203) and "evaluation" flaws (+0.2390), and collapsed on deep domain roots (7.6 percent of cases), where a decade-deep specialist connecting a paper to an obscure prior technique could not be matched. Free-text feedback emphasized factual errors and misreadings.
Citation integrity: in a sample of 100 generated reviews containing 1,356 citations, 1,346 (99.3 percent) were verified as valid, matched to published work with corresponding authors and titles.
2.2 Expert adjudication against Nature-family review
A 45-scientist study across the physical, biological, and health sciences spent 469 hours rating 2,960 individual criticisms drawn from human and AI reviews of 82 Nature-family papers, scoring each on correctness, significance, and sufficiency of evidence [7]. Findings:
Current AI reviewers are competitive with the top-rated human reviewer in Nature's official peer review on the composite measure, producing a significantly higher fraction of qualifying review items per paper.
AI reviewers surfaced a distinct 26 percent of issues that no human raised, with particular strength in cross-reference checking and code-level inspection.
AI reviewers produced more factually incorrect items than humans — the persistent counterweight.
2.3 Error detection: Google's Paper Assistant Tool
PAT was evaluated against the SPOT benchmark of manuscripts containing verified mistakes that led to errata or retractions [2]:
Zero-shot Gemini 3.1 Pro: 55.2 percent; PAT: 89.7 percent — a 34-point improvement attributable to the engineered pipeline rather than raw model capability.
Pilot deployments at STOC 2026 and ICML 2026 covered over 4,700 submissions, identifying significant theoretical errors in more than one-third of ICML papers and prompting 31 percent of authors to run new experiments.
Author reception: 97 percent (STOC) and 92.1 percent (ICML) would use it again; 85.1 and 87 percent respectively reported improved clarity.
Critically, PAT is positioned at Level 1 — a tool authors run on their own manuscripts before submission [2]. Its effectiveness is therefore evidence for AI improving inputs to peer review, not for replacing it.
2.4 Triage and screening validity
Two 2026 studies establish that AI performs respectably at ranking but not at deciding. A comparative analysis at the American Journal of Sports Medicine concluded in its title that "Artificial Intelligence Cannot Replace Peer Reviewers but May Help Editors Triage" [9]. Independently, a training-free, prompt-only manuscript score (AIPR) validated against 300 ICLR submissions separated rejected from accepted papers with AUROC 0.82 (95% CI 0.78–0.87), rising monotonically across decision tiers and tracking mean reviewer rating, with signal concentrated in the lowest-scoring quintile [8]. The paper's title — Intelligence Is Not the Bottleneck — captures the year's central lesson: model capability is no longer the limiting factor.
2.5 The most effective implementation of all: AI coaching human reviewers
Published in Nature Machine Intelligence in 2026, the Review Feedback Agent represents, in this reviewer's assessment, the highest-yield implementation demonstrated to date [10]. Rather than generating reviews, it uses multiple LLMs to give reviewers private feedback on vague comments, content misunderstandings, and unprofessional remarks before authors see the review. Deployed as a randomized controlled study over more than 20,000 reviews, with submissions randomly assigned to receive feedback on none, half, or all of their reviews, and with automated LLM guardrails gating every piece of feedback:
27 percent of reviewers who received feedback updated their reviews, incorporating over 12,000 suggestions.
Reviews became measurably more informative, and reviewer–author engagement increased.
This design is instructive because it inverts the replacement premise: the AI never evaluates the science, and the human retains full authorship and accountability. It is also the only 2026 intervention with a randomized field design at scale.
2.6 Counter-evidence: the case against automation
Three 2026 results argue directly against Layer 3–4 replacement:
The hivemind effect and paper laundering. A position paper comparing human and AI reviews at ICLR 2026 documented excessive agreement within and across papers, reducing perspective diversity, and showed that AI review scores are trivially gameable — prompting an LLM to rewrite a paper significantly increases the scores it receives [11].
Adversarial repackaging. Modifying only presentation-level content — abstract, contribution framing, related work, discussion, narrative structure — while leaving methods, experiments, figures, equations, proofs, and numerical results untouched achieved a 75.1 percent attack success rate with a mean score gain of +1.21/10across three mainstream AI reviewers. No hidden text and no prompt injection were required [12].
Prompt injection. Where invisible instructions were embedded (white text on white background), acceptance rates across tested models rose to between 99.2 and 100 percent, from a baseline of zero [3].
2.7 Illicit substitution: what happens when replacement is unauthorized
The year's defining scandals concern AI review deployed without sanction.
ICLR 2026. The conference received 19,525 valid submissions; 779 were desk-rejected and 5,042 withdrawn, leaving 13,763 decisions based on 76,139 reviews from 18,054 reviewers [13]. An independent analysis by Pangram Labs flagged 21 percent of reviews (approximately 15,899) as fully AI-generated, with over half showing some AI involvement, at a claimed false-positive rate of 1 in 10,000; of 58 cases where authors independently accused a review of being AI-generated, 50 (86.2 percent) had been flagged [14]. The vendor sells detection tools and therefore has a commercial interest in the result — a caveat that should be carried forward. ICLR separately implemented hallucinated-reference detection, with every flagged paper reviewed by at least three humans and an appeals channel [13].
ICML 2026. The conference embedded hidden watermark instructions in every submission PDF, drawn from a 170,000-phrase dictionary, causing any LLM processing the paper to emit telltale phrases. Pre-deadline tests exceeded 80 percent success against frontier models; every flagged review was manually verified at a family-wise error rate of 0.0001. The outcome: 795 reviews removed (1 percent of the total) and 497 papers desk-rejected (2 percent of submissions), since a reviewer's violation is grounds for rejecting papers that reviewer co-authored [15][16]. NeurIPS 2026 adopted a comparable prompt-injection approach [19].
The enforcement drew significant criticism, characterized as designing "a trap that presumes bad faith" and treating reviewers as suspects [19].
2.8 The volume signal
An editorial analysis of 6,957 submissions and 10,389 reviews at Organization Science between 2021 and 2026 documented a 42 percent rise in submissions since the release of ChatGPT, alongside declining writing quality, with AI-generated writing accounting for nearly all of both trends — a collapse of the quality–quantity trade-off driven by submission growth outpacing review infrastructure [17]. Retraction data point the same way: the retraction rate reached approximately 0.2 percent in 2025, up from 0.02 percent in 2016, with compromised peer review and paper mills together accounting for 43 percent of retractions and compromised peer review alone for 37 percent [20].
Assessment against M: Met. For the first time, parity claims can be tested rather than asserted. The measured result is complementarity with asymmetric failure modes, not equivalence.

3. ACHIEVABLE — Technical and Institutional Feasibility
What is achievable now
Integrity screening, triage ranking, reference verification, code and cross-reference checking, error detection at 89.7 percent against verified-error benchmarks, and review-quality coaching are all demonstrated at production scale in 2026 [1][2][5][10].
What is not achievable
Three barriers are structural rather than capability-limited.
Accountability cannot be delegated. Springer Nature's editorial principles state that human accountability cannot be transferred to AI systems and that AI may support but not replace scholarly judgment [5]; Nature Portfolio specialty editorials say the same [6]. Elsevier bans AI at all stages of peer review and editorial decision-making, including auxiliary tasks such as language improvement [3]. JAMA has closed off AI in peer review outright [25].
Gameability is unresolved and worsening. The adversarial results in Section 2.6 show that a defended AI reviewer can be moved more than a full point on a ten-point scale without altering any scientific content [12].
Equilibrium effects punish naive adoption. A three-sided equilibrium model of editors, authors, and reviewers finds that when AI capability crosses a critical threshold, reviewer effort collapses discontinuously: authors use AI to polish submissions while reviewers use it to generate plausible reports without evaluative effort [18]. The model's policy implication is counterintuitive and directly relevant to publisher strategy: before the transition, editors should tighten acceptance standards to curb rent-dissipating polishing; after it, editors must loosen standards while investing in detection, because further tightening amplifies dissipative polishing without improving sorting. Monitoring and loosened selectivity are complements, not substitutes [18].
Assessment against A: Not met for Layers 3–4. Full replacement is not achievable in 2026 on institutional grounds independent of model capability, and the adversarial surface is expanding faster than defenses.

4. RELEVANT — Does Replacement Address the Real Bottleneck?
The bottleneck is reviewer supply against submission volume. Editors now contact 20 to 30 potential experts to secure two completed evaluations [29]. Submissions at major venues have grown steeply — ICLR from 7,304 in 2024 to 11,672 in 2025 to 19,814 in 2026, with reviewers recruited from the pool of submitting authors [13][14]; AAAI roughly doubling to near 30,000 [1].
AI is both cause and proposed cure. The 42 percent submission increase attributable to generative writing tools [17] is the same force that makes the reviewer shortage acute. Automating review to absorb AI-generated volume is a treadmill argument unless coupled with incentive reform.
Relevance is further complicated by the displacement of editors rather than reviewers. In June 2026, Michael Okun, associate professor of neuroscience at the University of Nottingham and an associate editor of Frontiers in Systems Neuroscience, resigned after journal officials told him the publisher's Artificial Intelligence Research Assistant (AIRA) could not be switched off. AIRA had issued its own reviewer invitations in parallel with his, and revoked all of his manually issued invitations to domain experts once one of AIRA's invitees accepted. Okun characterized these as "intentional features, designed to essentially remove the human editors as much as possible." A second editor, Shuzo Sakata of the University of Strathclyde, reported the system inviting a reviewer after he had already decided to reject a manuscript [21].
This is the closest documented case in 2026 of AI displacing a human function inside an established journal — and it concerns reviewer selection, not reviewer judgment.
Assessment against R: Partially met. AI addresses throughput but not the incentive structure generating the volume, and the most consequential real-world displacement to date was of editorial discretion, not of reviewing labor.

5. TIME-BOUND — The 2026 Timeline and the 2027 Pipeline
2026 milestones
Date
Event
January 2026
ICMJE issues revised recommendations with a new AI section; JAMA, NEJM, The Lancet, BMJ and member-aligned journals treat it as the baseline [25]
March 2026
JAAI launches, claiming to be the first fully autonomous academic journal [26]
18 March 2026
ICML publishes its watermark enforcement results: 795 reviews removed, 497 papers desk-rejected [15]
25 March 2026
Nature reports the watermark detection publicly [16]
31 March 2026
ICLR publishes its 2026 review-process retrospective [13]
April 2026
AAAI-26 pilot results released [1]; Organization Science editorial published [17]
May 2026
45-scientist expert adjudication of AI reviews released [7]
June 2026
Okun resigns from Frontiers in Systems Neuroscience over AIRA [21]; adversarial repackaging results published [12]
July 2026
Nature reports Biology Open's payment results [28]; 18 associate editors resign from Statistics and Computing [33]
August 2026
111-venue policy and quality survey published [3]; JAMA formalizes its prohibition on AI in peer review [25]

The 2027 pipeline is explicitly supplementary
AAAI-27 will continue the pilot with a revised system. AI-generated reviews and summaries will contain no ratings or recommendations, will be visible to assigned reviewers only after they submit their own reviews, and will play no formal role in decisions, which remain solely human [22].
NeurIPS 2026 is running a voluntary, author-opt-in randomized experiment with three arms — no LLM assistance, open-ended assistance, structured assistance — integrated into OpenReview. The assistant is explicitly "not intended to replace reviewer judgment or produce a review on the reviewer's behalf," and all other LLM use is unsanctioned and may trigger desk rejection. The Position Paper Track bans AI in review entirely [23].
EMNLP 2026 is running an opt-in experiment with ReviewerToo (Mila, ServiceNow Research, HEC Montréal, Polytechnique Montréal, Université de Montréal, Unified Sciences), built on GPT-OSS-120B with literature-grounded multi-stage generation. AI reviews are visible only to authors and AI Review Chairs, are posted after the author-response period of the ARR May 2026 cycle, and play no role in decisions [24].
Assessment against T: Not met. No venue, publisher, or funder has published a dated target for autonomous decision-making. Every announced 2027 program reaffirms human decision authority.

6. Journals Replaced by AI Peer Review: The Actual Record
Three categories exist, and only the second involves anything that could be called replacement.
6.1 Fully autonomous venues — new entrants, not replacements
JAAI (jaai.pub), established March 2026, describes itself as "the world's first fully autonomous academic journal," with the slogan "AI writes. AI reviews. AI publishes," and states that no human hand touches the peer review process. Its inaugural volume contains 35 research articles [26].
AISC 2026, hosted on the aiXiv platform, states that it is the first venue at which every stage — from peer review to final acceptance decisions — is performed entirely by AI agents, with zero human involvement in the review pipeline. It accepts research papers and proposals across all disciplines, permits submission through a web portal or an Agent API, and publishes all reviews, discussions, and decision rationale openly [27].
These are genuinely novel and are the only venues in 2026 that have literally replaced human review. They are also new titles with no prior human-reviewed history, no evidence of Scopus, Web of Science, or PubMed indexing, and no impact factor. They have not displaced any existing journal. They are best characterized as demonstrations of feasibility and as a test bed for the science of automated review, not as substitutes for established venues.
6.2 Partial displacement inside established journals
The Frontiers/AIRA case (Section 4) is the documented instance of AI replacing a human editorial function at a real, indexed journal against the wishes of the person displaced [21]. Springer Nature's deployment is far larger by volume but explicitly retains human oversight throughout [5].
6.3 Journals contracting under AI-generated submission load
Rising volumes of undisclosed LLM-generated commentaries and letters have forced journals to suspend article types and issue retractions [20]. This is AI pressuring journals, not reviewing for them.
6.4 Summary
No journal has been replaced by the AI peer review process. Any planning document, grant application, or strategy paper asserting otherwise is not supported by the 2026 record. The defensible statement is narrower and still significant: AI has replaced integrity screening and reviewer matching at scale, has been deployed as a labeled supplementary reviewer across more than 22,000 papers at a single venue, and has fully replaced human review only at newly created, unindexed venues built for that purpose.

7. Initiatives Constituting an "AI Peer Review Takeover"
Five distinct initiative types are active in 2026, pushing in different directions.
Venue-led supplementary pilots. AAAI-26 and its AAAI-27 continuation [1][22], NeurIPS 2026's three-arm randomized experiment [23], and EMNLP 2026's opt-in author-feedback study [24]. Common design signature: labeled output, no scores, no recommendations, no decision role, author consent where feasible. This is the mainstream trajectory.
Publisher-led workflow automation. Springer Nature's ~60 tools, Snapp, Geppetto, and SnappShot, covering more than 1.5 million papers with a further 25 percent expansion planned for 2026 [5]; Frontiers' AIRA, which is the most aggressive in displacing editorial discretion [21]. This is where actual replacement is occurring.
Platform-led autonomous publishing. JAAI [26] and aiXiv/AISC 2026 [27] — the only genuine "takeover" initiatives, operating entirely outside established publishing.
Vendor and laboratory tooling. Google's PAT, positioned as an author-side pre-submission tool [2]; the OpenAI–AAAI partnership underpinning the AAAI-26 pipeline [1]; ReviewerToo from the Mila-led consortium [24].
Counter-initiatives. These are as consequential as the adoption programs. Elsevier's blanket prohibition on AI at all stages of review and editorial decision-making [3]; JAMA's outright bar [25]; the ICMJE January 2026 recommendations establishing disclosure as a shared baseline across hundreds of member-aligned journals [25]; enforcement regimes at ICML and NeurIPS [15][19]; and a position paper arguing that today's AI systems should not be used to produce paper reviews at all, grounded in the hivemind and laundering results [11].
The honest characterization is that there is no coordinated takeover initiative. There is a rapid, uncoordinated expansion of automation at Layers 1–2, a carefully fenced set of experiments at Layer 3, an explicit prohibition at Layer 4, and a small autonomous fringe operating outside the system entirely.

8. How the Payment System May Change
8.1 The current position
Peer review remains overwhelmingly unpaid, and the economic critique — that reviewers validate the science while publishers capture the revenue — is now mainstream rather than marginal [36][35]. The push for compensation is driven by measurable scarcity: 20 to 30 invitations per two completed reviews [29].
8.2 The 2026 evidence that payment works
Journal / venue
Payment
Measured effect
Biology Open
$284 per review
Time to first editorial decision cut by 85 percent; reviews returned in 4.6 business days versus 38; quality maintained; being rolled out more widely [28][35]
Critical Care Medicine
$250 to half of 715 invited reviewers
Acceptance 53 percent versus 48 percent; reviews completed one day faster [35]
advances.in/psychology
$100 per review; editors also paid
Funded from a $1,950 APC ($450 for commentaries); founded by Jonas Kunst, University of Oslo, expressly to close the gap between who does the work and who is paid [29][31]
The ResearchHub Journal (ISSN 3070-3395)
$150 in ResearchCoin per review, paid within 7 days
Open marketplace in which qualified reviewers self-select papers rather than being assigned [30]
Open Biology
APC-redeemable tokens
Non-cash credit model [35]

The editor-in-chief case for payment, as reported by Nature, rests on the Biology Open result: dramatically faster decisions with sustained review quality [28].
8.3 The funder lever — the most consequential structural change
The NIH's tiered allowable-publication-cost policy, effective for new and competing awards from 1 January 2026, permits up to $3,000 per publication only where peer reviewers are compensated and reviews are shared openly, against a lower baseline cap otherwise. The $1,000 increment is explicitly premised on a typical journal paying three reviewers $300 each [32].
This is the first instance of a major public funder making reviewer compensation a condition of reimbursement. It converts payment from a publisher's discretionary experiment into a revenue-relevant compliance question, and it establishes $300 as a de facto public benchmark for the value of one review.
8.4 Counter-pressure on the APC model
The same year saw APC increases trigger organized editorial revolt. Eighteen associate editors of Statistics and Computing announced resignations effective 31 December 2026 after Springer Nature moved the journal to full open access from 2027 with a $2,990 APC, calling the decision "irreconcilable with our vision of science" and noting that "the exploitation still remains" [33]. Separately, 23 of 31 Communications in Algebra editorial board members resigned in March 2026 [33]. Any payment model funded from higher APCs will meet this resistance.
8.5 On the claim that post-doctoral researchers are now paid instead of journals
This proposition requires careful separation of what is established from what is emerging.
What is established in 2026. A small but growing set of journals pays per-review honoraria in the $100–$284 range, with a crypto-denominated variant at $150 and a funder-implied benchmark of $300 [28][30][31][32][35]. At least one publisher pays both editors and reviewers out of the APC [31]. Post-doctoral researchers and other early-career researchers are disproportionately represented in this labor pool — it is common for established researchers to involve postdocs and junior assistants in review as training, and journals have introduced formal co-review recognition initiatives partly because quality review remains time-consuming and uncompensated, depressing engagement [34].
What is not established. There has been no redirection of journal revenue to post-doctoral researchers in place of publishers. Payments are per-review honoraria, not salary or income replacement. APCs continue to flow to publishers; in the advances.in model the APC merely funds the honoraria. A large-scale, industry-wide shift to direct monetary compensation has not occurred [35]. Any statement that post-docs "now get paid for their works, instead of journals" overstates the 2026 record substantially.
The decisive economic tension. The AAAI-26 pilot generated a complete, labeled review for under $1 per paper [1]. Human reviews are being priced at $100–$300. That is a two-to-three order of magnitude cost differential for the commodity portion of review labor — first-pass error detection, reference verification, presentation critique — which is precisely the portion where AI performs best [1][2][7]. No rational payer will pay $300 for work that costs under $1, once the substitution is judged acceptable.
The implication for compensation design is therefore the opposite of the intuitive one. AI does not create a broad market for paid post-doctoral reviewing; it collapses the price of the commodity pass while raising the scarcity value of what AI demonstrably cannot do: deep-domain adjudication (the 7.6 percent of cases where AI failed against specialists [1]), resolution of conflicting evidence, and — decisively — the accountable signature that no publisher will delegate [5][6]. The plausible 2027–2028 equilibrium is fewer paid human review slots at a substantially higher unit price, concentrated at the adjudication layer, with the first pass automated. Whether post-docs capture that value depends entirely on whether they hold the deep-domain expertise the market will still pay for — which argues for compensation frameworks tied to adjudication and accountability rather than to review volume.
A supporting theoretical result. The equilibrium model of editorial design finds that as AI capability rises, editors must purchase monitoring — detection capability — as a complement to loosened selectivity [18]. In budget terms, publisher spending is being pulled toward detection and verification infrastructure, and this competes directly with any budget line for reviewer honoraria. The two reforms most often advocated together — pay reviewers, and deploy AI screening — are in partial fiscal conflict.

9. Risk Register
Risk
2026 evidence
Severity
Undisclosed AI review at scale
21 percent of ICLR 2026 reviews flagged as fully AI-generated [14]
High
Adversarial gaming without prompt injection
75.1 percent attack success, +1.21/10 via presentation-only edits [12]
High
Prompt injection
99.2–100 percent acceptance under hidden instructions [3]
High
Homogenization of judgment
Hivemind effect documented across papers [11]
High
Factual error injection
AI produces more factually incorrect items than humans [7]
Moderate–High
Erosion of reviewer trust through covert enforcement
Watermark and prompt-injection traps drew sustained criticism [19]
Moderate
Editorial discretion overridden by automation
AIRA revoking editor-issued invitations [21]
Moderate
Confidentiality breach
96 percent of prohibiting medical journals cite this [3]
Moderate
Volume treadmill
+42 percent submissions, declining quality [17]
High


10. Recommended SMART Goals for the Next Cycle
Framed as testable objectives rather than aspirations, and calibrated to the 2026 evidence:
Goal 1 — Adopt Layer 1–2 automation with a documented editorial override. Specific: deploy integrity screening and reviewer matching with a mandatory, always-available editor override. Measurable: 100 percent of automated reviewer invitations reversible by the handling editor; zero editor-issued invitations auto-revoked. Achievable: the technology is in production [5]. Relevant: directly prevents the failure that caused the year's only editorial resignation over automation [21]. Time-bound: within one editorial cycle.
Goal 2 — Deploy reviewer coaching before deploying reviewer substitution. Specific: implement a Review Feedback Agent–equivalent that critiques reviews without evaluating science. Measurable: target the published benchmark of 27 percent of coached reviewers revising their reviews [10]. Achievable: validated by randomized field trial. Relevant:improves review quality without transferring accountability. Time-bound: one submission cycle, with a randomized design to permit causal inference.
Goal 3 — Publish supplementary AI reviews under the AAAI-27 guardrail set. Specific: labeled reports, no numeric scores, no accept/reject recommendation, no decision role, released to reviewers only after their own submission [22]. Measurable: survey response volume and per-criterion preference against human review, replicating the AAAI-26 instrument [1]. Time-bound: one cycle, with pre-registered stopping criteria.
Goal 4 — Establish reviewer compensation at the funder-implied benchmark, conditional on adjudication rather than volume. Specific: pay at or near $300 per adjudicating review, publish review reports openly, and claim the higher allowable-cost tier [32]. Measurable: time to first decision, benchmarked against Biology Open's 85 percent reduction [28]; reviewer acceptance rate, benchmarked against Critical Care Medicine's 53 versus 48 percent [35]. Relevant:addresses reviewer scarcity while positioning for funder policy. Time-bound: aligned to the funder policy year, with explicit accounting for the APC-increase resistance documented at Statistics and Computing [33].
Goal 5 — Purchase monitoring capability in proportion to automation. Specific: budget detection and verification alongside any AI review deployment, and loosen rather than tighten acceptance thresholds post-transition, per the equilibrium result [18]. Measurable: detection coverage rate and verified false-positive rate, following the ICML precedent of manual verification at a family-wise error rate of 0.0001 [15]. Time-bound: concurrent with, not subsequent to, deployment.

11. Conclusion
Judged against the SMART framework, the proposition that AI peer review is replacing human review of journal publications fails on Specificity in public discourse, succeeds decisively on Measurability, fails on Achievability at the evaluative layer, is only partially Relevant to the underlying bottleneck, and is entirely unbounded in Time.Two of five criteria are met.
The year's genuine achievement is not replacement but instrumentation. In 2026 the field acquired, for the first time, the measurement apparatus to adjudicate the question: a 22,977-paper deployment with a 5,834-response survey [1], a 469-hour expert adjudication of 2,960 individual criticisms [7], a randomized trial across 20,000 reviews [10], a verified-error benchmark moved from 55.2 to 89.7 percent [2], and a policy census spanning 802 journals and 111 venues [3][4].
What that apparatus shows is consistent across studies: AI reviewers are competitive with strong human reviewers on error detection and surface roughly a quarter of issues humans miss, while producing more factual errors, converging on homogeneous judgments, and remaining trivially gameable by an author who changes nothing but the framing. These are not the properties of a replacement. They are the properties of a powerful, cheap, unreliable, and adversarially exposed complement — which is precisely how every serious venue has deployed it.
The most consequential number in this review is not an accuracy figure. It is $1 per paper [1], set against $100–$300 per review [28][30][32][35]. That ratio, not model capability, will determine how peer review is paid for. It will not make post-doctoral researchers the beneficiaries of journal revenue; it will compress the paid human contribution toward the narrow band of deep-domain adjudication and accountable signature that AI has demonstrably failed to reach — the 7.6 percent of cases where a decade-deep specialist still wins [1], and the accountability that no publisher has been willing to delegate [5][6].

References
@article{biswas2026aaai26,
  author = {Biswas, Joydeep and Schoepp, Sheila and Vasan, Gautham and Opipari, Anthony and Zhang, Arthur and Hu, Zichao and Joseph, Sebastian and Lease, Matthew and Li, Junyi Jessy and Stone, Peter and Wagstaff, Kiri L. and Taylor, Matthew E. and Jenkins, Odest Chadwicke},
  title = {{AI-Assisted Peer Review at Scale: The AAAI-26 AI Review Pilot}},
  journal = {arXiv preprint arXiv:2604.13940},
  year = {2026},
  month = {April},
  eprint = {2604.13940},
  archivePrefix = {arXiv},
  primaryClass = {cs.DL},
  url = {https://arxiv.org/abs/2604.13940},
  note = {Largest live deployment of AI-generated peer review to date: 22,977 papers, under 24 hours, under \$1 per paper, 5,834 survey responses},
}

@article{jayaram2026pat,
  author = {Jayaram, Rajesh and Tyler, Drew and Woodruff, David and Cortes, Corinna and Matias, Yossi and Mirrokni, Vahab and Cohen-Addad, Vincent},
  title = {{Towards Automating Scientific Review with Google's Paper Assistant Tool}},
  journal = {arXiv preprint arXiv:2606.28277},
  year = {2026},
  month = {June},
  eprint = {2606.28277},
  archivePrefix = {arXiv},
  primaryClass = {cs.DL},
  url = {https://arxiv.org/abs/2606.28277},
  note = {SPOT benchmark accuracy raised from 55.2\% to 89.7\%; pilots at STOC 2026 and ICML 2026 covering over 4,700 submissions; source of the four-level automation taxonomy},
}

@article{fichtl2026across,
  author = {Fichtl, Alexander M. and Ellinger, Lukas and Kelber, Josefin and Ol{\'i}k, Kry{\v{s}}tof and Groh, Georg},
  title = {{AI-Assisted Peer Review Across Research Communities: From Reviewer AI Policies to LLM Review Quality}},
  journal = {arXiv preprint arXiv:2608.03581},
  year = {2026},
  month = {August},
  eprint = {2608.03581},
  archivePrefix = {arXiv},
  primaryClass = {cs.CL},
  url = {https://arxiv.org/abs/2608.03581},
  note = {Survey of reviewer-facing AI policies across 111 AI/NLP conferences and medical journals, with quality evaluation of AI reviews at ICLR 2026 and Nature Communications},
}

@article{wang2026crossdisciplinary,
  author = {Wang, Zhongshi and Gong, Mengyue},
  title = {{A Cross-Disciplinary Analysis of AI Policies in Academic Peer Review}},
  journal = {Learned Publishing},
  volume = {39},
  number = {1},
  pages = {e2035},
  year = {2026},
  doi = {10.1002/leap.2035},
  url = {https://doi.org/10.1002/leap.2035},
  note = {Policy analysis of 439 high-impact-factor and 363 middle-impact-factor journals; 24.5\% of high-impact journals revised AI peer review policies within six months},
}

@misc{springernature2026aitools,
  author = {{Springer Nature Group}},
  title = {{Springer Nature Embraces AI Tools Across the Publishing Process, Resulting in Less Friction and Increased Author Satisfaction}},
  howpublished = {Springer Nature Group press release},
  year = {2026},
  url = {https://group.springernature.com/gp/group/media/press-releases/ai-tools-support-less-friction-and-increased-author-satisfaction/27849346},
  note = {Over 1.5 million papers supported by nearly 60 AI tools in 2025, projected to rise 25\% in 2026; Snapp used by more than half of Springer Nature journals; Geppetto and SnappShot integrity screening},
}

@article{naturenano2026peerreview,
  author = {{Nature Nanotechnology Editorial}},
  title = {{Peer Review in the Time of Artificial Intelligence}},
  journal = {Nature Nanotechnology},
  volume = {21},
  pages = {479},
  year = {2026},
  doi = {10.1038/s41565-026-02177-2},
  url = {https://doi.org/10.1038/s41565-026-02177-2},
  note = {Editorial establishing that the user of an AI tool is always accountable, that every AI output requires human validation, and that AI use must be declared in the review report},
}

@article{kim2026limits,
  author = {Kim, Seungone and Yoon, Dongkeun and Gashteovski, Kiril and Suk, Juyoung and Baek, Jinheon and Aggarwal, Pranjal and Wu, Ian and Zaverkin, Viktor and Petkoski, Spase and Schrider, Daniel R. and others},
  title = {{On the Limits and Opportunities of AI Reviewers: Reviewing the Reviews of Nature-Family Papers with 45 Expert Scientists}},
  journal = {arXiv preprint arXiv:2605.20668},
  year = {2026},
  month = {May},
  eprint = {2605.20668},
  archivePrefix = {arXiv},
  primaryClass = {cs.CL},
  url = {https://arxiv.org/abs/2605.20668},
  note = {45 domain scientists spent 469 hours rating 2,960 criticisms from human and AI reviews of 82 Nature-family papers; AI surfaced a distinct 26\% of issues but produced more factually incorrect items},
}

@article{georgantas2026bottleneck,
  author = {Georgantas, Costa},
  title = {{Intelligence Is Not the Bottleneck: Validating an LLM First-Pass Manuscript Score Against Peer-Review Outcomes}},
  journal = {arXiv preprint arXiv:2606.15887},
  year = {2026},
  month = {June},
  eprint = {2606.15887},
  archivePrefix = {arXiv},
  primaryClass = {cs.DL},
  url = {https://arxiv.org/abs/2606.15887},
  note = {Training-free manuscript score (AIPR) validated on 300 ICLR submissions; AUROC 0.82 (95\% CI 0.78--0.87) separating rejected from accepted papers},
}

@article{patel2026ajsm,
  author = {Patel, Romir and Shultz, Christopher and Ollivier, Matthieu and Wascher, Daniel C.},
  title = {{Artificial Intelligence Cannot Replace Peer Reviewers but May Help Editors Triage: A Comparative Analysis of a Large Language Model and Human Reviewer Recommendations at the American Journal of Sports Medicine}},
  journal = {The American Journal of Sports Medicine},
  year = {2026},
  doi = {10.1177/03635465261463006},
  url = {https://doi.org/10.1177/03635465261463006},
  note = {Clinical-journal comparison concluding that LLMs support editorial triage but cannot substitute for reviewer judgment},
}

@article{thakkar2026feedback,
  author = {Thakkar, Nitya and Yuksekgonul, Mert and Silberg, Jake and Garg, Animesh and Peng, Nanyun and Sha, Fei and Yu, Rose and Vondrick, Carl and Zou, James},
  title = {{A Large-Scale Randomized Study of Large Language Model Feedback in Peer Review}},
  journal = {Nature Machine Intelligence},
  volume = {8},
  year = {2026},
  doi = {10.1038/s42256-026-01188-x},
  url = {https://doi.org/10.1038/s42256-026-01188-x},
  note = {Review Feedback Agent deployed as a randomized controlled study over more than 20,000 reviews; 27\% of coached reviewers revised their reviews, incorporating over 12,000 suggestions},
}

@inproceedings{baumann2026stop,
  author = {Baumann, Joachim and Pei, Jiaxin and Koyejo, Sanmi and Hovy, Dirk},
  title = {{Stop Automating Peer Review Without Rigorous Evaluation}},
  booktitle = {Proceedings of the Post-AGI Science and Society Workshop},
  year = {2026},
  eprint = {2605.03202},
  archivePrefix = {arXiv},
  primaryClass = {cs.CL},
  url = {https://arxiv.org/abs/2605.03202},
  note = {Documents the hivemind effect of excessive agreement among AI reviewers and demonstrates paper laundering, whereby LLM rewriting inflates AI review scores},
}

@article{yang2026nohidden,
  author = {Yang, Xu and others},
  title = {{No Hidden Prompts Needed! You Can Game AI Peer Review with Presentation-Only Revisions}},
  journal = {arXiv preprint arXiv:2606.13044},
  year = {2026},
  month = {June},
  eprint = {2606.13044},
  archivePrefix = {arXiv},
  primaryClass = {cs.CL},
  url = {https://arxiv.org/abs/2606.13044},
  note = {Adversarial repackaging achieves a 75.1\% attack success rate and mean score gain of +1.21/10 across three mainstream AI reviewers without altering any scientific content},
}

@misc{iclr2026retrospective,
  author = {{ICLR 2026 Program Chairs}},
  title = {{A Retrospective on the ICLR 2026 Review Process}},
  howpublished = {ICLR Blog},
  year = {2026},
  month = {March},
  day = {31},
  url = {https://blog.iclr.cc/2026/03/31/a-retrospective-on-the-iclr-2026-review-process/},
  note = {19,525 valid submissions, 779 desk rejections, 5,042 withdrawals, 13,763 decisions based on 76,139 reviews from 18,054 reviewers; hallucinated-reference detection with three-human verification and an appeals channel},
}

@misc{pangram2026iclr,
  author = {{Pangram Labs}},
  title = {{Pangram Predicts 21\% of ICLR Reviews Are AI-Generated}},
  howpublished = {Pangram Labs technical blog},
  year = {2026},
  url = {https://www.pangram.com/blog/pangram-predicts-21-of-iclr-reviews-are-ai-generated},
  note = {Detection analysis of ICLR 2026 reviews; claimed false-positive rate of 1 in 10,000 and 86.2\% concordance with independent author complaints. Vendor sells AI detection tools},
}

@misc{icml2026violations,
  author = {{ICML 2026 Program Chairs}},
  title = {{On Violations of LLM Review Policies}},
  howpublished = {ICML Blog},
  year = {2026},
  month = {March},
  day = {18},
  url = {https://blog.icml.cc/2026/03/18/on-violations-of-llm-review-policies/},
  note = {Watermark-based enforcement using a 170,000-phrase dictionary; 795 reviews removed (1\% of total) and 497 papers desk-rejected (2\% of submissions) at a family-wise error rate of 0.0001},
}

@article{gibney2026conference,
  author = {Gibney, Elizabeth},
  title = {{Major Conference Catches Illicit AI Use --- and Rejects Hundreds of Papers}},
  journal = {Nature},
  year = {2026},
  month = {March},
  day = {25},
  doi = {10.1038/d41586-026-00893-2},
  url = {https://www.nature.com/articles/d41586-026-00893-2},
  note = {News coverage of watermark-based detection of undisclosed LLM use in conference peer review},
}

@article{gartenberg2026more,
  author = {Gartenberg, Claudine and Hasan, Sharique and Murray, Alex and Pierce, Lamar},
  title = {{More Versus Better: Artificial Intelligence, Incentives, and the Emerging Crisis in Peer Review}},
  journal = {Organization Science},
  volume = {37},
  number = {3},
  pages = {795--812},
  year = {2026},
  doi = {10.1287/orsc.2026.ed.v37.n3},
  url = {https://doi.org/10.1287/orsc.2026.ed.v37.n3},
  note = {Analysis of 6,957 submissions and 10,389 reviews from 2021 to 2026 documenting a 42\% post-ChatGPT rise in submissions with declining writing quality},
}

@article{hakobyan2026monitor,
  author = {Hakobyan, Zaruhi},
  title = {{Buying the Right to Monitor: Editorial Design in AI-Assisted Peer Review}},
  journal = {arXiv preprint arXiv:2604.23645},
  year = {2026},
  month = {April},
  eprint = {2604.23645},
  archivePrefix = {arXiv},
  primaryClass = {econ.TH},
  url = {https://arxiv.org/abs/2604.23645},
  note = {Three-sided equilibrium model showing discontinuous collapse of reviewer effort above a critical AI capability threshold, and the resulting case for loosened selectivity combined with investment in detection},
}

@misc{scientist2026trap,
  author = {{The Scientist}},
  title = {{A Trap for AI Use in Peer Reviews Sparks Controversy}},
  howpublished = {The Scientist},
  year = {2026},
  url = {https://www.the-scientist.com/a-trap-for-ai-use-in-peer-reviews-sparks-controversy-74702},
  note = {Reports the NeurIPS 2026 and ICML 2026 prompt-injection enforcement approach and the community criticism that designing traps presuming bad faith corrodes reviewer trust},
}

@misc{mdpi2026retractions,
  author = {{MDPI}},
  title = {{Learning from Retractions to Drive Prevention Strategies}},
  howpublished = {MDPI Blog},
  year = {2026},
  month = {July},
  day = {23},
  url = {https://blog.mdpi.com/2026/07/23/retractions-data-2025/},
  note = {Retraction rate of approximately 0.2\% in 2025 against 0.02\% in 2016; compromised peer review and paper mills together account for 43\% of retractions, compromised peer review alone for 37\%},
}

@misc{scientist2026resignation,
  author = {{The Scientist}},
  title = {{Automation Concerns Prompt Editor Resignation}},
  howpublished = {The Scientist},
  year = {2026},
  month = {June},
  url = {https://www.the-scientist.com/automation-concerns-prompt-editor-resignation-74645},
  note = {Michael Okun resigns as associate editor of Frontiers in Systems Neuroscience after the AIRA system revoked his manually issued reviewer invitations and could not be disabled},
}

@misc{aaai2026reviewprocess,
  author = {{Association for the Advancement of Artificial Intelligence}},
  title = {{AAAI-27 Review Process}},
  howpublished = {AAAI conference documentation},
  year = {2026},
  url = {https://aaai.org/conference/aaai/aaai-27/review-process/},
  note = {Continuation of the AI-assisted peer review pilot with revisions; AI reviews carry no ratings or recommendations and play no formal role in decisions, which remain solely human},
}

@misc{neurips2026experiment,
  author = {{Neural Information Processing Systems Foundation}},
  title = {{NeurIPS 2026 AI-Assisted Reviewing Experiment}},
  howpublished = {NeurIPS conference documentation},
  year = {2026},
  url = {https://neurips.cc/Conferences/2026/ai-reviewing-experiment},
  note = {Author-opt-in randomized experiment assigning reviewers to no LLM assistance, open-ended assistance, or structured assistance; all other LLM use unsanctioned},
}

@misc{emnlp2026experiment,
  author = {{EMNLP 2026 Organizing Committee}},
  title = {{EMNLP 2026 AI Reviewing Experiment}},
  howpublished = {EMNLP 2026 conference documentation},
  year = {2026},
  url = {https://2026.emnlp.org/ai-reviewing-experiment/},
  note = {Opt-in AI review study using the ReviewerToo system (Mila, ServiceNow Research, HEC Montr{\'e}al, Polytechnique Montr{\'e}al, Universit{\'e} de Montr{\'e}al, Unified Sciences) on GPT-OSS-120B; AI reviews visible only to authors and AI Review Chairs and play no role in decisions},
}

@misc{journalmetrics2026icmje,
  author = {{JournalMetrics}},
  title = {{The January 2026 ICMJE Update: A Practical Guide for Authors}},
  howpublished = {JournalMetrics editorial-policy guide},
  year = {2026},
  url = {https://www.journalmetrics.org/blog/icmje-2026-recommendations-authors},
  note = {Summarizes the January 2026 ICMJE revision introducing a dedicated AI section treated as authoritative by JAMA, NEJM, The Lancet, BMJ and affiliated specialty journals, together with JAMA's prohibition of AI in peer review},
}

@misc{jaai2026,
  author = {{JAAI}},
  title = {{JAAI: The World's First Fully Autonomous Academic Journal}},
  howpublished = {Journal website},
  year = {2026},
  url = {https://jaai.pub/},
  note = {Established March 2026 under the description ``AI writes. AI reviews. AI publishes.''; inaugural volume contains 35 research articles. Not indexed in major abstracting databases},
}

@misc{aisc2026,
  author = {{aiXiv}},
  title = {{AISC 2026: The AI Scientists Conference}},
  howpublished = {Conference website, aiXiv platform},
  year = {2026},
  url = {https://aixiv.science/aisc2026/},
  note = {States that every stage from peer review to final acceptance decision is performed entirely by AI agents with zero human involvement in the review pipeline; reviews, discussions and decision rationale published openly; submissions accepted via web portal or Agent API},
}

@article{naddaf2026paying,
  author = {Naddaf, Miryam},
  title = {{Why Paying Peer Reviewers Works, According to a Journal's Editor-in-Chief}},
  journal = {Nature},
  year = {2026},
  month = {July},
  day = {1},
  doi = {10.1038/d41586-026-01973-z},
  url = {https://www.nature.com/articles/d41586-026-01973-z},
  note = {Reports that Biology Open's reviewer payment trial cut time to first editorial decision by 85\% while maintaining review quality},
}

@misc{insidehighered2026paying,
  author = {{Inside Higher Ed}},
  title = {{Will Paying Reviewers Ease the Peer Review Crisis?}},
  howpublished = {Inside Higher Ed},
  year = {2026},
  month = {May},
  day = {14},
  url = {https://www.insidehighered.com/news/faculty/books-publishing/2026/05/14/will-paying-reviewers-ease-peer-review-crisis},
  note = {Reports reviewer scarcity requiring 20 to 30 invitations per two completed reviews, and Jonas Kunst's advances.in model paying \$100 per completed review},
}

@misc{researchhub2026journal,
  author = {{ResearchHub Foundation}},
  title = {{The ResearchHub Journal: Paid Peer Review Program Guidelines}},
  howpublished = {ResearchHub Foundation documentation},
  year = {2026},
  url = {https://docs.researchhub.com/researchhub-foundation/programs-and-initiatives/researchhub-journal-rhj},
  note = {ISSN 3070-3395; pays \$150 in ResearchCoin per review within seven days of the bounty window closing, with reviewers self-selecting papers in an open marketplace},
}

@misc{advances2026psychology,
  author = {{advances.in/psychology}},
  title = {{About the Journal: Compensating Editors and Reviewers}},
  howpublished = {Journal website},
  year = {2026},
  url = {https://advances.in/psychology/about/},
  note = {Open-access journal founded by Jonas Kunst (University of Oslo) that financially compensates both editors and reviewers from a \$1,950 article processing charge (\$450 for commentaries)},
}

@misc{casrai2026nih,
  author = {{CASRAI}},
  title = {{NIH Open Access Publishing Fee Cap}},
  howpublished = {CASRAI research-policy guide},
  year = {2026},
  url = {https://casrai.org/guides/nih-open-access-publishing-fee-limits},
  note = {Tiered allowable-publication-cost policy effective 1 January 2026 permitting up to \$3,000 per publication only where peer reviewers are compensated and reviews are shared openly, premised on three reviewers at \$300 each},
}

@misc{orrall2026statistics,
  author = {Orrall, Avery},
  title = {{`The Exploitation Still Remains': Stats Journal Associate Editors Resign over \$3,000 Publishing Charge}},
  howpublished = {Retraction Watch},
  year = {2026},
  month = {July},
  day = {9},
  url = {https://retractionwatch.com/2026/07/09/the-exploitation-still-remains-stats-journal-associate-editors-resign-over-3000-publishing-charge/},
  note = {Eighteen associate editors of Statistics and Computing resign effective 31 December 2026 over a \$2,990 article processing charge and the move to full open access in 2027},
}

@article{naturecompsci2026ecr,
  author = {{Nature Computational Science Editorial}},
  title = {{Supporting Early-Career Researchers in Peer Review}},
  journal = {Nature Computational Science},
  year = {2026},
  doi = {10.1038/s43588-026-01001-0},
  url = {https://doi.org/10.1038/s43588-026-01001-0},
  note = {Describes the co-review initiative recognizing post-doctoral and junior researchers who contribute to reviews, and the effect of uncompensated review time on engagement},
}

@misc{neucite2026payment,
  author = {{Neucite Press}},
  title = {{Do Peer Reviewers Get Paid? What Journals Actually Offer in 2026}},
  howpublished = {Neucite Press},
  year = {2026},
  url = {https://neucitepress.com/should-journals-pay-peer-reviewers-the-ongoing-debate-explained/},
  note = {Compiles 2026 reviewer compensation practice, including Critical Care Medicine's \$250 offer to half of 715 invited reviewers (53\% versus 48\% acceptance) and Biology Open's \$284 per review (4.6 versus 38 business days)},
}

@misc{duckofminerva2026peerreview,
  author = {{The Duck of Minerva}},
  title = {{Is Peer Review Broken? Should Reviewers Be Paid?}},
  howpublished = {The Duck of Minerva},
  year = {2026},
  month = {January},
  url = {https://www.duckofminerva.com/2026/01/is-peer-review-broken-should-reviewers-be-paid.html},
  note = {Disciplinary commentary on the economics of unpaid review labor and the case for and against direct reviewer compensation},
}


Sources:
AI-Assisted Peer Review at Scale: The AAAI-26 AI Review Pilot
Towards Automating Scientific Review with Google's Paper Assistant Tool
AI-Assisted Peer Review Across Research Communities
A Cross-Disciplinary Analysis of AI Policies in Academic Peer Review
Springer Nature embraces AI tools across the publishing process
Peer review in the time of artificial intelligence
On the limits and opportunities of AI reviewers
Intelligence Is Not the Bottleneck
Artificial Intelligence Cannot Replace Peer Reviewers but May Help Editors Triage
A large-scale randomized study of large language model feedback in peer review
Stop Automating Peer Review Without Rigorous Evaluation
No Hidden Prompts Needed!
A Retrospective on the ICLR 2026 Review Process
Pangram Predicts 21% of ICLR Reviews are AI-Generated
On Violations of LLM Review Policies
Major conference catches illicit AI use
More Versus Better
Buying the Right to Monitor
A Trap for AI Use in Peer Reviews Sparks Controversy
Learning from Retractions to Drive Prevention Strategies
Automation Concerns Prompt Editor Resignation
AAAI-27 Review Process
NeurIPS 2026 AI-Assisted Reviewing Experiment
EMNLP 2026 AI Reviewing Experiment
The January 2026 ICMJE Update
JAAI
AISC 2026: The AI Scientists Conference
Why paying peer reviewers works
Will Paying Reviewers Ease the Peer Review Crisis?
ResearchHub Journal
advances.in/psychology
NIH Open Access Publishing Fee Cap
Stats journal associate editors resign
Supporting early-career researchers in peer review
Do Peer Reviewers Get Paid?
Is Peer Review Broken? Should Reviewers Be Paid?

Three notes on the premises in your request
No journals have been replaced by AI peer review. I looked specifically for this and found no case. The two fully autonomous venues (JAAI, AISC 2026) are new, unindexed entrants. The nearest real case of AI displacing a human function at an established journal is Frontiers' AIRA overriding an editor's reviewer invitations — which concerns reviewer selection, not evaluative judgment, and produced a resignation rather than a rollout.
There is no coordinated "AI peer review takeover" initiative. There is uncoordinated Layer 1–2 automation, fenced Layer 3 experiments, explicit Layer 4 prohibitions (Elsevier, JAMA), and a small autonomous fringe. I have documented all four rather than assuming a single trend.
Post-docs are not being paid instead of journals. Per-review honoraria of $100–$284 exist at a handful of journals, and NIH has made compensation a condition of its higher reimbursement tier — but no journal revenue has been redirected to post-doctoral researchers. I flagged the countervailing force explicitly: AAAI-26 generated reviews at under $1 per paper, two to three orders of magnitude below human rates, which caps what anyone will pay for the commodity portion of review labor.
I have not committed anything to the repository, per your instruction.

