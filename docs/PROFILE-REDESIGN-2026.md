# GitHub profile redesign — research and decision record

*Mission 1.0 · 12 November 2026 · Scope: public GitHub profile presentation, not application code.*

## What was actually reviewed

- Existing `kelwin-feitosa/kelwin-feitosa` README, assets, two scheduled workflows, and existing profile links.
- Public README files for `supermarket-management-api`, `assistente-financeiro`, `personaldev`, and `simulador-emprestimo-java`, plus repository visibility and archived state.
- **20 existing, independently retrieved profile READMEs** listed below, across minimal, descriptive, visual and dynamic styles.
- GitHub official documentation on the profile README, image variants for light/dark themes, and making projects understandable to hiring managers.

**Method:** direct inspection of README source and its content structure, not an empirical hiring study. Counts, impressions and trade-offs are exploratory. No claim is made that we ran a controlled recruiter usability study or benchmarked recruiting conversion.

## Twenty real reference profiles

The linked sources below were inspected directly as README text. Their composition can change over time.

| Profile | Observed approach | Usable lesson / limitation |
| --- | --- | --- |
| [anuraghazra](https://github.com/anuraghazra/anuraghazra) | Large visual intro, images, activity cards | Clear personal branding, but external cards can displace proof of work |
| [aralroca](https://github.com/aralroca/aralroca) | Short header, links, visual widgets | Easy entry points; project context still matters |
| [athul](https://github.com/athul/athul) | Compact link-oriented introduction | Minimal copy can feel confident, if work is readily accessible |
| [jh3y](https://github.com/jh3y/jh3y) | Image/logo-led near-empty README | Memorable mark; unsuitable for a junior profile that needs context |
| [peterthehan](https://github.com/peterthehan/peterthehan) | Link-centered introduction | Immediate onward paths without a long tech inventory |
| [M0nica](https://github.com/M0nica/M0nica) | Personal voice, header, contact | Human identity creates recognition; keep it professional |
| [benjaminsampica](https://github.com/benjaminsampica/benjaminsampica) | Game-inspired headings and choice links | Shows personality; gaming metaphor does not fit this audience |
| [gautamkrishnar](https://github.com/gautamkrishnar/gautamkrishnar) | Long, richly dynamic profile | Automation can convey activity but creates reading and maintenance load |
| [roaldnefs](https://github.com/roaldnefs/roaldnefs) | Concise professional description, few extras | Strong information density with low upkeep |
| [filiptronicek](https://github.com/filiptronicek/filiptronicek) | Skills overview, disclosure/details | Progressive disclosure is useful for secondary content |
| [halfrost](https://github.com/halfrost/halfrost) | Technical specialization and numerous icons | A clear technical specialty matters more than icons |
| [KiSobral](https://github.com/KiSobral/KiSobral) | Personal intro and stats | Brief introduction works; stats are optional |
| [dayyass](https://github.com/dayyass/dayyass) | Skills, experience, education, projects | Familiar hiring sequence; avoid empty or unverified claims |
| [simonw](https://github.com/simonw/simonw) | Current projects, recent releases, blog and TIL | Highly useful project-centered updates, when maintained |
| [codestackr](https://github.com/codestackr/codestackr) | Extensive social, media and technology visuals | Appropriate for creator audiences, too noisy for backend-first positioning |
| [mokkapps](https://github.com/mokkapps/mokkapps) | Portfolio-oriented banner and compact links | Short portfolio path; banner should not obscure proof |
| [MartinHeinz](https://github.com/MartinHeinz/MartinHeinz) | Badges, blog, technology and stats | Clear topical grouping, but badge proliferation raises visual noise |
| [saadeghi](https://github.com/saadeghi/saadeghi) | Almost entirely image-led | Powerful with established work; poor for explaining junior competencies |
| [WaylonWalker](https://github.com/WaylonWalker/WaylonWalker) | Customized graphics and dynamic sections | Visual identity is possible; maintenance cost matters |
| [DenverCoder1](https://github.com/DenverCoder1/DenverCoder1) | Very extensive badges, images and widgets | Technical showcase, but not the right information hierarchy for this profile |

Curated discovery source: [Awesome GitHub Profile Gallery](https://github.com/nitr0yukkuri/awesome-github-profile-gallery).

## Verified constraints and design rules

- GitHub renders a README from a **public repository named after the account**, with a nonempty root `README.md`: [GitHub Docs](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme).
- `<picture>` with `prefers-color-scheme` is documented for responsive theme-aware README images: [GitHub Docs](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github).
- GitHub recommends a concise bio, selected projects, and practical documentation for employers: [GitHub Docs](https://docs.github.com/en/account-and-profile/tutorials/using-your-github-profile-to-enhance-your-resume).
- Do not depend on custom JavaScript, externally hosted counters, or inline application behavior inside a README. Keep graphics local, static and text-independent.
- Make important content plain selectable Markdown; the header SVG is decorative, not a substitute for text.

## Starting audit: key findings

1. Repeated bold icon badges carry less useful information than explicit project architecture and status.
2. The current README spends space on generated statistics and a contribution snake. Two scheduled workflows regenerate these outputs daily.
3. The old PersonalDev section describes an active product in a way that no longer reflects the archived public repository. It should not be highlighted as an active product.
4. The Supermarket API and AI Finance Assistant have substantive public READMEs and concrete engineering scope; these are the two clearest front-page cases.
5. Some recent work is private. The new public README does **not** name or imply public availability for private repositories.
6. Existing portfolio pins include an archived repository and learning exercises. Suggested curation is a separate manual account-level action, not performed by this PR.
7. The visible account bio is Portuguese and backend-focused; an updated international-friendly bio is recommended below, but changing the account bio is outside the repository.

## Three design concepts

| Option | Benefit | Trade-off | Decision |
| --- | --- | --- | --- |
| **A · Engineering Minimalism** | Fast, reliable, minimal upkeep | Risks looking indistinct | Adopt structure |
| **B · Editorial Technology** | Clear sections, editorial rhythm, credible project focus | Needs careful graphic restraint | **Selected core** |
| **C · Computational Identity** | Expresses music/engineering crossover | Motifs can become abstract noise | Use as subtle accent only |

**Chosen solution:** restrained editorial engineering. No badges, no counters, no snake in the visible README. A simple geometric/music-signal banner in two static SVGs, dark/light mode variants, and most important content rendered as text. The banner is not a musical score or a claim about signal processing performance.

**Color tokens:** dark #101928 / blue #7CA8FF / warm #FFC18D; light #F4F7FB / blue #2458AC / warm #AF5F25. Geometry and text remain intelligible without gradients, external fonts, animation, or JS.

## Content architecture

1. Theme-adaptive abstract banner.
2. Name and immediate backend positioning in Portuguese, with an English language link.
3. Location, education and opportunity direction.
4. Direct links to projects, LinkedIn, email, English version.
5. Two substantial public project cases, with problem, implementation focus and limitations.
6. A collapsed section for small foundational public projects.
7. Skills organized by engineering domain instead of badge brand.
8. Short explanation of music training as an interdisciplinary differentiator.
9. Simple contact path.

Project statements are restricted to what their public READMEs support; product roadmap items remain identified as incomplete.

## Quality assessment — qualitative, not objective scores

| Dimension | Baseline / 10 | Proposed / 10 | Rationale |
| --- | ---: | ---: | --- |
| Initial positioning | 6 | 9 | Immediate target role and value |
| Technical evidence | 7 | 9 | Work descriptions lead with verifiable engineering |
| Differentiation | 4 | 8 | Subtle authorial visual and music context |
| Visual restraint | 4 | 9 | Replaces dense badges with compact signal graphic |
| International access | 4 | 9 | Portuguese default with a complete English counterpart |
| Accessibility design | 6 | 8 | Text-first content, alt text, high contrast variants |
| Maintenance simplicity | 4 | 9 | No dynamic widgets in the rendered profile |
| Honest project status | 5 | 9 | Removes outdated active state and flags limitations |

These are design heuristics based on source inspection and structural intent, **not validated user outcomes**. They should be reassessed after reviewing the rendered PR, especially on mobile.

## Manual account-level follow-up

The connected repository API can create file changes and PRs, but does not expose a supported action for account bio or pinned repository selection in this workflow.

Suggested bio (edit at GitHub profile settings):

> Backend developer | Java & Spring Boot · APIs, testing & automation | CS undergraduate · Brazil | Open to internships and junior roles

Suggested pins: Supermarket Management API, AI Finance Assistant, then selected active public projects as they mature. Remove the archived PersonalDev pin if present. Keep exercises visible in the repository list rather than positioning them as flagship applications.

## Validation checklist

- [x] No third-party images or statistics referenced by the new main README.
- [x] Both header variants exist in the branch.
- [x] Portuguese main README and English companion README exist in the branch.
- [x] No private project names or private repository links are published in the new README.
- [x] Planned functionality in the showcased projects is described as planned.
- [ ] Visual GitHub UI review on desktop + mobile (requires rendered inspection).
- [ ] Browser contrast inspection after GitHub image proxy rendering.
- [ ] Recruiting outcomes or user testing (not measured).

The original `profile/*.svg` assets are deliberately retained for rollback. The two previously scheduled decorative workflows may be switched to manual-only to avoid regenerating unused content; this is a reviewable change in the PR.

## Language decision — updated after author feedback

The main `README.md` is **Portuguese** to serve local recruiters and represent the author's preferred presentation language. A complete English counterpart is available at [`README.en.md`](../README.en.md) and linked near the introduction. The English language remains fully supported without being the default. This supersedes the earlier English-first proposal in the original mission.


---

## Mission 2.0 — Signal Cartography (17 November 2026)

**Scope:** visual evolution of the public profile README only. All repository visibility and account-level settings remain unchanged. This section supersedes the earlier *static-only* aesthetic preference, while retaining the text-first, evidence-based principles.

### Decision: editorial minimalism vs. visual signal cartography

| Alternative | Strength | Cost | Decision |
| --- | --- | --- | --- |
| Restrained editorial minimalism (previous baseline) | Low visual noise, predictable rendering, small assets | Limited memorability | Keep content architecture |
| Signal cartography (selected) | Distinctive identity linking geometry, systems and musical rhythm; bespoke project diagrams | Six local assets and minor CSS motion compatibility risk | **Adopt** |

The result uses an editorial masthead and two project-specific vector schematics. Headings, links, project evidence and limitations remain in ordinary Markdown outside all images.

### Implementation overview

- `assets/signal-cartography-{dark,light}.svg`: a custom 1200 × 320 editorial banner using a geometric grid, a stylized waveform/network motif and accessible color variants.
- `assets/case-systems-{dark,light}.svg`: visual abstraction of domain-oriented modules.
- `assets/case-ai-{dark,light}.svg`: visual abstraction of the voice → AI → tool calling → service boundary.
- `README.md` and `README.en.md`: parallel content, project-level evidence, clear scope limitations and links to verifiable public repositories.
- Existing decorative output, legacy SVGs and disabled scheduled workflows remain untouched for rollback; no external profile widgets added.

SVG motion is intentionally **nonessential**. Two CSS effects are scoped to `prefers-reduced-motion: no-preference`; the base paths remain visible without CSS. Rendering of those animations through GitHub's image handling **has not been visually verified**. The fallback is the complete static artwork, not an empty frame.

### Public project selection

The two current project showcases remain `supermarket-management-api` and `assistente-financeiro`, with explicit development scope and bootcamp attribution. Secondary public items are `simulador-emprestimo-java`, `UDF-Projetos` and `exercism`. Archived and forked repositories are intentionally not featured as original flagship products.

**Initial 2.0 scope (superseded for project-name disclosure by Mission 2.1 below):** private repositories were assessed only for portfolio potential, without identifying private projects in the README at that point. No repository was made public, and no team-owned code or account pins were modified.

Future publication requires an explicit authorization step and a separate assessment of credentials, historical commits, third-party copyrights, personal data, licenses and team ownership. A single clean current working tree is not sufficient evidence of safe historical publication.

### Research and tooling decision

References consulted:

- [GitHub Docs — Profile README](https://docs.github.com/en/account-and-profile/concepts/personal-profile)
- [GitHub Docs — Theme-specific images](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
- [GitHub Docs — Pinning items](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/pinning-items-to-your-profile)
- [Anthropic frontend-design guidance](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md)
- [UI/UX Pro Max skill guidance](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)
- [Vercel web-design-guidelines skill](https://github.com/vercel-labs/agent-skills/blob/main/skills/web-design-guidelines/SKILL.md)
- [SVG animation cookbook (community reference)](https://github.com/WaterTian/svg-motion-cookbook)

The three design skills were **consulted as research**, not installed or executed. In particular, browser UI and React-specific patterns were not copied into a GitHub README. No npm packages, external font servers or new GitHub Action dependencies were needed. This reduces supply-chain exposure and maintenance overhead.

### Validation evidence and limitations

On the branch:

- Both language READMEs were fetched back after writing; each contains three matching theme-aware images, a reachable local image path for all six SVG variants, and explicit project links.
- All six SVGs were fetched back; lightweight tag-nesting and entity checks found no mismatches. A denylist check found no scripts, event handlers or external image references.
- Text foreground/background ratios calculated from declared design tokens were: **16.71:1** (dark main), **14.34:1** (light main), **9.14:1** (dark muted) and **5.18:1** (light muted). These are token-level checks, not a pixel-accurate accessibility audit.
- **Initial 2.0 check (superseded in Mission 2.1 below):** neither profile README named the then-private experiments. The explicitly excluded project remains absent from both language versions.
- No build pipeline or hosted animation has been benchmarked. Actual GitHub-rendered appearance, keyboard/screen-reader behavior and animation through the image proxy **still require browser inspection**.
- No claim of a recruiter usability test or hiring impact has been made.

### Manual account-level follow-up

Review the new profile visually in both GitHub themes and on mobile **before merging**. For pinned projects, prioritize the two documented public showcase repositories; other candidates should be chosen only after inspecting their maturity. Pinned items, profile bio and private repository visibility remain account-level decisions outside this PR.

If visual motion does not survive GitHub's image handling, retain the static SVGs or choose a separately reviewed GIF asset without compromising reduced-motion needs.


---

## Mission 2.1 — Portfolio positioning: software, AI, automation and transparent authorship (17 November 2026)

### Requirement update from the author

The author clarified that **FluteOMR**, **Kelwin Hub** and **Aurora** were primarily experiments to test their skills working with AI in software development and automation. Their implementations were produced with substantial model assistance, rather than serving as evidence of manual authorship of every function or exhaustive hands-on validation.

This explicitly supersedes the earlier preference not to name private projects in the profile README. Mentioning their names and conceptual scope is now authorized **for the profile narrative only**. It does **not** authorize making source repositories public, exposing private files, adding inaccessible GitHub repository links, or changing pinned repositories.

### New content architecture

1. Lead with **software development · AI-assisted engineering · automation · MusicTech**, without claiming advanced professional seniority.
2. Preserve the two publicly inspectable engineering showcases as the highest-priority code links.
3. Add a dedicated **AI development experiments** section: three short, real, distinct experiment narratives.
4. Distinguish model-generated implementation from requirements, guidance, experimentation and actual manual validation; avoid false attribution of manual code authorship.
5. Mark all three source repositories as **currently private** and do not link to pages inaccessible to visitors.
6. Distinguish programmatic checks from personal/real-world homologation. Treat unfinished prototypes as legitimate research showcases, not as commercial releases.
7. Retain the flute background to explain the MusicTech research direction.
8. Maintain PT-BR and English semantic parity and working local light/dark image paths.

### Experiment status checked against repository READMEs

| Experiment | Framing | Reported implementation scope | Unresolved validation |
| --- | --- | --- | --- |
| FluteOMR | AI-assisted research in optical music recognition | Python image geometry and controlled MusicXML export experiments | Reliable general transcription and independent human validation remain incomplete |
| Kelwin Hub | AI-assisted local-first application and automation experiment | FastAPI/SQLite modules for tasks, contacts, projects, alerts, backup | No personally homologated general release, no production third-party messaging |
| Aurora | AI-assisted academic email/calendar workflow prototype | TypeScript, installable PWA, provider integration code, simulated tests | Real OAuth, hosting and push delivery still require end-to-end validation |

README text avoids misleading clickable links to private repositories. The three project names are included solely as **descriptions of the user's own experiments**. The explicitly excluded project remains absent from public-facing materials.

### Visual adjustments

- Both existing hero SVGs now explicitly reference **AI** and **automation** in the editorial tagline.
- A theme-aware, version-controlled **conceptual workflow schematic** (`assets/case-ai-lab-{dark,light}.svg`) presents the experiment loop, without claiming that every phase has already received personal human validation.
- No external widget, npm dependency, hosted image service, GitHub Action, or new deployment process was introduced.

### Validation boundary

The verification performed during this mission must not be described as equivalent to executing full source-project tests, auditing all old Git histories, viewing the GitHub-rendered interface in an actual browser, or approving a change of repository visibility. Publication of the three private repositories is a **separate** operation with its own security and licensing decision.

Profile updates remain on the same draft PR; `main` and private repository visibility remain unchanged.
