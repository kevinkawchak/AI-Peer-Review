The 2026 State of AI Peer Review in Scholarly Journals: A SMART-Framework Review
Abstract
As of August 15, 2026, artificial intelligence has entered substantive peer-review workflows, but the available 2026 evidence does not support the claim that established scholarly journals have broadly replaced human peer reviewers or human editorial judgment with autonomous AI. The most advanced journal-specific example identified in the 2026 literature is the IEEE Transactions on Medical Imaging (TMI) AI Reviewer trial, whereas large publishing organizations such as Frontiers and Springer Nature primarily employ AI for research-integrity screening, editorial support, reviewer identification, and other bounded tasks. A 2026 survey of 111 publication venues found that, among 48 high-impact medical journals, 58% prohibited reviewer AI use and 38% permitted only partial use; TMI was the sole journal in that sample classified as actively employing AI-assisted reviewing [1]. 
The strongest evidence that AI can produce useful reviews at scale comes not from journals but from the AAAI-26 conference, where 22,977 papers received an additional, clearly labeled AI review in less than 24 hours. Importantly, no human reviewer was replaced, the AI supplied no acceptance score or recommendation, and final decision authority remained human [3].  At the opposite extreme, the AI Scientists Conference (AISC 2026) explicitly proposes an experimental scholarly process in which AI agents conduct review, discussion, rebuttal, and acceptance decisions without humans, but AISC is a conference rather than an established journal and therefore should be interpreted as a proof-of-concept for autonomous review rather than evidence that journal publishing has already undergone an AI takeover [14]. 
Using the SMART framework—Specific, Measurable, Achievable, Relevant, and Time-bound—this review concludes that the technically and institutionally most successful 2026 model is hybrid AI-human peer review, not human replacement. A parallel development is the emergence of directly compensated human reviewing. Biology Open’s Fast & Fair model, evaluated in 2026, pays qualified reviewers £220 per manuscript conditional on timeliness and quality; other journals, such as Advances in Psychology, were reported in 2026 to pay $100 per completed qualifying review [11–13].  Thus, a plausible future is not simply “AI instead of reviewers,” but a division of labor in which inexpensive AI performs repetitive screening and analytical support while scarce expert human judgment becomes more explicitly recognized and, in some systems, paid.
Scope and interpretation of “replacement”
This review deliberately restricts its evidentiary base to materials published, posted, or officially dated in 2026, with a cutoff of August 15, 2026. Some 2026 studies necessarily analyze manuscripts or workflows originating before publication of the study, but no pre-2026 source is included in the reference section or used as an independent evidentiary basis.
“AI replacing peer review” also requires a precise definition. There is a material difference between an AI system that checks images or recommends reviewers, an AI system that drafts an additional review for a human editor, an AI system that assigns an acceptance score, and an AI system that independently determines whether a manuscript is published. The 2026 evidence shows rapid movement through the first two categories, substantial experimentation with the third, and only experimental non-journal examples of the fourth [1–4,14]. 
2026 status by implementation type
Venue or system
2026 AI role
Human peer review replaced?
Significance
IEEE Transactions on Medical Imaging
AI Reviewer/AIR trial integrated with journal review
No
Most advanced journal-specific AI-review implementation identified in the surveyed medical-journal sample [1,2]
Frontiers journals
AIRA performs more than 40 AI-supported integrity and quality checks before expert review
No
Mature production use of AI to protect and focus human review [5,6]
Springer Nature journal workflows
AI embedded in screening, editorial evaluation, integrity, and reviewer-support workflows, with explicit human oversight
No
Major publisher-scale operational integration rather than reviewer replacement [7]
Nature Nanotechnology
Editorial position permits/supports thoughtful AI assistance but rejects replacement of human judgment
No
Illustrates a prominent 2026 editorial boundary on autonomous review [8]
AAAI-26
One additional AI review for every full-review main-track paper
No
Strongest large-scale empirical demonstration of substantive AI reviewing, but a conference rather than a journal [3]
NeurIPS 2026
Randomized experiment comparing no LLM assistance, open-ended assistance, and structured assistance
No
Particularly useful experimental design for measuring causal effects of AI assistance [4]
AISC 2026
AI review, discussion, rebuttal, and final decision
Yes, by design
Explicit autonomous “takeover” experiment, but not an established journal [14]
Biology Open Fast & Fair
Precontracted, directly paid human reviewers
No; human review strengthened
Demonstrates that redesigning reviewer incentives is an alternative or complement to automation [11,12]

