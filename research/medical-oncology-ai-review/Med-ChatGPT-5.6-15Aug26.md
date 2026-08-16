## Med-ChatGPT-5.6-15Aug26.md

AI Peer Review in Medical and Oncology Publishing in 2026: A SMART-Framework Review of Replacement Readiness, Implementations, Governance, and Reviewer Economics
Abstract
This review evaluates the status of artificial intelligence (AI)-assisted peer review in medical journal publishing, with an emphasis on oncology, using the SMART framework—Specific, Measurable, Achievable, Relevant, and Time-bound. The evidence base is restricted to publications, preprints, or formal guidance dated 2026 and publicly available through August 15, 2026. The principal finding is that AI has not replaced human peer review in any medical or oncology journal identified in the 2026 evidence base. Rather, the leading implementations are hybrid systems in which AI performs reviewer support, manuscript triage, editor matching, structured critique, or quality-control functions while humans retain scientific accountability and editorial authority. A May 2026 survey of 48 leading medical journals found that 58% prohibited reviewer AI use, 38% allowed only partial use, and only one—IEEE Transactions on Medical Imaging (TMI), through its AI4TMI initiative—was classified as actively using AI-assisted reviewing [1]. 
The strongest 2026 implementations therefore support task replacement rather than reviewer replacement. TMI’s Editorial AI Reviewer (AIR) and AI-supported associate-editor assignment demonstrate how secure AI can enter a real medical journal workflow [5,6]. A cardiology journal study found AI-generated reviews fast and broadly comparable with human review on several structured measures, but the authors recommended complementary rather than replacement use [7]. Large-scale nonmedical experiments reinforce this pattern: AI can improve human-written reviews [9] and can generate tens of thousands of supplemental reviews at very low marginal computational cost [10], yet current systems remain vulnerable to calibration errors, overly favorable recommendations, insufficient evidence grounding, and adversarial manipulation [1,11,12]. 
For oncology specifically, the 2026 evidence supports a conservative transition toward secure AI co-review, not autonomous adjudication. JAMA Network’s August 2026 guidance—which encompasses JAMA Oncology—explicitly classifies external AI use for peer review as unacceptable because transmitting a manuscript or review summary to an external AI system violates confidentiality [3]. Meanwhile, oncology-specific research in Annals of Surgical Oncology is actively testing LLM-assisted scientific-merit screening, illustrating strong interest in automation without demonstrating a replacement-ready system [8]. 
The economics of review may change at the same time. A 2026 report on Biology Open’s paid-review model found that paying reviewers £220 for timely, editorially acceptable reviews reduced mean time to a first decision with reviews from 37.7 to 5.5 working days [15]. However, there is no 2026 evidence that oncology journals have broadly begun paying postdoctoral researchers instead of relying on journal or publisher revenue models. The more plausible near-term model is a hybrid economic system in which AI handles routine screening and drafting while scarce specialist human judgment—potentially supplied by qualified postdoctoral researchers as well as faculty and practicing clinicians—is compensated more explicitly [15,16]. 

1. Scope and interpretation of “replacement”
For purposes of this review, “AI replacement of peer review” should be divided into three levels:
Task replacement: AI independently performs an individual function previously performed manually—for example, editor matching, checklist verification, identifying statistical inconsistencies, or producing a preliminary critique.


Reviewer replacement: an AI review substitutes for a human review slot that otherwise would have been assigned to a subject-matter expert.


Editorial-authority replacement: AI determines whether a manuscript is accepted, revised, or rejected without accountable human adjudication.


This distinction is essential because 2026 literature sometimes describes systems as “AI reviewers” even though those systems are supplemental. The strongest contemporary survey concludes that current LLMs can broaden the set of issues detected and generate detailed review text, but remain insufficiently calibrated and grounded for autonomous reviewer status [1]. 
No medical or oncology journal identified in the 2026 evidence reviewed here has reached Level 3, and there is no convincing evidence of routine Level-2 replacement in medical journals. Level-1 automation, by contrast, is already operational. Among 48 high-impact medical journals examined in May 2026—including eight journals from each of six clinical categories, one of which was oncology—28 of 48 prohibited reviewer AI, 18 allowed restricted use, one had no policy, and only TMI was classified as having an active AI-assisted review process [1]. Fifteen of the 18 medical journals with partial-use policies specifically prohibited reviewers from uploading manuscripts to AI systems [1]. 
This makes the phrase “AI peer-review takeover” somewhat ahead of the evidence. In 2026, the transition is better described as a selective transfer of low- and intermediate-level reviewing functions to AI under human supervision.

