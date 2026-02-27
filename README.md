*[Leia em Português](README-pt.md)*

# Bossa — UI Design Experiment with Structured Prompts

An experiment in generating high-fidelity mobile app interfaces using only structured prompts fed into image generation models. No design tools. No Figma. No manual pixel work.

The subject is a fictional Brazilian investment brokerage called **Bossa** — a name that nods to Bossa Nova's quiet sophistication and to a builder's attitude.

---

## What this is

This repository contains the prompts, outputs, and methodology behind an experiment: can you go from zero to a credible fintech mobile UI using only natural language and structured design tokens?

The goal is not to replace designers. It is to stress-test how far prompt engineering can push visual output quality in current image generation models, and to document the process honestly — what works, what breaks, and where human judgment remains irreplaceable.

---

## The brief

A mobile-first investment app for a digitally savvy Brazilian audience. Core products: Tesouro Direto, Renda Fixa, and Fundos. The visual identity blends Bossa Nova cultural warmth with modern wealth management aesthetics, drawing loose inspiration from Wealthfront's clean confidence without copying any specific player.

Key constraints:
- Dark theme, indigo-based palette
- Must not resemble XP, Nubank, BTG, Rico, or Inter's color language
- iPhone 15 frame (393 x 852px)
- Three screens: Home, Investimentos, Movimentacoes

---

## Repository structure

```
bossa-experiment/
  home-single-screen/
    prompt.md                       # Single screen prompt (Home)
    home-single-screen.png          # Generated output
  three-tabs-screens/
    prompt.md                       # Three screens side by side
    three-tabs-screens.png          # Generated output
  README.md
  README-pt.md
```

---

## Results

### Single Screen — Home

The home screen concentrates balance, portfolio allocation, and recent transactions in a single scrollable view.

[View prompt](home-single-screen/prompt.md)

![Home Single Screen](home-single-screen/home-single-screen.png)

### Three Tabs — Home, Investimentos, Movimentacoes

Three screens presented side by side, each with its corresponding active tab in the bottom navigation.

[View prompt](three-tabs-screens/prompt.md)

![Three Tabs Screens](three-tabs-screens/three-tabs-screens.png)

---

## Methodology

1. **Define the product context.** A fictional but plausible Brazilian brokerage, with real product categories and realistic data. The fiction needs to be specific enough that the model has no excuse to go generic.

2. **Build the prompt as a design spec.** Not a vague description — a structured document with layout hierarchy, component definitions, color tokens, typography scale, and spacing rules. The closer the prompt resembles what a developer would receive from a designer, the better the output.

3. **Establish a color palette with intent.** Every color choice was made to avoid direct association with existing Brazilian brokerages while maintaining fintech credibility. The palette was derived by cross-referencing competitors and deliberately steering away from their primary identifiers.

4. **Generate and evaluate.** Run the prompt through the model, assess the output against the spec, identify gaps, and refine. Each iteration is preserved for comparison.

5. **Document honestly.** The point is not to cherry-pick the best result. It is to show the full trajectory from prompt to output, including the failures.

---

## Model

Outputs were generated using **Google Gemini** (image generation capabilities). Prompts are model-agnostic in structure but were optimized for this specific model's interpretation of structured design requirements.

---

## Color palette rationale

| Token            | Hex       | Role                                    |
|------------------|-----------|-----------------------------------------|
| background       | #0C1222   | Deep indigo — nighttime sophistication  |
| surfaceCard      | #141C2E   | Card layer — subtle elevation           |
| primaryAccent    | #4A7CFF   | Electric blue — trust, technology       |
| secondaryAccent  | #D4956A   | Terracotta — warmth, Brazilian identity |
| success          | #34D399   | Mint green — positive returns           |
| danger           | #F87171   | Coral red — losses, alerts              |

Deliberately avoided: black/yellow (XP), purple (Nubank), dark blue/white (BTG), orange (Rico, Inter).

---

## What this is not

- This is not a product. Bossa does not exist.
- This is not a design system. The tokens are part of the prompt, not a maintained spec.
- This is not a claim that AI replaces design work. It is an observation of where the boundary sits today.

---

## Context

This experiment is part of a broader exploration into AI-assisted workflows for product and technology leaders. The focus is practical: what can you actually ship or prototype faster with these tools, and where do you still need human craft?

---

## Author

**Felipe Bossolani** — CPTO at Warren, ex-founder, 20+ years in fintech.

Writing about AI tools, product engineering, and the intersection of technology leadership with hands-on craft at [bossolani.com](https://bossolani.com) and [LinkedIn](https://www.linkedin.com/in/bossolani/).

---

## License

Prompts and methodology are open under MIT. Do whatever you want with them. If you run the experiment yourself and get interesting results, share them.