The most important correction to the premise of an AI “takeover” is therefore that no established journal could be verified from the 2026 evidence reviewed here as having completely eliminated expert human review and human editorial authority in favor of autonomous AI. Within Fichtl et al.’s 2026 sample of high-impact medical journals, only TMI had an active AI-assisted reviewing initiative; the dominant journal policy remained prohibition or carefully delimited assistance [1].  This distinction is also consistent with the 2026 Nature Nanotechnology editorial position that generative AI can support peer review but should not replace human judgment, expertise, and critical thinking [8]. 

S — Specific: What precisely is being replaced?
The clearest 2026 development is functional decomposition of peer review. Instead of attempting to replace the reviewer as one indivisible role, successful systems separate peer review into tasks that differ in risk and required expertise. AI is increasingly assigned screening, consistency checking, literature/context retrieval, detection of possible technical problems, reviewer recommendation, structured criticism, and research-integrity checks. Humans retain interpretation of novelty, scientific importance, methodological context, unusual domain-specific circumstances, conflicts among reviews, appeals, and final publication responsibility [1,3,5–9]. 
This distinction explains why TMI is more appropriately described as an AI-assisted journal than an AI-reviewed journal. Its 2026 AIR editorial describes an IEEE-supported effort to develop and evaluate AI systems as assistants within TMI’s peer-review workflow [2]. The 2026 cross-venue analysis independently classified TMI, through its AI4TMI initiative, as the only active AI-assisted reviewing implementation among the 48 medical journals examined [1].  The significance of TMI is therefore substantial, but it would be inaccurate to say that TMI’s human reviewers have been replaced.
Frontiers provides another instructive implementation. Its AIRA system performs more than 40 AI-powered quality and integrity checks before editorial assessment, including checks related to plagiarism, ethical compliance, image manipulation, and possible paper-mill activity. Flags are presented for human review; Frontiers explicitly states that AIRA does not replace editorial judgment [5].  Its April 2026 BE WISE guidance additionally requires transparency, accountability, appropriate tools, verification, integrity safeguards, and equity, with “permission-to-proceed” checkpoints governing higher-impact uses [6]. 
Springer Nature illustrates a comparable publisher-scale approach. Its March 2026 announcement stated that AI tools were embedded throughout publishing workflows for screening, editorial evaluation, research integrity, and reviewer support and that deployment would increase further during 2026. The publisher explicitly described the model as one with expert human oversight and accountability rather than autonomous editorial decision-making [7]. 
The Specific component of a SMART assessment therefore yields a clear answer: in 2026, AI is replacing components of reviewer labor much faster than it is replacing reviewers as accountable scientific decision-makers.