2. Current 2026 status in medicine and oncology
2.1 Medicine overall: governance currently favors human accountability
The January 2026 International Committee of Medical Journal Editors (ICMJE) Recommendations establish a governance structure that is fundamentally incompatible with unsupervised AI peer review. ICMJE states that humans remain responsible for checking AI-generated material, that confidential submitted manuscripts should not be uploaded to AI systems when confidentiality cannot be assured without author permission, that AI use during review should be transparent, and that journals should establish explicit AI policies [2]. 
Consequently, the strongest medical publishing governance framework in 2026 does not prohibit all AI involvement, but it places responsibility on identifiable humans. That difference is important. A secure journal-owned system could, in principle, satisfy confidentiality requirements far more readily than a reviewer copying an unpublished manuscript into a public consumer chatbot.
2.2 Oncology: particularly conservative because errors have clinical consequences
Oncology presents a strong argument for cautious implementation because manuscript assessment frequently requires interpretation of survival endpoints, subgroup analyses, biomarkers, treatment sequencing, adverse events, pathology, radiologic response, and the clinical meaningfulness of effect sizes. An apparently sophisticated review can therefore be unsafe if the system fails to distinguish statistical significance from clinical relevance or cannot recognize a subtle design problem.
A 2026 systematic analysis of 60 high-impact oncology journals found broad agreement that human accountability should remain central to AI use in scholarly publishing [4]. Because that 2026 publication retrospectively analyzed previously issued policies, it should be interpreted as contextual evidence rather than as the primary August 2026 policy snapshot. The newer May 2026 reviewer-policy survey [1] and August 2026 JAMA guidance [3] provide more contemporaneous evidence regarding peer-review use. 
The clearest oncology example is JAMA Oncology. JAMA Oncology is part of the JAMA Network, and the Network’s August 10, 2026 guidance lists “Peer review” as an unacceptable use of external AI: transmitting an author’s manuscript or the reviewer’s manuscript summary to an external AI tool or LLM violates confidentiality [3]. Thus, one of the leading oncology journals is presently moving in the opposite direction from autonomous AI takeover. 
2.3 Journals actually replaced by AI peer review
None were identified in medical or oncology publishing as of August 15, 2026.
The distinction can be summarized as follows:
Journal or initiative
2026 role of AI
Human reviewers replaced?
Autonomous AI editorial decision?
Interpretation
IEEE Transactions on Medical Imaging / AI4TMI and AIR
Active AI-assisted editorial/review workflow
No evidence of routine replacement
No
Most mature medical-journal implementation identified [1,5,6]
JAMA Oncology / JAMA Network
External AI peer review prohibited
No
No
Strong confidentiality-first policy [3]
European Heart Journal – Imaging Methods and Practice
Blinded comparison of AI and human reviews
No
No
Performance study; supports complementary use [7]
Annals of Surgical Oncology / ASBrS work
LLM assessment of scientific abstracts
No
No
Oncology-specific evidence for screening research, not journal-review replacement [8]
Orthopaedics & Traumatology: Surgery & Research
AI versus human desk-decision concordance study
No
No
Results argue against autonomous editorial disposition [12]
AAAI-26
One AI review added to full-review submissions
No
No
Largest 2026 operational benchmark, but not medical [10]


3. Most effective implementations to date
3.1 IEEE Transactions on Medical Imaging: the strongest real medical-journal implementation
The most important 2026 medical example is IEEE Transactions on Medical Imaging. Fichtl et al.‘s cross-journal survey identifies TMI as the only active AI-assisted reviewing venue among the 48 leading medical journals sampled [1]. TMI’s AIR trial was formally reported in January 2026 as part of the broader AI4TMI effort [5]. 
TMI is significant because it is not simply a laboratory comparison between an LLM and archived reviews. It represents an effort to embed AI into an actual journal’s editorial infrastructure while maintaining a controlled workflow.
A complementary AI4TMI project automates associate-editor assignment. Xu et al. developed a locally operated system using ModernBERT embeddings, structured manuscript keywords, dimensionality reduction, and similarity matching against a curated associate-editor database [6]. Structured keywords proved to be the dominant signal, titles added useful information, and abstracts provided comparatively little additional benefit. The system was explicitly designed to reduce manual editorial workload while preserving the editorial structure rather than eliminating it [6]. 
This is arguably the most defensible implementation strategy in medicine because editor assignment has several characteristics favorable to AI:
the objective can be defined reasonably well;


performance can be measured against historical assignments;


errors are reversible before publication;


confidential data can remain within journal-controlled infrastructure;


the output is a ranked recommendation rather than a scientific verdict; and


a human managing editor retains authority.


In SMART terms, TMI demonstrates that narrow, measurable automation is more achievable than replacing the reviewer as a whole.
3.2 Cardiology: evidence that AI can produce useful reviews extremely quickly
A 2026 blinded comparison in European Heart Journal – Imaging Methods and Practice evaluated AI-generated reviews against human reviews [7]. The AI system achieved 67.5% concordance with final article-level decisions, compared with 71.9% for evaluable human consensus; AI-human agreement on binary recommendations was substantial, with κ approximately 0.73, while human-human agreement was lower in that analysis. AI reviews were also generated on a dramatically shorter timescale than traditional human review [7]. The investigators nevertheless characterized AI as a complementary editorial tool rather than a substitute for human peer review. 
The lesson is important: near-human agreement is not equivalent to safe replacement. Editorial decisions themselves are noisy, human reviewers disagree, and agreement measures can conceal whether AI reached a recommendation for the correct methodological reason.
For oncology, the analogous use would be a second-opinion reviewer that independently flags concerns after a human reviewer has formed an initial opinion. Such sequencing also reduces anchoring: the reviewer first assesses the study independently and then evaluates AI-suggested concerns.
3.3 AI that improves the human reviewer may outperform AI that tries to replace the reviewer
One of the strongest causal demonstrations in 2026 is the Review Feedback Agent reported by Thakkar et al. in Nature Machine Intelligence [9]. The publication reports a randomized deployment involving more than 20,000 reviews. AI supplied feedback on vague comments, misunderstandings, specificity, and professionalism; reviewers then decided whether to incorporate the suggestions. Twenty-seven percent of reviewers who received feedback modified their reports, incorporating more than 12,000 suggestions, and blinded assessment found the resulting reviews more informative [9]. 
Although the deployment evaluated in that 2026 publication occurred in a computer-science review setting rather than medicine, its architecture is highly transferable. It gives the LLM a role analogous to an editor for the reviewer, not a replacement for the scientific expert.
For an oncology journal, this model could ask:
Does the review identify whether the primary endpoint was prespecified?


