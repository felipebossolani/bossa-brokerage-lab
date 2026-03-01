# Bossa Landing Page — Prompt Workflow

Um guia passo a passo para gerar a landing page da Bossa usando Gemini Nanobanana 2, seguindo um workflow de design system first.

---

## Passo 1: Definir o design system

Antes de gerar qualquer imagem, alimente o modelo com o sistema de design completo. Isso ancora todas as decisões visuais e evita output genérico.

```
<design_system>
Brand: Bossa — Brazilian investment brokerage
Visual identity: Bossa Nova cultural warmth meets modern wealth management

Color tokens:
--bg-deep: #0C1222 (main background, deep indigo)
--bg-surface: #141C2E (card and section backgrounds)
--bg-elevated: #1A2540 (elevated elements, inputs, hover states)
--accent-blue: #4A7CFF (primary accent, electric blue, CTAs)
--accent-warm: #D4956A (secondary accent, terracotta, warm details)
--accent-cyan: #6BC5E8 (tertiary, charts and data viz)
--text-primary: #FFFFFF
--text-secondary: #8B95A8
--text-muted: #4A5568
--success: #34D399
--danger: #F87171

Typography:
- Headlines: SF Pro Display or Inter, weight 700, letter-spacing -1.5px
- Subheadlines: Inter, weight 500, 20-24px
- Body: Inter, weight 400, 16-18px
- Captions and labels: Inter, weight 400, 13-14px
- Numeric/financial data: tabular figures, weight 600

Radius: 16px cards, 12px buttons, 999px pills
Shadows: cool-toned, rgba(12, 18, 34, 0.6)
Borders: none, separation via elevation and tonal contrast only

Motif: abstract sound waves (Bossa Nova reference), used as subtle background texture at 5-10% opacity. Smooth sine curves, not aggressive. Musical, elegant.

Overall: dark mode only, premium, institutional-grade, no flat generic fintech look. Awwwards-level craft. Clean whitespace. Confident, not flashy.
</design_system>
```

---

## Passo 2: Gerar assets custom com Nanobanana

### 2a. Hero background

Gere o background do hero section separadamente para ter controle total sobre a qualidade.

```
Abstract dark background for a premium fintech landing page hero section.

Deep indigo base color (#0C1222). Smooth, flowing sine wave lines in electric blue (#4A7CFF) and subtle terracotta (#D4956A) at low opacity (10-15%), layered across the composition. The waves reference Bossa Nova music — elegant, rhythmic, organic curves. Not aggressive, not geometric. Think jazz album cover meets wealth management.

Additional details:
- Very subtle particle dots scattered sparsely, like distant stars, in muted blue-gray
- Slight gradient from darker at top to slightly lighter indigo at bottom center, creating a natural focal point for text placement
- No text, no UI elements, no icons — pure atmospheric background
- High resolution, 2560x1440px, PNG
- The overall mood is nighttime sophistication, calm confidence, quiet luxury
```

### 2b. Ilustrações de produto (opcional, gerar se quiser enriquecer a seção de produtos)

```
Set of 3 minimal, premium fintech icons on transparent background. Dark theme style.

Icon 1: A shield with a subtle upward arrow inside, representing government bonds (Tesouro Direto). Electric blue (#4A7CFF) with soft glow.

Icon 2: A lock combined with a bar chart, representing fixed income (Renda Fixa). Electric blue with terracotta (#D4956A) accent detail.

Icon 3: Overlapping circular layers, representing investment funds (Fundos). Gradient from electric blue to cyan (#6BC5E8).

Style: outline with subtle inner glow, not flat, not skeuomorphic. Thin strokes (2px). Consistent 120x120px size. Premium, minimal, cohesive. Dark background (#0C1222) if not transparent.
```

---

## Passo 3: Gerar a landing page completa

Este é o prompt principal. Estruturado como storyboard, seção por seção.