M — Measurable: What 2026 evidence shows that AI peer review actually works?
The AAAI-26 pilot provides the most compelling quantitative evidence of substantive AI-review capability. The system generated an official, clearly identified AI review for each of 22,977 papers that reached full review. The AI reviews were produced in less than 24 hours, at a reported model cost below $1 per paper; the cost was covered through donated API credits. Crucially, the AI review appeared alongside at least two human reviews, contained no score or acceptance recommendation, and displaced no human reviewer [3]. 
The system was considerably more sophisticated than a single prompt sent to a general-purpose language model. It used a multistage pipeline examining the paper’s scientific story, presentation, evaluations, correctness, and significance, followed by self-critique and revision. Intermediate outputs and logs were retained for auditing and human oversight [3].  This architecture is one reason AAAI-26 should be treated as a benchmark implementation: the effective unit is not “an LLM,” but a governed review system built around specialized stages, tools, logging, and role constraints.
Among 5,834 survey responses, AI reviews were rated above human reviews on six of nine review-quality dimensions. Their largest measured advantages were identification of technical errors (+0.67 on the study’s comparison scale), identification of previously unconsidered points (+0.61), suggestions for presentation improvement (+0.54), research-design suggestions (+0.49), and thoroughness (+0.48). Conversely, AI reviews were judged more likely to overemphasize minor problems (-0.38), somewhat more likely to contain technical errors themselves (-0.22), and slightly more likely to provide incorrect or unhelpful suggestions (-0.11) [3]. 
The same results reveal why replacement remains premature. Although 53.9% of respondents considered the AI reviews useful and 61.5% expected future AI reviews to be useful, 49.4% of program-committee respondents said the AI review overlooked issues a human reviewer would probably have caught. Simultaneously, 46.6% said AI identified concerns difficult for a human reviewer to catch. Only 13.8% reported that the AI review changed their interpretation or evaluation of the paper [3].  This is unusually strong empirical evidence for complementarity: AI and humans make different errors and discover different problems.
Fichtl et al.’s August 2026 cross-community evaluation arrives at much the same conclusion. AI reviews can be detailed, broad, and actionable, but the researchers identified overly positive recommendations, weak calibration, generic criticism, and uneven evidence grounding. They specifically recommend a second-pass arrangement in which a human first reaches an independent judgment and only afterward considers AI-generated candidate concerns, thereby reducing anchoring and preserving diversity of judgment [1]. 
The medical evidence is similarly cautious. In a 2026 JMIR AI algorithm-validation study, the best retrieval-augmented configuration obtained an exact-match accuracy of only 0.35 and a looser accuracy of approximately 0.78 on the study’s journal-tier classification task. The authors concluded that the tested LLMs were inadequate for independent peer review and that human supervision remained nonnegotiable [9].  The finding is particularly important because it demonstrates the difference between producing persuasive-looking review prose and making calibrated publication judgments.