Does the reviewer discuss multiplicity?


Has the reviewer distinguished progression-free survival from overall survival implications?


Has the reviewer addressed biomarker validation?


Are recommendations tied to specific manuscript sections?


Is the critique actionable rather than generic?


Does the language remain professional?


Has the reviewer overlooked an important reporting requirement?


This division of labor retains domain expertise while using AI for completeness and communication quality.
3.4 AAAI-26: the strongest demonstration of operational scale
The AAAI-26 AI Review Pilot is not a medical-journal implementation, but it is a major proof of scalability. Every main-track paper receiving full review—22,977 submissions—received one clearly identified AI-generated review, produced through a multistage system using frontier models, tools, and safeguards [10]. All AI reviews were generated in less than a day [10]. 
The critical point is what AAAI did not do. It did not remove human peer reviewers. AI was integrated into a human-AI evaluation system, consistent with the broader 2026 evidence that the practical frontier is collaboration rather than substitution [1,10]. 
For medical publishing, AAAI-26 is therefore best viewed as a stress test showing that AI reviewing can scale technically. It does not establish that such a system is sufficiently safe, confidential, clinically knowledgeable, or regulatorily acceptable for oncology publication decisions.
3.5 Oncology-specific evidence: breast-surgery abstract evaluation
Cohen and colleagues examined whether LLMs could reproduce scientific-merit scoring for abstracts associated with the American Society of Breast Surgeons, with the study published in Annals of Surgical Oncology in July 2026 [8]. The investigators evaluated 378 accepted abstracts with multiple LLMs under zero-shot and few-shot approaches. Human median scores were 21.2 on the relevant rubric, whereas LLM median scores were substantially higher, approximately 27.0–29.7 [8]. 
This is particularly informative for oncology because it illustrates leniency/calibration bias in an oncology-adjacent scientific evaluation task. It is not evidence that Annals of Surgical Oncology has replaced its journal peer reviewers. Instead, it suggests that AI may help pre-screen large numbers of submissions, but thresholds cannot simply be imported from human scoring systems.
The study therefore supports using AI for prioritization or quality-floor screening only after journal-specific calibration.

4. Why autonomous replacement remains premature
4.1 Persuasive prose is not calibrated scientific judgment
The 2026 cross-disciplinary analysis by Fichtl et al. found that AI-generated reviews can be detailed, fluent, and superficially strong yet still show systematic weaknesses. These included overly positive recommendations, generic criticism, variable grounding in manuscript evidence, and imperfect calibration with paper quality [1]. The authors therefore concluded that LLMs are currently better suited to reviewer assistance than autonomous reviewing [1]. 
This matters especially in oncology. A review can sound sophisticated while failing to recognize that a subgroup analysis is underpowered, a surrogate endpoint is not validated for the relevant disease state, a control arm is outdated, or an apparent treatment benefit results from informative censoring.
4.2 Prompt injection creates a direct integrity threat
The strongest medical security warning published in 2026 comes from Choi et al. in JAMA Network Open. The investigators embedded invisible instructions into manuscripts during simulated medical peer review and tested several LLM systems [11]. Invisible-text injection increased acceptance recommendations from essentially 0% to nearly 100% in the manipulated condition for the tested systems under neutral prompting. Under stringent flaw-detection criteria, overall successful flaw detection declined from 18.9% to 8.5%; methods-section detection fell from 56.3% to 25.6% [11]. More stringent prompting did not reliably eliminate the manipulation [11]. 
An autonomous oncology-review system would therefore create a new incentive: authors could attempt to write not only for human readers, but for the hidden vulnerabilities of the reviewing model.
This changes peer-review security from a primarily social problem into an adversarial machine-learning problem.
4.3 Desk decisions remain unreliable
A July 2026 study in Orthopaedics & Traumatology: Surgery & Research compared three contemporary LLMs with actual human editorial desk decisions [12]. Accuracy was approximately 59–63%, with weak agreement statistics and a tendency toward erroneous disposition of manuscripts [12]. 
This negative result is useful. Desk review sounds like an easier task than full clinical peer review, yet current systems can still produce plausible explanations without reliably reproducing editorial judgment. That finding argues against allowing a medical LLM to autonomously determine which manuscripts never reach human experts.
4.4 Confidentiality is a structural obstacle, not merely a model-performance problem
ICMJE’s January 2026 recommendations explicitly link AI manuscript processing to confidentiality risk [2], and JAMA Network’s August 2026 guidance makes that principle operational by prohibiting external AI peer-review use [3]. 
A viable medical AI reviewer therefore needs a different technical architecture from casual consumer-chatbot use:
journal-controlled or contractually protected model execution;


