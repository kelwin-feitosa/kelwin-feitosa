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
