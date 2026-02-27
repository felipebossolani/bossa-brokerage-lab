Bossa — Prompt 2: Três Telas (Home + Investimentos + Movimentações)
<requirements>
## 1. Overall Style & Visual Language
This is a premium Brazilian investment brokerage mobile app called "Bossa". 
The visual identity blends **Bossa Nova cultural warmth** with **modern wealth management aesthetics** inspired by Wealthfront's clean, confident design language.

Core characteristics:
- Deep indigo/navy foundation evoking sophistication and nighttime Rio elegance
- Electric blue primary accent conveying trust and technology
- Warm secondary accent (soft gold or terracotta) as a subtle Bossa Nova signature
- Clean, spacious, confident typography
- Card-based layout with generous whitespace
- No borders — separation through elevation, subtle shadows, and tonal contrast

Target perception:
- Trustworthy and institutional-grade
- Digitally native, not legacy finance
- Brazilian identity without cliché — sophisticated, not tropical
- Designed for a digitally savvy audience investing in Tesouro Direto, Renda Fixa, and Fundos

---

## 2. Device & Layout

- Device: iPhone 15 (393 × 852 px)
- Show 3 screens side by side with realistic device frames (rounded corners, dynamic island)
- Screens from left to right: **Home** → **Investimentos** → **Movimentações**
- Each screen shares the same bottom navigation bar with the corresponding tab active
- Small gap (24-40px) between devices
- Background behind phones: dark gradient or solid (#080C18) for presentation context
- Status bar: system default (time, signal, battery) in white on each screen

---

## 3. Bottom Navigation Bar (shared across all 3 screens)
- Height: ~84px (including safe area)
- Background: deep indigo, slightly darker than main bg
- 3 tabs with icons + labels:
  1. **Home** (house icon)
  2. **Investimentos** (bar chart / trending up icon)
  3. **Movimentações** (list/receipt icon)
- Active state: electric blue filled icon + electric blue label
- Inactive: outline icon + muted gray label
- No top border — separation via shadow or tonal shift

---

## 4. Screen 1 — Home (left phone, Home tab active)

### Header
- Top-left: "Bossa" logotype — refined sans-serif, lowercase or mixed-case
  - Subtle musical note flourish on the "o" — minimal, elegant, not cartoonish
  - White color
- Top-right: notification bell (outline, muted) + red dot
- Below logo: "Bom dia, Felipe" in secondary text

### Total Balance Hero Card
- Full-width card, 16px horizontal margins
- Subtle gradient or glassmorphism background
- Content:
  - "Patrimônio total" (caption, muted)
  - "R$ 284.520,37" (30px, bold, white)
  - Eye toggle icon
  - "▲ 1,24% este mês" (success green)
- Faint decorative wavy line pattern at 5-8% opacity (Bossa Nova musical wave motif)

### Quick Actions
- Row of 3 circular buttons: "Investir" | "Resgatar" | "Pix"
- Outlined icons, electric blue, caption labels below

### Portfolio Cards (horizontal scroll)
- 3 cards peeking:
  - Tesouro Direto: R$ 142.300,00 / +12,4% (12m)
  - Renda Fixa: R$ 89.220,37 / +9,8% (12m)
  - Fundos: R$ 53.000,00 / +6,2% (12m)
- Card surface color, rounded, no border, subtle shadow

### Recent Transactions (3 items)
- "Movimentações recentes" + "Ver tudo" link
- Compact rows with icon, title, date, amount

---

## 5. Screen 2 — Investimentos (center phone, Investimentos tab active)

### Header
- Title: "Investimentos" (h1, 24px, bold, white)
- Top-right: filter icon (outline, muted)

### Portfolio Summary Card
- Full-width hero card
- "Total investido" (caption)
- "R$ 284.520,37" (large, bold)
- Below: mini donut chart or horizontal stacked bar showing allocation:
  - Tesouro Direto: 50% (electric blue)
  - Renda Fixa: 31% (lighter blue / cyan)
  - Fundos: 19% (terracotta/warm accent)
- Legend below the chart with percentages

### Investment Category Cards (vertical list)
Three expandable cards, stacked vertically:

**Tesouro Direto**
- Icon: shield outline
- Title + total value: "R$ 142.300,00"
- Subtitle: "3 títulos ativos"
- Right: chevron
- Sub-items visible:
  - Tesouro Selic 2029 — R$ 80.000 — +13,2%
  - Tesouro IPCA+ 2035 — R$ 42.300 — +11,8%
  - Tesouro Prefixado 2027 — R$ 20.000 — +9,4%

**Renda Fixa**
- Icon: lock outline
- Title + total: "R$ 89.220,37"
- Subtitle: "2 posições"
- Collapsed state (show chevron only)

**Fundos**
- Icon: layers/pie outline
- Title + total: "R$ 53.000,00"
- Subtitle: "2 fundos"
- Collapsed state

### Card style
- Each category card: surface color, 14-16px radius
- Sub-items: slightly indented, smaller text, dividers between
- Performance values: success green for positive

---

## 6. Screen 3 — Movimentações (right phone, Movimentações tab active)

### Header
- Title: "Movimentações" (h1, 24px, bold, white)
- Top-right: search icon (outline, muted)

### Filter Chips Row
- Horizontal scrollable chips: "Todas" (active/filled) | "Entradas" | "Saídas" | "Tesouro" | "Renda Fixa" | "Fundos"
- Active chip: electric blue background, white text
- Inactive: surface elevated background, secondary text

### Monthly Section
- Section header: "Fevereiro 2026" (caption, muted, left-aligned)
- Transaction list:

| Date   | Description                     | Amount           |
|--------|---------------------------------|------------------|
| 22 fev | Aplicação Tesouro Selic 2029    | - R$ 5.000,00    |
| 20 fev | Resgate CDB Banco X             | + R$ 12.340,00 ✓ |
| 18 fev | Aplicação Fundo Multi XYZ       | - R$ 3.000,00    |
| 15 fev | Juros CDB 120% CDI              | + R$ 890,22 ✓    |
| 10 fev | Aplicação Tesouro IPCA+ 2035    | - R$ 10.000,00   |
| 05 fev | Cupom Tesouro IPCA+ 2035        | + R$ 1.245,00 ✓  |

- Each row: type icon (arrow up for income/green, arrow down for expense/neutral) + description + date below + amount right-aligned
- Positive amounts: success green
- Negative amounts: white (neutral, it's an investment not a loss)
- Row height: ~68px
- Subtle 1px dividers

### Previous Month Peek
- "Janeiro 2026" section header visible with 1-2 rows partially showing to indicate scroll continuity

---

## 7. Color Palette

| Token              | Value     | Usage                          |
|--------------------|-----------|---------------------------------|
| background         | #0C1222   | Main app background             |
| surfaceCard        | #141C2E   | Card backgrounds                |
| surfaceElevated    | #1A2540   | Elevated elements, chips, inputs|
| primaryAccent      | #4A7CFF   | Electric blue — CTAs, active    |
| secondaryAccent    | #D4956A   | Warm terracotta — chart, detail |
| tertiaryAccent     | #6BC5E8   | Lighter blue/cyan — charts      |
| textPrimary        | #FFFFFF   | Headings, values                |
| textSecondary      | #8B95A8   | Labels, captions                |
| textMuted          | #4A5568   | Disabled, hints                 |
| success            | #34D399   | Positive returns, income        |
| danger             | #F87171   | Negative, losses                |
| chipActive         | #4A7CFF   | Active filter chip bg           |
| chipInactive       | #1A2540   | Inactive filter chip bg         |
| bottomNavBg        | #0A0F1C   | Bottom bar background           |

---

## 8. Typography
- Font: SF Pro Display / SF Pro Text (system iOS)
- Screen titles: 24px, weight 700
- Balance value: 30px, weight 700
- Section titles: 17px, weight 600
- Card values: 18px, weight 600
- Body/labels: 14px, weight 400
- Captions: 12px, weight 400
- Numeric values: tabular figures

---

## 9. Design Details
- All corners: 14-16px radius on cards, 999px on chips and action buttons
- Shadows: subtle, cool-toned (rgba blue-black)
- No hard borders anywhere
- Bossa Nova motif: faint wavy sine-wave lines as background texture in hero cards only (5-8% opacity)
- Overall density: comfortable, premium — wealth management, not trading terminal
- Presentation layout (3 phones): slight perspective or straight-on, consistent lighting, professional mockup quality

</requirements>