explicit data-retention rules;


no training on submitted manuscripts;


access control;


encrypted storage and transmission;


model/version logging;


prompt and output auditability;


defined deletion schedules; and


disclosure to authors and reviewers.


These conditions make secure deployment feasible, but they also mean that the apparent low cost of “asking an LLM to review a paper” substantially understates the cost of a compliant medical-publishing system.

5. Initiatives that could lead toward greater AI takeover
The 2026 initiatives can be placed along a replacement continuum.
Phase A: administrative automation
This includes editor assignment, reviewer matching, metadata extraction, reporting-guideline checks, conflict screening, and manuscript completeness. TMI’s associate-editor matching system is the clearest medical example [6]. These functions are comparatively low risk because human editors can easily inspect or override the output. 
Phase B: reviewer augmentation
Systems such as the Review Feedback Agent analyze an existing human review and suggest improvements [9]. This approach has especially strong evidence because it preserves the reviewer’s independent scientific opinion while improving clarity and coverage. 
Phase C: supplemental AI reviewer
TMI’s AIR direction [5], the cardiology comparison [7], and AAAI-26 [10] represent movement toward AI functioning as an additional reviewer. In this design, AI identifies candidate problems, but a human reviewer or editor verifies them. 
Phase D: human-slot substitution
This would occur if a journal historically assigned, for example, three human reviewers but began assigning two humans plus one AI. The 2026 medical evidence reviewed here does not demonstrate widespread operational adoption of this model.
Phase E: autonomous editorial system
A more radical 2026 research direction is ADAPT—AI-Driven Decentralized Adaptive Publishing Testbed—which models publication as an adaptive system containing human and AI reviewers and changing governance rules [14]. Importantly, even this forward-looking architecture preserves human decision authority and confidentiality rather than proposing unrestricted AI control [14]. 
Thus, even initiatives explicitly exploring future AI-intensive publishing are generally converging on human-governed automation rather than human-free publishing.

6. SMART assessment for oncology journal implementation
S — Specific
A defensible 2026 goal for an oncology journal should not be:
“Replace human peer reviewers with AI.”
A more appropriate goal is:
Deploy a secure AI co-review system that automates defined low- and intermediate-risk review functions while reserving novelty, clinical importance, causal interpretation, ethical assessment, and final editorial decisions for accountable human oncology experts.
The AI scope should initially include:
associate-editor and reviewer matching;


manuscript-structure checks;


reporting-guideline completeness;


identification of missing statistical information;


internal consistency checks between abstract, tables, figures, and conclusions;


reference-verification flags;


identification of potentially overlooked methodological issues;


generation of questions for the reviewer;


review-quality feedback; and


structured comparison of disagreements among human reviewers.


Final judgment on therapeutic relevance, novelty, clinical practice implications, risk-benefit interpretation, and publication priority should remain human.
M — Measurable
AI review cannot be evaluated merely by asking whether its recommendation agrees with an editor. Fichtl et al. show why: high aggregate language-quality ratings can coexist with poor calibration and generic criticism [1]. 
An oncology journal should prespecify a multidimensional scorecard that includes:
Domain
Recommended measurement
Major-error detection
Sensitivity for deliberately seeded or independently adjudicated critical errors
False alarms
Number of invalid concerns per manuscript
Evidence grounding
Fraction of critiques traceable to a specific table, figure, method, result, or citation
Clinical reasoning
Expert rating of whether conclusions reflect oncology context
Statistical performance
Agreement with specialist statistical review
Calibration
Relationship between AI severity scores and independently adjudicated manuscript problems
Bias/fairness
Performance by cancer type, country, institution type, study design, and author characteristics
Security
Successful adversarial or prompt-injection attacks
Confidentiality
Unauthorized disclosure or retention events
Human workload
Active reviewer/editor time
Timeliness
Submission-to-review and submission-to-decision time
Review quality
Independent blinded quality scores
Decision quality
Subsequent appeals, reversals, corrections, and major postpublication problems