A — Achievable: Which implementations appear most effective?
1. Most effective substantive review implementation: AAAI-26’s bounded hybrid model
AAAI-26 currently provides the strongest transferable implementation pattern, even though it is a conference. Its effectiveness comes from five design choices operating together: multistage scientific analysis, access to tools rather than text generation alone, self-critique, logging/auditability, and a deliberately bounded institutional role. The AI could identify potential weaknesses but could not independently award acceptance scores, issue final recommendations, or eliminate human reviewers [3]. 
The main lesson for journals is not that autonomous reviewing has arrived, but that AI review becomes substantially more useful when it is engineered as an auditable scientific-analysis pipeline and inserted as an additional source of evidence rather than as an unaccountable replacement decision-maker.
2. Most advanced journal-specific implementation: TMI’s AIR/AI4TMI trial
For journals, TMI deserves particular attention because it is one of the clearest 2026 attempts to move AI beyond integrity screening and into substantive review assistance. The AIR trial is explicitly framed around responsible, secure, and efficient peer review, while human-review data and AI-review outputs can be evaluated comparatively [2]. 
This design is promising because it addresses a fundamental weakness in claims about AI review: one cannot improve AI reviewers without collecting structured comparisons between AI criticism and domain-expert criticism. A paired-review trial can establish where AI finds legitimate concerns, where it fabricates or misprioritizes concerns, and which categories of manuscripts are inappropriate for automation.
3. Most effective production-scale risk reduction: Frontiers AIRA
Frontiers’ implementation is arguably more mature operationally, although it is less ambitious in terms of replacing substantive scientific judgment. More than 40 automated checks act as a protective layer before editors and expert reviewers invest time in a manuscript [5].  This is a highly practical application because many integrity problems are pattern-detection problems and can be escalated rather than autonomously adjudicated.
Frontiers’ 2026 governance framework is equally important. Its BE WISE approach makes human accountability explicit and creates checkpoints around oversight, policy compliance, permitted data inputs, and verification [6].  For journals concerned about confidentiality, reviewer responsibility, or inappropriate uploading of unpublished manuscripts into third-party systems, governance architecture may be as consequential as model accuracy.
4. Most effective publisher-scale integration: Springer Nature
Springer Nature demonstrates that AI adoption need not begin with generation of complete referee reports. Its 2026 strategy embeds AI within existing publishing and peer-review infrastructure while retaining human oversight [7].  From an implementation perspective, reviewer identification, triage, research-integrity screening, and editor assistance have lower epistemic risk than delegating acceptance decisions. These functions also remove administrative workload that contributes to delays without pretending that matching a manuscript to a reviewer is equivalent to judging the science.
5. Most methodologically useful experiment underway: NeurIPS 2026
NeurIPS 2026 is running a voluntary randomized experiment in which participating reviewers are assigned, at the paper level, to no LLM assistance, open-ended LLM assistance, or structured LLM assistance [4].  This design is important because much of the AI-peer-review literature compares AI and human outputs after the fact. Randomization can instead determine whether AI assistance causally changes reviewer quality, behavior, effort, or decisions. For journals considering adoption, controlled comparisons of this kind are preferable to simply turning on an AI feature and measuring user satisfaction.
6. Why autonomous review is not yet an achievable journal standard
Technical weaknesses remain sufficiently serious that a fully autonomous journal workflow would be difficult to justify under current evidence. The 2026 cross-venue study found miscalibration and overly positive AI judgments [1]; the JMIR AI validation found insufficient independent decision accuracy [9]; and Li et al. demonstrated that AI-mediated review scores could be manipulated through relatively superficial rephrasing of manuscript abstracts. Their strongest tested attack succeeded approximately 38% of the time, with success exceeding 50% when the original AI evaluation favored rejection [10]. 
This creates a particularly important risk for autonomous journals: once authors know what models or model families evaluate submissions, scientific writing may increasingly be optimized for the evaluator rather than for scientific validity. The resulting problem resembles search-engine optimization, except that the optimized objective is a publication decision.

R — Relevant: Why this transition matters for scientific publishing
AI peer review is relevant because the problem is not simply the quality of individual reports; it is the capacity and incentive structure of the entire publication system. AI can generate parallel analyses almost instantly, operate consistently across large submission volumes, search for overlooked issues, and perform repetitive checks that humans are poorly incentivized to undertake. Yet science also depends on tacit domain knowledge, causal reasoning, evaluation of novelty, recognition of unusual but legitimate methodological choices, and accountability for consequential decisions. The strongest 2026 evidence therefore supports a division of labor rather than an undifferentiated substitution of machines for scientists [1,3,8,9]. 
The human-accountability issue becomes especially important for journals. Conference acceptance is consequential, but journals create durable records that may influence clinical medicine, regulation, scientific priority, and subsequent research programs. La Rosa and Nasser’s 2026 discussion of AI in peer review warns specifically that delegating all or part of review to AI can fail to identify methodological problems if responsibility is not carefully governed [15].  The journal sector’s more restrictive posture in the 2026 Fichtl survey is therefore not merely technological conservatism; it also reflects confidentiality and accountability constraints [1]. 

