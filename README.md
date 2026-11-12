# WIMB — Where Is My Break?

**A personalised after-work recovery app.**
UX/UI capstone project · neue fische Bootcamp · 2026
by Dženeta Bratić, Léia Coelho and Maria Brand

**▶ Try the live prototype: [coelhoxs.github.io/wimb](https://coelhoxs.github.io/wimb/)** (best on a phone, or in your browser’s phone view)

![WIMB app screens: Home, Your Break is ready, Break Journal](WIMB-presentation-mockup.png)

---

## The problem

Many busy people come home from work physically tired, mentally overwhelmed, or both. They want to rest, but they don't know what would help, and choosing and preparing an activity feels like one more task.

Wellness apps exist, but they offer large content libraries. More choice often means more effort, which is exactly what a drained person doesn't have.

> **Recovery should not feel like another task.**

## The solution

WIMB asks two questions and gives one answer:

**How do you feel?** → **How much time do you have?** → **Your Break is ready.**

There is no library to browse and no plan to make. The user presses **Start** and follows one short, personalised ritual. For example, a mentally overwhelmed user with 15 minutes might get breathing, gentle stretching, calming audio and a warm drink prompt.

Optional physical products, such as tea, an eye mask or bath salts, can support the ritual and make it easier to repeat at home.

## Research

We ran a survey with **26 busy city residents** (August 18–20, 2026), backed by desk research on existing wellness apps.

| Finding | Result |
| --- | --- |
| Feel drained at least a few times a week | **88%** (23 of 26) |
| Have tried a wellness, meditation, sleep or fitness app | **65%** |
| Use one regularly | **19%** |

**Key insights**

- **Exhaustion is recurring, not occasional.** WIMB is designed for a daily after-work moment, not a rare crisis.
- **The mind comes first, but the body matters too.** A busy, overstimulated mind was the largest single need, and mixed physical and mental fatigue was almost as common.
- **Existing apps get tried but not kept.** People said those apps felt like another task, they forgot to use them, or there was too much choice.

**Product direction:** one personalised, low-effort break based on mood and available time, not a large content library.

📊 Full report: [`survey-analysis-report/`](survey-analysis-report/)

## Key features

- **Weekly insight.** A small card on Home with Wimble, the mascot, showing how many breaks you took and what helped most.
- **Onboarding.** A short welcome, account setup, three questions and location, so the app knows the user from the start.
- **Find my Break.** Starts right on Home: pick how you feel (Busy mind, Low energy, Need to move), then how much time you have, and get one ready-to-start activity.
- **Quick Activities.** One-tap shortcuts ordered by time: Breathe (5 min), Exercise (10 min) and Tea (15 min).
- **Break Journal.** Moments to remember, shown as Gallery, Calendar and Favorite views.
- **Profile.** History, a list of activities and personal preferences.

![WIMB profile screen](WIMB-profile-mockup.png)

## Design system

UI foundation decisions by Léia Coelho.

Calm, organic and atmospheric: dark turquoise backgrounds, soft purple and orange light, and liquid-glass surfaces. Readability always comes before effects.

**Typography**
- **Lora** for headlines, headings and card titles
- **DM Sans** for body text, buttons, labels and navigation

**Colour**

| Palette | Key shade | Role |
| --- | --- | --- |
| Turquoise | `#0D2024` – `#488590` | Atmospheric background |
| Orange | `#F89F8F` · `#F6795A` · `#E35C2E` | Liquid-glass primary actions, active navigation |
| Purple | `#9754FF` | Selected surfaces and accent light |
| Gray | `#181818` – `#F9F9F9` | Neutrals |

**Layout:** 26px screen padding · 20px gutter · 70px top and 35px bottom safe areas · 50px main action height.

Full specification: [`DESIGN.md`](DESIGN.md)

## Process

1. **Concept & Milestone II.** Problem definition, hypothesis and research plan ([deck](After-Work-Reset_Milestone-II.pptx)). The project started under the working title *After-Work Reset*.
2. **Research.** Survey and competitor desk research.
3. **Wireframes.** Low-fidelity user flow ([`wireframe-english.svg`](wireframe-english.svg)).
4. **UI design.** High-fidelity screens and design system in Figma.
5. **Prototype.** A functional HTML prototype built from the approved Figma design.
6. **QA.** Layout and interaction checks against the design ([`design-qa.md`](design-qa.md)).

## Run the prototype

The easiest way is the live link: **https://coelhoxs.github.io/wimb/**. To run it locally instead:


Requires [Node.js](https://nodejs.org/).

```bash
git clone https://github.com/dzenirose-jpg/WIMB.git
cd WIMB
node serve.cjs
```

Then open **http://127.0.0.1:5173** in your browser. The prototype is designed for a mobile viewport (402 × 874), so use your browser's device mode for the best view.

## Repository

| Path | Contents |
| --- | --- |
| `index.html` | The functional prototype |
| `serve.cjs` | Local preview server |
| `assets/` | Icons, mascot illustrations and images |
| `DESIGN.md` | Approved design system |
| `survey-analysis-report/` | Survey analysis |
| `After-Work-Reset_Milestone-II.pptx` | Milestone II presentation |
| `wireframe-english.svg`, `wire/` | Wireframes |

## Team

- Dženeta Bratić
- Léia Coelho — UI foundation (typography, colour, layout and visual language)
- Maria Brand

---

*WIMB is a capstone project from the neue fische UX/UI Design Bootcamp (category: mobile app design, industry: wellness). It is a prototype and not a released product.*