No single metric should determine readiness.
A — Achievable
The 2026 evidence suggests that partial automation is achievable now.
TMI demonstrates feasible integration into medical editorial workflows [5,6]. AI-generated cardiology reviews demonstrate that substantive critiques can be produced quickly [7]. The Review Feedback Agent provides randomized evidence that AI can improve human reports [9]. AAAI-26 demonstrates technical scalability [10]. 
Conversely, autonomous acceptance/rejection is not yet demonstrably achievable at a medical-journal safety standard because of calibration failures [1], prompt injection [11], confidentiality requirements [2,3], and weak desk-decision performance [12]. 
R — Relevant
The goal is especially relevant to oncology because peer-review demand is increasing while the work requires increasingly specialized expertise spanning molecular oncology, pathology, imaging, biostatistics, genomics, immunotherapy, surgery, radiation oncology, real-world evidence, and increasingly complex trial designs.
AI’s highest value may therefore be preserving expert attention rather than replacing experts. If AI can perform clerical checking and identify candidate inconsistencies, an oncologist can spend a larger fraction of review time evaluating whether the scientific question matters and whether the authors’ clinical interpretation is justified.
That division of labor is more consistent with the 2026 evidence than an attempt to recreate the entire oncologist reviewer inside an LLM [1,13]. The 2026 medical-informatics scoping review similarly identifies efficiency opportunities while emphasizing governance, privacy, bias, and continued human oversight [13]. 
T — Time-bound
For the remainder of 2026, a high-impact oncology journal could reasonably structure implementation as follows.
August–September 2026: establish governance, define prohibited and permitted functions, negotiate data-security requirements, create an AI-use disclosure policy, and establish an adversarial-testing protocol.
October–November 2026: conduct a silent parallel evaluation. AI reviews the same submissions as humans, but AI output does not influence decisions. Compare AI findings with oncologists, statisticians, and editors.
November–December 2026: if prespecified safety criteria are satisfied, introduce AI only for low-risk functions such as checklist review, discrepancy detection, reviewer-feedback assistance, or editor matching.
By December 31, 2026: publish or publicly report validation results, including negative findings, subgroup performance, security testing, human override rates, and resource use.
Autonomous acceptance or rejection should not be a 2026 SMART objective. It should remain contingent on prospective evidence showing that autonomous judgment adds value without unacceptable loss of methodological, clinical, ethical, or security performance.

7. Economic implications: will AI change who is paid?
7.1 The present assumption should be clarified
It would be inaccurate to state that, in 2026, oncology journals generally “pay postdocs instead of journals.” The conventional peer-review system still relies heavily on unpaid specialist labor. A 2026 review in Naunyn-Schmiedeberg’s Archives of Pharmacology describes unpaid expert review as the predominant model and specifically raises the possibility that publishers could substitute unpaid human reviewers with inexpensive AI reviewing [16]. 
Furthermore, journal finances and reviewer compensation are separate issues. Publishers may receive subscription revenue, article-processing charges, society support, institutional agreements, advertising revenue, or other income. Paying reviewers does not make the journal itself unnecessary, because editorial management, production, indexing, archiving, integrity screening, infrastructure, and governance continue to carry costs.
7.2 The strongest 2026 paid-review experiment
Biology Open provides an important 2026 economic comparator. Its Fast & Fair system compensated reviewers £220 per manuscript, conditional on completing a timely review that met editorial quality expectations [15]. Mean time to a first decision with reviews fell from 37.7 working days under the conventional process to 5.5 working days under Fast & Fair; invitations were also accepted at a higher rate, and accepted invitations were more likely to result in completed reviews [15]. 
This is not an oncology journal, and the 2026 report describes an implementation originating earlier. It should therefore be treated as an economic proof of concept, not evidence of a current oncology compensation standard.
7.3 How AI could make reviewer payment more rather than less plausible
At first glance, AI might seem to remove the need to pay reviewers. A different outcome is possible.
Suppose a traditional manuscript requires several hours of unpaid expert review. If AI can safely automate administrative checking, literature cross-checking, consistency review, and preliminary issue extraction, the remaining human task becomes smaller but more specialized.
Under that model, a journal could economically compensate humans for the scarce component:
oncology-specific interpretation;


expert biostatistical assessment;


pathology or imaging interpretation;


evaluation of therapeutic significance;


assessment of adverse-event relevance;


validation of biomarker claims;


causal reasoning;


ethical judgment; and


adjudication when reviewers disagree.


In other words, AI could change peer review from a large quantity of unpriced academic labor into a smaller quantity of explicitly priced expert adjudication.
7.4 Role of postdoctoral researchers
Qualified postdoctoral researchers could benefit substantially from such a model, but career stage alone should not determine eligibility.
A future oncology system might certify reviewers by demonstrated competence—for example, oncology postdoctoral fellows with appropriate publication experience, statistical expertise, tumor-specific expertise, or methodological training. A postdoctoral researcher who provides high-value human verification could then receive:
monetary compensation;


documented academic credit;


reviewer-performance records;


training and certification; or


eligibility for progressively more complex review assignments.


This would address a longstanding asymmetry: early-career scientists often perform substantial reviewing work without formal compensation or fully visible credit.
However, no 2026 oncology-wide system identified in this review has institutionalized such a postdoc-payment model. It should be characterized as a plausible economic redesign rather than a current fact.
7.5 Possible future economic configurations
Model
AI role
Human compensation
Likely 2026–near-term feasibility
Traditional
Minimal
Usually unpaid
Current baseline
AI + unpaid expert
Routine AI assistance
Usually unpaid
Highly plausible
AI + paid expert adjudication
AI handles routine checks
Humans paid for high-value judgment
Increasingly plausible; Biology Open provides economic precedent [15]
Paid certified early-career reviewers
AI assists; trained postdocs verify
Direct compensation plus credentialing
Plausible, but not established in oncology
AI replaces most human review
AI handles scientific judgment
Minimal reviewer expenditure
Technically conceivable but unsupported for medical use
Fully autonomous journal
AI reviews and decides
Little/no human reviewing
Not supported by 2026 medical evidence

