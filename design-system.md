# GuessLess Design System — SEO Audit Reports

Derivado do briefing de marca GuessLess: Growth Agency Fullstack para mercado de luxo.
Arquétipos: Governante (controle, estrutura) + Sábio (dados, clareza) + Mago (transformação).

---

## Princípios Visuais

1. **Sofisticação sem exagero** — Elegância vem da contenção, não do excesso
2. **Dados como protagonista** — Números e métricas devem ser o foco visual
3. **Hierarquia rigorosa** — Cada elemento tem um papel claro na composição
4. **Espaço é luxo** — Breathing room generoso entre seções
5. **Contraste intencional** — Apenas destaques estratégicos recebem cor

---

## Paleta de Cores

### Fundos (Dark Mode — Padrão)

| Token | Hex | Uso |
|-------|-----|-----|
| `--bg` | `#08080C` | Fundo principal da aplicação |
| `--surface` | `#0F0F15` | Sidebar, áreas elevadas |
| `--card` | `#16161F` | Cards, containers de conteúdo |
| `--card-hover` | `#1C1C28` | Hover state dos cards |
| `--border` | `#23232F` | Bordas sutis, separadores |
| `--border-accent` | `#2E2E3A` | Bordas em elementos interativos |

### Texto

| Token | Hex | Uso |
|-------|-----|-----|
| `--text` | `#F0EDE6` | Texto principal (off-white quente) |
| `--text-muted` | `#9A9488` | Texto secundário, descrições |
| `--text-dim` | `#5C5850` | Labels, captions, placeholders |

### Accent — Champagne/Ouro (Identidade GuessLess)

| Token | Hex | Uso |
|-------|-----|-----|
| `--accent` | `#C9A96E` | Accent primário — links, badges, destaques |
| `--accent-light` | `#D4B97E` | Hover do accent |
| `--accent-glow` | `rgba(201,169,110,.10)` | Background sutil para accent areas |
| `--accent-strong` | `#B8944F` | Accent em estados ativos |

### Semânticas (Status)

| Token | Hex | Background | Uso |
|-------|-----|------------|-----|
| `--green` | `#4ADE80` | `rgba(74,222,128,.08)` | Bom, aprovado, positivo |
| `--yellow` | `#FBBF24` | `rgba(251,191,36,.08)` | Atenção, warning |
| `--orange` | `#FB923C` | `rgba(251,146,60,.08)` | Problema, bad |
| `--red` | `#F87171` | `rgba(248,113,113,.08)` | Crítico, falha |
| `--blue` | `#93C5FD` | `rgba(147,197,253,.08)` | Informacional |
| `--cyan` | `#67E8F9` | `rgba(103,232,249,.08)` | Destaque neutro |

---

## Tipografia

### Font Stack

| Uso | Família | Weight | Fonte |
|-----|---------|--------|-------|
| **Headings (H1-H3)** | `'DM Serif Display', Georgia, serif` | 400 | Google Fonts |
| **Body / UI** | `'Inter', system-ui, sans-serif` | 300-700 | Google Fonts |
| **Monospace / Data** | `'JetBrains Mono', monospace` | 400-600 | Google Fonts |

### Escala Tipográfica

| Elemento | Tamanho | Weight | Tracking |
|----------|---------|--------|----------|
| H1 (Page title) | 32px | DM Serif 400 | -0.5px |
| H2 (Section) | 22px | DM Serif 400 | -0.3px |
| H3 (Subsection) | 16px | Inter 700 | 0 |
| Body | 13.5px | Inter 400 | 0 |
| Small / Caption | 12px | Inter 500 | 0 |
| Label (uppercase) | 10px | Inter 600 | 1.5px |
| Data / Number | 13px | JetBrains Mono 500 | 0 |

---

## Spacing

Base unit: 4px

| Token | Value | Uso |
|-------|-------|-----|
| `--space-xs` | 4px | Padding mínimo |
| `--space-sm` | 8px | Gap entre badges, ícones |
| `--space-md` | 16px | Padding interno de cards |
| `--space-lg` | 24px | Gap entre cards, seções menores |
| `--space-xl` | 32px | Padding de seções |
| `--space-2xl` | 48px | Separação entre seções principais |
| `--space-3xl` | 64px | Margin top de grandes seções |

---

## Border Radius

| Token | Value | Uso |
|-------|-------|-----|
| `--radius` | 12px | Cards, containers |
| `--radius-sm` | 6px | Badges, inputs, tags |
| `--radius-xs` | 4px | Inline elements |
| `--radius-full` | 9999px | Avatars, dots |

---

## Componentes

### Cards
- Background: `--card`
- Border: 1px solid `--border`
- Radius: `--radius`
- Padding: 24px
- Hover: border → `--accent`, bg → `--card-hover`
- Transição: 250ms ease

### Badges (Status)
- Padding: 3px 10px
- Radius: `--radius-full` (pill shape)
- Font: 11px, weight 600
- Background: variante semântica com 8% opacity
- Cor: variante semântica full

### Tables
- Background: `--card`
- Header: `--surface`, text uppercase 10px
- Rows: border-bottom 1px rgba(255,255,255,.03)
- Hover: `--card-hover`

### Section Headers
- Icon: 32x32px, radius `--radius-sm`
- Title: H2 (DM Serif Display)
- Separator line: 1px `--border`
- Margin: 48px top, 20px bottom

### Sidebar
- Width: 260px, fixed
- Background: `--surface`
- Logo: accent gradient icon + "GuessLess" branding
- Nav items: 13px Inter 500, `--text-muted`
- Active state: `--accent-glow` bg, `--accent` text

---

## Assinatura Visual GuessLess

- Logo text: "**Guess**Less" (bold no "Guess")
- Tagline nos reports: "Direção. Dados. Execução."
- Footer: "Powered by GuessLess — Growth Agency"
- Accent usado com moderação — apenas CTAs, scores e navegação ativa
- Sem emojis excessivos na UI — ícones SVG ou Unicode contidos
