# Research

This directory contains paired AI-generated literature reviews on the use of artificial intelligence in scholarly peer review. The research is organized into a general publishing track and a medical/oncology-focused track, with each subdirectory preserving the source prompt alongside outputs from ChatGPT and Claude generated on August 15, 2026.

## Directory structure

```text
research/
├── README.md
├── general-ai-review/
│   ├── README.md
│   ├── ChatGPT-5.6-15Aug26.md
│   └── Claude-Code-Opus-5-15Aug26.md
└── medical-oncology-ai-review/
    ├── README.md
    ├── Med-ChatGPT-5.6-15Aug26.md
    └── Med-Claude-Code-Opus-5-15Aug26.md
```

## Research tracks

### `general-ai-review/`

Examines the 2026 status of AI-assisted peer review across scholarly publishing using the SMART framework. The prompt asks the models to assess:

- the extent to which AI is replacing or augmenting human peer review;
- the most effective implementations reported in 2026;
- journals or publishing workflows moving toward AI-led review;
- initiatives that could accelerate broader AI adoption in peer review; and
- possible changes to reviewer compensation and publishing economics.

The directory contains the shared prompt in `README.md` and two independently generated reviews for comparison.

### `medical-oncology-ai-review/`

Applies the same research question specifically to medical publishing, with a preference for oncology. In addition to the general requirements above, the prompt requests an academic tone using U.S. spelling and focuses on the governance, safety, and implementation issues most relevant to medical and oncology journals.

The directory contains the medical/oncology prompt in `README.md` and two independently generated reviews for comparison.

## Shared research requirements

Both review tracks were designed around the following requirements:

- **2026-only evidence:** sources should be dated in 2026 unless an output explicitly identifies and justifies an exception.
- **SMART framing:** findings are organized or evaluated using Specific, Measurable, Achievable, Relevant, and Time-bound criteria.
- **Implementation focus:** reviews should distinguish between AI support for individual review tasks and full replacement of human reviewers or editorial decision-making.
- **Publishing economics:** reviews consider whether automation could change reviewer compensation, including the possibility of directly paying qualified reviewers such as postdoctoral researchers.
- **Traceable citations:** numbered in-text citations are intended to correspond to complete BibTeX entries containing DOI or URL information where available.

## Comparing the model outputs

The paired reports are useful for comparing how different AI systems interpret the same prompt, select evidence, qualify claims, structure a SMART assessment, and handle references. Differences between reports should be treated as material for comparison rather than as evidence that one version is necessarily authoritative.

## Verification note

These files are AI-generated research syntheses. Before using their claims or references in academic, editorial, policy, or clinical work, verify important statements against the original cited sources and confirm that bibliographic details, dates, DOIs, and URLs are accurate.