The key economic uncertainty is therefore not merely whether AI becomes cheaper than a reviewer. It is who captures the productivity gain: publishers, authors through lower fees, institutions, AI vendors, or human experts through compensated review.
Teixeira da Silva explicitly identifies the risk that free human labor may simply be replaced by inexpensive AI rather than creating a more equitable reviewer economy [16]. 

8. Recommended target operating model for an oncology journal
The most defensible architecture emerging from the 2026 evidence is a human-first, AI-second, human-final process.
Step 1: secure intake
The manuscript enters a journal-controlled environment. No unpublished manuscript content is sent to an unapproved external AI service. This follows ICMJE confidentiality principles [2]. 
Step 2: automated administrative review
AI examines formatting, required declarations, reporting checklists, missing information, references, duplicate statements, table-text inconsistencies, and possible integrity signals.
Step 3: AI-assisted editor assignment
A TMI-like matching architecture recommends the most appropriate associate editor and candidate reviewer expertise [6]. 
Step 4: independent human review first
Human oncology reviewers assess scientific merit without seeing the AI critique. This protects against anchoring and preserves independent viewpoints, consistent with the second-pass model supported by the 2026 cross-community analysis [1]. 
Step 5: AI second-pass critique
After the initial human assessment, the reviewer receives AI-generated candidate concerns, missing checks, or questions.
Step 6: reviewer validation
Every AI concern must be accepted, rejected, or marked uncertain by an accountable human reviewer. AI-generated citations should be independently verified.
Step 7: AI review-quality feedback
A Review Feedback Agent-like layer asks whether the human report is specific, adequately grounded, internally consistent, and constructive [9]. 
Step 8: adversarial-content defense
The AI pipeline removes or neutralizes hidden instructions and tests for prompt injection before manuscript content reaches the reviewing model, because 2026 medical evidence demonstrates that hidden-text attacks can profoundly distort review scores and acceptance recommendations [11]. 
Step 9: human editorial synthesis
The associate editor sees the original human reviews, verified AI flags, disagreements, and specialist assessments. The associate editor—not the model—recommends a disposition.
Step 10: human final decision and disclosure
The responsible editor makes the final decision. The journal records which AI system and version was used and what functions it performed.
This architecture captures most of the efficiency demonstrated in 2026 while avoiding the most consequential unsupported leap: transferring editorial authority to an opaque probabilistic system.

9. Overall SMART scorecard as of August 15, 2026
SMART dimension
Status of AI replacing medical peer review
Assessment
Specific
Narrow review tasks can now be clearly defined and automated
Strong
Measurable
Review quality, error detection, security, bias, and time can be prospectively measured, but no single gold-standard metric exists
Moderate-to-strong
Achievable
Reviewer support, editor matching, second opinions, structured checks, and review-quality coaching are achievable
Strong for augmentation; weak for full replacement
Relevant
Reviewer scarcity and submission volume make automation highly relevant, especially where expert time is costly
Strong
Time-bound
Controlled pilots can be deployed during 2026; autonomous medical decision authority lacks adequate validation
Strong for hybrid deployment; not ready for autonomous takeover

SMART conclusion: the evidence supports a 2026 goal of AI-augmented oncology peer review, not an objective of eliminating human review.

10. Conclusion
As of August 15, 2026, AI is beginning to alter the architecture of scientific peer review, but the claim that it has already replaced human peer review in medical or oncology journals is not supported by the 2026 evidence.
The most comprehensive contemporary policy survey found only one actively AI-assisted medical journal among 48 leading journals—IEEE Transactions on Medical Imaging—while most prohibited reviewer AI outright or allowed only restricted uses [1]. TMI’s AI4TMI program is therefore the most consequential current medical case because it integrates AI into real editorial processes rather than merely testing LLMs retrospectively [5,6]. Yet its significance lies precisely in its hybrid design rather than in the elimination of humans. 
Oncology is even less ready for autonomous replacement. JAMA Oncology, through current JAMA Network guidance, prohibits external AI use for peer review on confidentiality grounds [3]. Oncology-specific 2026 research is investigating LLM scientific-merit screening [8], but systematic score inflation illustrates why such models require calibration and human adjudication. 
The strongest positive evidence across 2026 does not show that AI is better when humans are removed. Instead, it shows that AI is particularly effective when it improves human work: recommending editors, identifying additional concerns, generating supplemental reviews, improving reviewer reports, and reducing repetitive workload [6,9,10]. At the same time, medical experiments show that AI review can be manipulated by hidden prompts [11], while editorial-decision studies demonstrate inadequate reliability for autonomous disposition [12]. 
Accordingly, the likely trajectory is not a single “AI takeover” event. It is a progressive decomposition of peer review into components. Routine components will increasingly be automated. High-value scientific judgment will remain human for longer. If publishing economics evolve intelligently, the savings from automation could support compensation for scarce expert review—including work performed by appropriately qualified postdoctoral researchers—rather than simply replacing unpaid humans with inexpensive AI. The Biology Open paid-review experience demonstrates that reviewer compensation can materially improve timeliness [15], but no corresponding oncology-wide payment transition has yet occurred [16]. 
Thus, the most realistic 2026 endpoint for medical and oncology publishing is not AI replacing peer review, but AI reorganizing it: machines increasingly perform scalable checking and critique, while accountable humans retain clinical interpretation, scientific responsibility, and final publication authority.