Reviewer payment: will AI cause money to move from journals to postdoctoral researchers?
The 2026 evidence supports a more nuanced conclusion than the proposition that “postdocs will now be paid instead of journals.” There is no field-wide 2026 system under which publishing payments have been redirected from journals to postdoctoral researchers. Journals and publishers continue to provide editorial management, technology, preservation, production, integrity infrastructure, and dissemination. What is beginning to change is that a small number of journals are treating review itself as compensable expert labor rather than automatically expecting it to be donated.
The strongest current example is Biology Open’s Fast & Fair initiative. In its 2026 evaluation, precontracted reviewers were paid £220 per manuscript, contingent on submitting their work on time and satisfying editorial quality expectations. The expanded implementation reported a mean of 5.5 working days to a first decision with reviews compared with 37.7 working days under conventional review. Invitation acceptance was reported at 67% versus 23%, and completion among accepted invitations at 98% versus 87%; final acceptance rates remained similar across the two pathways [11].  Nature’s July 2026 assessment summarized the result as approximately an 85% reduction in time to the first editorial decision while maintaining review quality [12]. 
A second 2026-reported model is Advances in Psychology, which pays $100 per qualifying completed review. More than 500 reviewers had reportedly registered with the system, and the journal’s editor attributed easier reviewer recruitment and fewer reminders in part to compensation [13].  These arrangements compensate reviewers directly, but they do not limit eligibility specifically to postdoctoral researchers. Depending on journal requirements, paid reviewers can be faculty members, independent researchers, postdoctoral researchers, or other appropriately qualified specialists.
The interaction between AI and paid reviewing may be more consequential than either reform alone. AAAI-26 reported an AI-generation cost below $1 per paper, whereas Biology Open’s human model pays £220 for a qualifying review [3,11].  These figures are not directly comparable: the AAAI AI review was an additional, nonvoting review whose model costs were sponsor-supported, whereas Biology Open pays accountable human experts expected to satisfy contractual quality and timeliness requirements. Nevertheless, the cost difference creates an obvious economic incentive to automate tasks that do not require accountable expert judgment.
A plausible payment architecture emerging from these 2026 developments is consequently a two-layer market for review labor. Routine integrity checks, formatting checks, literature comparisons, initial concern generation, and report structuring can be automated at low marginal cost. Human reviewers can then concentrate on methodological verification, interpretation, novelty, domain-specific judgment, AI-output verification, and disputes. In such a structure, paying expert reviewers becomes more economically defensible because the compensated human is no longer being paid to perform every mechanical component of review; the payment purchases the scarce component—expert accountable judgment.
This is a forecast derived from the 2026 evidence, not an established industry-wide payment policy. Current evidence also indicates that paid review remains exceptional rather than standard and would require broader publisher participation to become systemic [13].  Accordingly, AI does not presently imply that publishers disappear from the payment chain, nor that postdoctoral researchers automatically become the primary paid reviewers. A more credible near-term change is that human review moves from an assumed unpaid service toward selectively contracted expert verification while AI absorbs lower-value repetitive work.

T — Time-bound: What is a realistic SMART objective for journals through December 31, 2026?
A defensible 2026 objective is not “replace human peer reviewers with AI by year-end.” The evidence does not support that target. A better SMART objective would be:
By December 31, 2026, journals piloting substantive AI peer review should implement and prospectively evaluate a human-accountable hybrid workflow in which AI performs predefined review tasks, all material AI findings are independently verifiable, final publication decisions remain under identified human editorial authority, reviewer-facing AI use is disclosed according to journal policy, and performance is measured against an appropriate human-review control on accuracy, turnaround time, concern detection, false-positive criticism, bias, appeals, confidentiality incidents, and reviewer workload.
This objective is Specific because the AI’s role is bounded; Measurable because performance is compared against explicit operational and scientific-quality indicators; Achievable because AAAI-26, TMI, Frontiers, and Springer Nature demonstrate that the necessary technical components already exist [2,3,5–7]; Relevant because it targets both reviewer capacity and scientific integrity; and Time-bound because participating journals can complete or report an initial comparative evaluation by the end of 2026.
A practical SMART status assessment as of August 15, 2026 is summarized below.
SMART dimension
2026 status
Assessment
Specific
AI roles are becoming clearly separable into screening, matching, critique generation, reviewer assistance, and decision support.
Substantially achieved for hybrid systems; not achieved for safe autonomous replacement.
Measurable
AAAI-26 provides large-scale outcome and user-response data; journal studies and trials provide smaller-scale measures.
Good evidence for assistance; inadequate evidence for autonomous journal decisions.
Achievable
Production-scale screening and AI co-review are demonstrably feasible.
Hybrid implementation is achievable now. Full replacement is not validated.
Relevant
AI directly addresses workload, turnaround, integrity screening, and reviewer scarcity. Paid-review experiments address the human incentive problem.
Highly relevant.
Time-bound
Multiple 2026 experiments can inform policies before wider deployment.
The appropriate 2026 milestone is controlled hybrid adoption and evaluation, not takeover.