```
<requirements>
## 1. Overall Context
A premium landing page for "Bossa", a fictional Brazilian investment brokerage. Desktop layout, full-page screenshot, dark theme. The visual identity blends Bossa Nova elegance with modern wealth management design.

This is a single, continuous full-page design showing all sections from top to bottom in one image. Aspect ratio approximately 3:4 or taller to accommodate all sections.

Apply the following design system throughout:
- Background: #0C1222 (deep indigo)
- Surface: #141C2E
- Primary accent: #4A7CFF (electric blue)
- Secondary accent: #D4956A (terracotta)
- Text: #FFFFFF primary, #8B95A8 secondary, #4A5568 muted
- Typography: Inter or SF Pro, clean sans-serif
- No borders anywhere. Separation through color, elevation, and spacing only.
- Generous whitespace. Premium density. Not cramped.

---

## 2. Navbar
- Fixed to top, full width, max-width 1280px centered
- Background: transparent over hero, no border
- Left: "Bossa" logotype, white, refined sans-serif. Subtle musical note detail on the "o"
- Center: navigation links in secondary text color — "Produtos", "Sobre", "Seguranca", "Blog"
- Right: two buttons
  - "Entrar" — text only, white, no background
  - "Abra sua conta" — pill button, electric blue (#4A7CFF) background, dark text, rounded 999px
- Typography: 15px, weight 500

---

## 3. Hero Section
- Full viewport height feel, generous vertical padding (160px top, 120px bottom)
- Background: deep indigo with abstract flowing sine wave lines in electric blue and terracotta at very low opacity (8-12%). The waves are smooth, organic, musical. Bossa Nova motif. Subtle particle dots like distant stars.

- Content centered, max-width 800px:
  - Headline (two lines):
    Line 1: "Invista com clareza."
    Line 2: "Cresça com confiança."
    Style: 64-72px, weight 700, white, letter-spacing -1.5px, line-height 1.1
  - Subtitle below:
    "Tesouro Direto, Renda Fixa e Fundos em uma plataforma pensada para quem leva investimento a sério."
    Style: 20px, weight 400, secondary text color (#8B95A8), max-width 600px, centered
  - CTA row below subtitle (24px gap):
    - Primary: "Comece agora" — electric blue pill button, dark text
    - Secondary: "Conheça os produtos" — transparent, white text, subtle white border (1px, 20% opacity)
  - Below CTAs, small trust line:
    "Sem taxas escondidas. Sem pegadinhas. Seus investimentos, seu controle."
    Style: 13px, muted text, centered

---

## 4. Social Proof / Numbers Section
- Background: same deep indigo, separated from hero by generous spacing (100px+)
- Centered row of 4 metrics, evenly spaced, max-width 1080px:

  Metric 1:
  - Value: "R$ 2,4 bi"
  - Label: "sob custódia"

  Metric 2:
  - Value: "142 mil"
  - Label: "investidores ativos"

  Metric 3:
  - Value: "4.9"
  - Label: "nota na App Store"

  Metric 4:
  - Value: "0"
  - Label: "taxas de custódia"

- Values: 40-48px, weight 700, white
- Labels: 14px, weight 400, secondary text color
- No cards, no boxes. Just the numbers floating cleanly on the background.
- Subtle horizontal divider line above this section (1px, #1A2540)

---

## 5. Products Section
- Background: slightly lighter surface (#141C2E) to create visual separation
- Padding: 100px vertical
- Section header centered:
  - Overline: "PRODUTOS" (12px, weight 600, electric blue, letter-spacing 3px)
  - Title: "Tudo que você precisa em um só lugar" (36px, weight 700, white)
  - Subtitle: "Escolha entre as melhores opções de investimento do mercado brasileiro." (18px, secondary text, max-width 560px)

- Three product cards in a horizontal row, centered, gap 32px, max-width 1080px:

  **Card 1 — Tesouro Direto**
  - Icon: shield with upward arrow, electric blue outline with glow
  - Title: "Tesouro Direto" (20px, weight 600, white)
  - Description: "Títulos públicos com segurança do governo federal. Liquidez diária no Tesouro Selic." (15px, secondary text)
  - Bottom link: "Saiba mais →" in electric blue
  - Card: #1A2540 background, 16px radius, padding 32px, no border

  **Card 2 — Renda Fixa**
  - Icon: lock with bar chart, electric blue + terracotta detail
  - Title: "Renda Fixa"
  - Description: "CDBs, LCIs, LCAs e debêntures com as melhores taxas. Rentabilidade previsível."
  - Bottom link: "Saiba mais →"
  - Same card style

  **Card 3 — Fundos**
  - Icon: overlapping layers, blue to cyan gradient
  - Title: "Fundos de Investimento"
  - Description: "Multimercado, ações e renda fixa. Gestores renomados, acesso simplificado."
  - Bottom link: "Saiba mais →"
  - Same card style

- Cards have subtle hover state implied: slightly lighter background, faint blue top border glow

---

## 6. Footer
- Background: darker than main (#0A0F1C)
- Padding: 80px top, 40px bottom
- Max-width 1280px, centered
- Layout: 4 columns

  **Column 1 — Brand**
  - "Bossa" logotype (white, same as navbar)
  - Below: "Investimentos com clareza e confiança." (14px, muted text)

  **Column 2 — Produtos**
  - Header: "Produtos" (14px, weight 600, white)
  - Links: Tesouro Direto, Renda Fixa, Fundos (14px, secondary text)

  **Column 3 — Institucional**
  - Header: "Institucional" (14px, weight 600, white)
  - Links: Sobre, Carreiras, Blog, Imprensa (14px, secondary text)

  **Column 4 — Suporte**
  - Header: "Suporte" (14px, weight 600, white)
  - Links: Central de ajuda, Segurança, Termos de uso, Privacidade (14px, secondary text)

- Bottom bar: subtle 1px divider (#1A2540), then a single line:
  - Left: "2026 Bossa. Todos os direitos reservados." (12px, muted)
  - Right: "Este é um projeto fictício de caráter educacional." (12px, muted)

---

## 7. Anti-Generic Rules
- No flat design. No generic fintech template look.
- Pure dark mode. Rich depth through layered surfaces and subtle gradients.
- Premium, Awwwards-level visual quality.
- Subtle specular highlights on interactive elements (buttons, cards).
- The overall feeling is calm authority. Not startup energy. Not crypto hype. Wealth management confidence with Brazilian soul.
- Typography must feel intentional: tight letter-spacing on headlines, generous line-height on body text.
- The Bossa Nova wave motif should be present but never dominant. It whispers, it does not shout.

</requirements>
```

---

## Passo 4: Iterar

Depois do primeiro output:

1. Screenshot os pontos fracos
2. Re-prompt com ajustes específicos:

```
Keep the full design system and layout. Refine the following:
- [descreva o que precisa melhorar, ex: "hero waves need more depth and contrast", "product cards feel too flat, add subtle top-edge glow", "footer text hierarchy needs more contrast"]
- Maintain all typography, colors, and spacing from the original.
```

---

## Passo 5: Toques finais

Regras para o re-prompt de polimento:

```
Final polish pass. Keep everything. Enhance:
- Add subtle gradient overlay on hero (radial, center bottom, slightly lighter indigo fading to edges)
- Product card icons should have a faint ambient glow matching their color
- CTA buttons should have a soft box-shadow in accent color at 30% opacity
- Ensure all text is crisp and readable against backgrounds
- The overall composition should feel like a real product page, not an AI-generated mockup
```

---

## Notas

- Gere o hero background (passo 2a) separadamente e avalie antes de gerar a página completa
- O prompt da landing page (passo 3) é longo por design. O Nanobanana responde bem a specs detalhadas.
- Os valores de social proof são fictícios. Ajuste conforme necessário.
- Todo o projeto é educacional. A Bossa não existe.