References — BibTeX
[1]
@article{fichtl2026aiassisted,
  author = {Fichtl, Alexander M. and Ellinger, Lukas and Kelber, Josefin and Olík, Kryštof and Groh, Georg},
  title = {{AI-Assisted Peer Review Across Research Communities: From Reviewer AI Policies to LLM Review Quality}},
  journal = {arXiv preprint arXiv:2608.03581},
  year = {2026},
  doi = {10.48550/arXiv.2608.03581},
  url = {https://doi.org/10.48550/arXiv.2608.03581},
  note = {Submitted August 4, 2026}
}
[2]
@misc{icmje2026ai,
  author = {{International Committee of Medical Journal Editors}},
  title = {{Recommendations for the Conduct, Reporting, Editing, and Publication of Scholarly Work in Medical Journals: V. Use of Artificial Intelligence in Publishing}},
  year = {2026},
  month = {January},
  url = {https://www.icmje.org/recommendations/browse/artificial-intelligence/},
  note = {Updated January 2026; accessed August 15, 2026}
}
[3]
@article{flanagin2026updated,
  author = {Flanagin, Annette and Perlis, Roy H. and Bibbins-Domingo, Kirsten},
  title = {{Updated Guidance for Author Use of AI in Medical Publication}},
  journal = {JAMA},
  year = {2026},
  doi = {10.1001/jama.2026.16613},
  url = {https://doi.org/10.1001/jama.2026.16613},
  note = {Published online August 10, 2026}
}
[4]
@article{giusti2026oncology,
  author = {Giusti, Raffaele and Filetti, Marco and Lombardi, Pasquale and Lo Bianco, Francesca and Sganga, Stefano and Giovagnoli, Tommaso and Iannantuono, Giovanni Maria and Spinazzola, Andrea and Santini, Daniele and Mariniello, Monica and Porzio, Giampiero and Ibrahim, Mohsen and Daniele, Gennaro},
  title = {{Artificial Intelligence in Oncology Publishing: A Systematic Review and Policy Analysis of High-Impact Journals}},
  journal = {Frontiers in Oncology},
  volume = {16},
  pages = {1717048},
  year = {2026},
  doi = {10.3389/fonc.2026.1717048},
  url = {https://doi.org/10.3389/fonc.2026.1717048},
  note = {Published April 1, 2026}
}
[5]
@article{wang2026air,
  author = {Wang, Ge and Çukur, Tolga and Kruger, Uwe and Ferina, Jennifer and Shan, Hongming},
  title = {{Editorial AI Reviewer (AIR) Trial for Responsible, Secure, and Efficient Peer Review}},
  journal = {IEEE Transactions on Medical Imaging},
  volume = {45},
  number = {3},
  pages = {867--869},
  year = {2026},
  doi = {10.1109/TMI.2026.3658770},
  url = {https://doi.org/10.1109/TMI.2026.3658770},
  note = {Published January 28, 2026}
}
[6]
@article{xu2026assignment,
  author = {Xu, Xuanang and Yan, Joshua and Nwachukwu, Gloria and Shan, Hongming and Kruger, Uwe and Wang, Ge},
  title = {{Artificial Intelligence-Aided Assignment of Journal Submissions to Associate Editors---A Feasibility Study on IEEE Transactions on Medical Imaging}},
  journal = {Visual Computing for Industry, Biomedicine, and Art},
  volume = {9},
  pages = {1},
  year = {2026},
  doi = {10.1186/s42492-025-00212-y},
  url = {https://doi.org/10.1186/s42492-025-00212-y},
  note = {Version of record published January 12, 2026}
}
[7]
@article{zancanaro2026peer,
  author = {Zancanaro, Edoardo and Giannopoulos, Andreas and Gimelli, Alessia and Kresoja, Karl-Patrik},
  title = {{AI as a Peer Reviewer: A Blinded Comparative Study of LLM-Generated and Human Reviews in a Cardiology Journal}},
  journal = {European Heart Journal - Imaging Methods and Practice},
  volume = {4},
  number = {1},
  pages = {qyag097},
  year = {2026},
  doi = {10.1093/ehjimp/qyag097},
  url = {https://doi.org/10.1093/ehjimp/qyag097}
}
[8]
@article{cohen2026abstractselection,
  author = {Cohen, Lauren N. and Seibert, Drake and Kosten, Thomas and Wolfrath, Nathan and Al-Hilli, Zahraa and Kantor, Olga and Singh, Puneet and Teshome, Mediget and Blair, Sarah and Hieken, Tina J. and Wilke, Lee G. and Kothari, Anai N. and Cortina, Chandler S.},
  title = {{Streamlining the Abstract Selection Process for the American Society of Breast Surgeons' Annual Meeting by Utilizing Large Language Models}},
  journal = {Annals of Surgical Oncology},
  year = {2026},
  doi = {10.1245/s10434-026-20138-w},
  url = {https://doi.org/10.1245/s10434-026-20138-w},
  note = {Published online July 6, 2026}
}
[9]
@article{thakkar2026largescale,
  author = {Thakkar, Nitya and Yuksekgonul, Mert and Silberg, Jake and Garg, Animesh and Peng, Nanyun and Sha, Fei and Yu, Rose and Vondrick, Carl and Zou, James},
  title = {{A Large-Scale Randomized Study of Large Language Model Feedback in Peer Review}},
  journal = {Nature Machine Intelligence},
  volume = {8},
  pages = {326--336},
  year = {2026},
  doi = {10.1038/s42256-026-01188-x},
  url = {https://doi.org/10.1038/s42256-026-01188-x},
  note = {Published February 23, 2026}
}
[10]
@article{biswas2026aaai,
  author = {Biswas, Joydeep and Schoepp, Sheila and Vasan, Gautham and Opipari, Anthony and Zhang, Arthur and Hu, Zichao and Joseph, Sebastian and Lease, Matthew and Li, Junyi Jessy and Stone, Peter and Wagstaff, Kiri L. and Taylor, Matthew E. and Jenkins, Odest Chadwicke},
  title = {{AI-Assisted Peer Review at Scale: The AAAI-26 AI Review Pilot}},
  journal = {arXiv preprint arXiv:2604.13940},
  year = {2026},
  doi = {10.48550/arXiv.2604.13940},
  url = {https://doi.org/10.48550/arXiv.2604.13940},
  note = {Submitted April 15, 2026}
}
[11]
@article{choi2026invisible,
  author = {Choi, Byungjin and Jun, Tae Joon and Sung, Joung Won and Park, Il Woo and Lee, Jeong-Moo and Cho, Soo Ick and Park, Hyung Jun and Lee, Ro Woon and Suh, Jungyo},
  title = {{Invisible Text Injection and Peer Review by AI Models}},
  journal = {JAMA Network Open},
  volume = {9},
  number = {1},
  pages = {e2552099},
  year = {2026},
  doi = {10.1001/jamanetworkopen.2025.52099},
  url = {https://doi.org/10.1001/jamanetworkopen.2025.52099},
  note = {Published January 16, 2026}
}
[12]
@article{lupon2026desk,
  author = {Lupon, Elise and Bérard, Quentin and Migaud, Henri and Clavert, Philippe and Micicoi, Grégoire},
  title = {{Can Large Language Models Provide High-Quality Desk Review Decisions in an Orthopaedic Surgery Journal? A Concordance Study Comparing Three AI Models to Human Editorial Decisions}},
  journal = {Orthopaedics \& Traumatology: Surgery \& Research},
  pages = {104801},
  year = {2026},
  doi = {10.1016/j.otsr.2026.104801},
  url = {https://doi.org/10.1016/j.otsr.2026.104801},
  note = {Published online July 24, 2026}
}
[13]
@article{nabavi2026scoping,
  author = {Nabavi, Ali and Safari, Farima and Shmoury, Abdel Hadi and Tabet, Salam and Perdomo-Luna, Camilo and Celi, Leo Anthony},
  title = {{Artificial Intelligence in Scholarly Peer Review: A Scoping Review of Applications, Risks, and Governance Challenges}},
  journal = {International Journal of Medical Informatics},
  volume = {214},
  pages = {106418},
  year = {2026},
  doi = {10.1016/j.ijmedinf.2026.106418},
  url = {https://doi.org/10.1016/j.ijmedinf.2026.106418},
  note = {Published online April 6, 2026}
}
[14]
@article{manik2026adapt,
  author = {Manik, Md Motaleb Hossen and Wang, Ge},
  title = {{ADAPT: AI-Driven Decentralized Adaptive Publishing Testbed}},
  journal = {arXiv preprint arXiv:2604.04077},
  year = {2026},
  doi = {10.48550/arXiv.2604.04077},
  url = {https://doi.org/10.48550/arXiv.2604.04077},
  note = {Submitted April 5, 2026}
}
[15]
@article{gorelick2026expanded,
  author = {Gorelick, Daniel A. and Clark, Alejandra},
  title = {{Expanded Implementation of Fast \& Fair Paid Peer Review Reduces Time to First Decision Without Reducing Review Quality in a Biology Journal}},
  journal = {bioRxiv},
  year = {2026},
  doi = {10.64898/2026.06.02.729548},
  url = {https://doi.org/10.64898/2026.06.02.729548},
  note = {Preprint posted June 2026}
}
[16]
@article{teixeiradasilva2026paying,
  author = {Teixeira da Silva, Jaime A.},
  title = {{Paying Peer Reviewers: Benefits, Risks, and Challenges}},
  journal = {Naunyn-Schmiedeberg's Archives of Pharmacology},
  volume = {399},
  number = {7},
  pages = {9453--9470},
  year = {2026},
  doi = {10.1007/s00210-025-04969-0},
  url = {https://doi.org/10.1007/s00210-025-04969-0},
  note = {Published January 31, 2026}
}