Initiatives pointing toward an eventual AI-review “takeover”
The strongest explicit autonomous initiative is AISC 2026. Its organizers describe a scholarly process in which multiple AI reviewer agents evaluate papers, AI agents conduct discussion and rebuttal, and AI agents make acceptance decisions with zero human participation in the review pipeline [14].  This is significant precisely because it tests the institutional endpoint that conventional journals have so far avoided. Its scientific value will depend on whether autonomous agents can demonstrate calibration, resistance to manipulation, diversity of reasoning, and error detection comparable to independent experts.
AAAI-26 represents a much more conservative pathway to the same technological frontier: deploy AI at full operational scale, but prevent it from replacing reviewers or issuing acceptance recommendations [3]. NeurIPS 2026 occupies an intermediate experimental position by testing how different degrees and forms of LLM assistance affect human reviewers [4].  Together these initiatives outline three possible trajectories: AI as a supplementary reviewer, AI as a structured cognitive tool used by reviewers, and AI as an autonomous reviewing institution.
Journal publishing in 2026 is clearly following the first two trajectories rather than the third. TMI, Frontiers, and Springer Nature all preserve identifiable human authority, and Nature Nanotechnology has explicitly articulated the principle that AI should support rather than replace human judgment [2,5–8]. 

Overall assessment
The current status can be summarized in one sentence: 2026 is the year in which AI peer review became operationally credible at scale, but not the year in which reputable journals demonstrably replaced human peer review with autonomous machines.
The most successful implementations share a recurring architecture. They narrowly define AI responsibilities, retain human accountability, isolate high-risk decisions from automated outputs, disclose AI involvement, preserve audit trails, and evaluate AI against human performance rather than assuming that fluent prose constitutes expert judgment. AAAI-26 is presently the strongest large-scale demonstration of substantive AI-generated reviews; TMI is the clearest journal-level attempt to integrate an AI reviewer; Frontiers provides a mature example of AI-supported integrity screening; Springer Nature demonstrates publisher-scale workflow integration; and NeurIPS provides a strong experimental framework for determining when AI assistance actually improves human review [1–7]. 
At the same time, 2026 evidence exposes substantial barriers to full substitution. AI reviewers can be positively biased, poorly calibrated, overly focused on minor concerns, factually mistaken, weak at big-picture scientific significance, and vulnerable to strategic manipulation [1,3,9,10].  In high-stakes journal publishing, these limitations are difficult to reconcile with autonomous acceptance decisions.
The reviewer-payment experiments suggest a potentially important alternative to viewing human expertise primarily as a cost to be automated away. Biology Open’s 2026 results indicate that contractual payment can substantially improve reviewer responsiveness and turnaround without an observed deterioration in review quality [11,12].  If those findings generalize, AI and reviewer compensation need not be competing reforms. AI can make expert review more efficient, while payment recognizes that the remaining human contribution—methodological judgment, verification, accountability, and scientific interpretation—is valuable labor.
Accordingly, the most defensible SMART strategy for scholarly journals in the remainder of 2026 is AI augmentation plus stronger human accountability and incentives, rather than wholesale reviewer replacement. Fully autonomous peer review now exists as an experimental institutional concept, exemplified by AISC 2026, but its movement into established journal publication would require substantially stronger evidence on accuracy, robustness, confidentiality, bias, appeals, manipulation resistance, and accountability than is currently available [9,10,14]. 
References — 2026 sources only
@misc{fichtl2026aiassisted,
  author = {Fichtl, Alexander M. and Ellinger, Lukas and Kelber, Josefin and Olík, Kryštof and Groh, Georg},
  title = {{AI-Assisted Peer Review Across Research Communities: From Reviewer AI Policies to LLM Review Quality}},
  year = {2026},
  month = {August},
  howpublished = {arXiv preprint arXiv:2608.03581},
  url = {https://arxiv.org/abs/2608.03581},
  note = {Version 1 posted August 4, 2026; survey and evaluation of AI-assisted peer review across AI/NLP conferences and medical journals},
}

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
  note = {Published January 28, 2026; describes the journal's AI Reviewer trial and AI4TMI direction},
}

@misc{biswas2026aaai,
  author = {Biswas, Joydeep and Schoepp, Sheila and Vasan, Gautham and Opipari, Anthony and Zhang, Arthur and Hu, Zichao and Joseph, Sebastian and Lease, Matthew and Li, Junyi Jessy and Stone, Peter and Wagstaff, Kiri L. and Taylor, Matthew E. and Jenkins, Odest Chadwicke},
  title = {{AI-Assisted Peer Review at Scale: The AAAI-26 AI Review Pilot}},
  year = {2026},
  month = {April},
  howpublished = {arXiv preprint arXiv:2604.13940},
  url = {https://arxiv.org/abs/2604.13940},
  note = {Posted April 15, 2026; reports the full-scale AAAI-26 AI Review Pilot covering 22,977 papers},
}

@misc{neurips2026experiment,
  author = {{NeurIPS 2026}},
  title = {{NeurIPS 2026 AI-Assisted Reviewing Experiment}},
  year = {2026},
  organization = {Conference on Neural Information Processing Systems},
  url = {https://neurips.cc/Conferences/2026/ai-reviewing-experiment},
  note = {Official 2026 description of the randomized AI-assisted reviewing experiment; accessed August 15, 2026},
}

@misc{frontiers2026aira,
  author = {{Frontiers}},
  title = {{How Do You Know You Can Trust the Science You Read?}},
  year = {2026},
  month = {March},
  day = {5},
  organization = {Frontiers},
  url = {https://www.frontiersin.org/news/2026/03/05/how-do-you-know-you-can-trust-the-science-you-read},
  note = {Describes Frontiers' AIRA AI-powered review assistant, research-integrity checks, and continued human editorial responsibility},
}

@misc{frontiers2026bewise,
  author = {{Frontiers}},
  title = {{Frontiers Launches Unique AI Practical Guidance for Researchers, Editors, and Reviewers, and Calls for Policy Evolution}},
  year = {2026},
  month = {April},
  day = {13},
  organization = {Frontiers},
  url = {https://www.frontiersin.org/news/2026/04/13/frontiers-launches-unique-ai-practical-guidance-for-researchers-editors-and},
  note = {Introduces the BE WISE framework and operational checkpoints for responsible AI use in scholarly publishing},
}

@misc{springernature2026aitools,
  author = {{Springer Nature}},
  title = {{Springer Nature Embraces AI Tools Across the Publishing Process, Resulting in Less Friction and Increased Author Satisfaction}},
  year = {2026},
  month = {March},
  day = {12},
  organization = {Springer Nature Group},
  url = {https://group.springernature.com/gp/group/media/press-releases/ai-tools-support-less-friction-and-increased-author-satisfaction/27849346},
  note = {2026 publisher announcement describing expanded AI-supported publishing workflows with expert human oversight},
}

@article{naturenanotechnology2026peerreview,
  author = {{Nature Nanotechnology}},
  title = {{Peer Review in the Time of Artificial Intelligence}},
  journal = {Nature Nanotechnology},
  volume = {21},
  pages = {479},
  year = {2026},
  month = {April},
  doi = {10.1038/s41565-026-02177-2},
  url = {https://doi.org/10.1038/s41565-026-02177-2},
  note = {Published April 20, 2026; editorial position that generative AI may support but should not replace human judgment in peer review},
}

@article{shen2026llmpeerreview,
  author = {Shen, Selena Ming and Wang, Zifu and Paul, Krittika and Li, Meng-Hao and Huang, Xiao and Koizumi, Naoru},
  title = {{Evaluation of Large Language Models for Peer Review in Transplantation Research: Algorithm Validation Study}},
  journal = {JMIR AI},
  volume = {5},
  pages = {e84322},
  year = {2026},
  month = {February},
  doi = {10.2196/84322},
  url = {https://doi.org/10.2196/84322},
  note = {Published February 11, 2026; evaluates open-source LLMs and concludes that independent AI review remains insufficiently reliable},
}

@misc{li2026gaming,
  author = {Li, Lin and Zhang, Qi and Davies, Xander and Qiu, Jianing and Gal, Yarin},
  title = {{Gaming AI-Assisted Peer Reviews Poses New Risks to the Scientific Community}},
  year = {2026},
  month = {June},
  howpublished = {arXiv preprint arXiv:2606.10159},
  url = {https://arxiv.org/abs/2606.10159},
  note = {Posted June 8, 2026; demonstrates vulnerability of AI-assisted peer review to strategic manuscript rephrasing},
}

@misc{gorelick2026fastfair,
  author = {Gorelick, Daniel A. and Clark, Alejandra},
  title = {{Expanded Implementation of Fast \& Fair Paid Peer Review Reduces Time to First Decision Without Reducing Review Quality in a Biology Journal}},
  year = {2026},
  month = {June},
  howpublished = {bioRxiv preprint},
  doi = {10.64898/2026.06.02.729548},
  url = {https://doi.org/10.64898/2026.06.02.729548},
  note = {Posted June 3, 2026; reports expanded implementation of paid, precontracted peer review at Biology Open},
}

@article{naddaf2026paying,
  author = {Naddaf, Miryam},
  title = {{Why Paying Peer Reviewers Works, According to a Journal's Editor-in-Chief}},
  journal = {Nature},
  volume = {655},
  pages = {290--291},
  year = {2026},
  month = {July},
  doi = {10.1038/d41586-026-01973-z},
  url = {https://doi.org/10.1038/d41586-026-01973-z},
  note = {Published July 1, 2026; discusses Biology Open's compensated-reviewer model and reported turnaround improvements},
}

@misc{palmer2026payingreviewers,
  author = {Palmer, Kathryn},
  title = {{Will Paying Reviewers Ease the Peer Review Crisis?}},
  year = {2026},
  month = {May},
  day = {14},
  organization = {Inside Higher Ed},
  url = {https://www.insidehighered.com/news/faculty/books-publishing/2026/05/14/will-paying-reviewers-ease-peer-review-crisis},
  note = {Reports 2026 evidence and examples of compensated peer review, including Advances in Psychology and Biology Open},
}

@misc{aisc2026conference,
  author = {{AI Scientists Conference}},
  title = {{AISC 2026: The AI Scientists Conference}},
  year = {2026},
  organization = {aiXiv},
  url = {https://aixiv.science/aisc2026/},
  note = {Official 2026 conference site describing an experimental scholarly workflow in which AI agents conduct peer review, discussion, rebuttal, and final decisions without human participation},
}

@article{larosa2026elephant,
  author = {La Rosa, Giusy Rita Maria and Nasser, Mona},
  title = {{AI in Peer Review: The Elephant in the Editorial Room}},
  journal = {Evidence-Based Dentistry},
  volume = {27},
  pages = {23--24},
  year = {2026},
  month = {June},
  doi = {10.1038/s41432-026-01227-x},
  url = {https://doi.org/10.1038/s41432-026-01227-x},
  note = {Published June 4, 2026; discusses governance and methodological risks associated with delegating peer-review work to AI},
}

