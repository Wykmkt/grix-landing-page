# GRIX Landing Page — Design Specs para Penpot

## Como usar no Penpot
1. Crie um novo projeto "GRIX — Landing Page"
2. Crie um Frame de 1440 x 6000px com fundo `#06060B`
3. Importe os SVGs de cada seção (na pasta `sections/`)
4. Posicione cada seção verticalmente na ordem abaixo

---

## Grid System
- **Container:** 1200px (centralizado)
- **Margens laterais:** 120px cada lado (em 1440px)
- **Gutter:** 24px
- **Colunas:** 12

---

## Paleta de Cores

| Token | HEX | RGB | Uso |
|-------|-----|-----|-----|
| Background | `#06060B` | 6, 6, 11 | Fundo principal |
| Surface | `#0C0C14` | 12, 12, 20 | Cards, navbar |
| Elevated | `#13131F` | 19, 19, 31 | Cards hover |
| Card | `#10101C` | 16, 16, 28 | Cards internos |
| Border | `rgba(255,255,255,0.05)` | — | Bordas |
| Border Hover | `rgba(140,82,255,0.2)` | — | Bordas hover |
| Text Primary | `#F5F5F7` | 245, 245, 247 | Headings |
| Text Secondary | `#A1A1AA` | 161, 161, 170 | Body text |
| Text Muted | `#636370` | 99, 99, 112 | Captions |
| Accent | `#8C52FF` | 140, 82, 255 | CTAs, ícones |
| Accent Light | `#A87AFF` | 168, 122, 255 | Hover |
| Accent Glow | `rgba(140,82,255,0.2)` | — | Glows |
| Gradient Start | `#8C52FF` | — | Gradientes |
| Gradient End | `#C084FC` | — | Gradientes |

---

## Tipografia

| Elemento | Font | Weight | Size | Line Height | Letter Spacing |
|----------|------|--------|------|-------------|----------------|
| Hero Title | Inter | 300 (Light) / 800 (ExtraBold) | 72px | 76px | -3px |
| H2 Seção | Inter | 800 | 48px | 54px | -2px |
| H3 Card | Inter | 600 | 20px | 26px | -0.5px |
| Body | Inter | 400 | 16px | 28px | 0 |
| Small | Inter | 400 | 14px | 22px | 0 |
| XS / Caption | Inter | 400 | 12px | 18px | 0 |
| Badge | Inter | 500 | 10px | 14px | 0.5px |
| Button | Inter | 600 | 14px | 20px | -0.1px |
| Nav Link | Inter | 400 | 14px | 20px | 0 |

---

## Seções (top → bottom)

### 1. NAVBAR (h: 80px, w: 1440px)
- Fundo: `#06060B` com 85% opacidade
- Padding: 0 80px
- **Esquerda:** Logo "🛡️ GRIX" (Inter Bold 16px, branco)
- **Centro:** Links (Inter Regular 14px, `#A1A1AA`)
  - Produto | Como funciona | Soluções | Plataforma | Contato
- **Direita:** 
  - Ícones LinkedIn + Instagram (17px, `#636370`)
  - Botão "Agendar diagnóstico" (outline, radius 999, stroke 1px `rgba(255,255,255,0.12)`)

### 2. HERO (h: 900px, w: 1440px)
- Fundo: `#06060B`
- **Glow roxo:** Ellipse 700x500px, center, fill `#8C52FF` 12% opacity, blur 120px
- **Rim light:** Ellipse 350x350px, center top, fill `#8C52FF` 35% opacity, blur 30px
- **Portrait:** 550x700px, center, opacity 75%, mix-blend: screen, desaturado
- **Badge ISO** (esquerda, y: 50%):
  - Frame 155x180px, fundo `#0C0C14`, border `rgba(255,255,255,0.05)`, radius 16px
  - "2025" (12px, `#8C52FF`, SemiBold)
  - "🛡️" (emoji 24px)
  - "ISO 27001\n27701 · 37001" (13px, Bold, branco)
  - "Certificações próprias em\nSegurança, Privacidade\ne Antissuborno" (10px, `#A1A1AA`)
- **Título linha 1:** "Proteja a decisão." (72px, Inter Light, branco)
- **Título linha 2:** "Blinde sua gestão." (72px, Inter ExtraBold, branco)
- **Subtitle:** "Cibersegurança, Governança e Compliance para gestores que\nrespondem pelo próprio CPF — com metodologia em 90 dias." (16px, `#A1A1AA`)
- **CTAs:**
  - "Diagnóstico executivo" (pill, fill `#8C52FF`, radius 999, 200x48px)
  - "Como funciona" (pill, outline, radius 999, 160x48px)
- **Trust line:** "15+ anos protegendo decisões · 50+ projetos entregues · 3 certificações ISO" (12px, `#636370`)

### 3. HOW IT WORKS (padding: 120px 0)
- **Header** (flex row, space-between):
  - Título: "Como a GRIX protege\nsua gestão ⚙" (48px, ExtraBold)
  - Subtitle: "Da vulnerabilidade à blindagem\nregulatória — em 90 dias." (16px, `#A1A1AA`)
- **Grid** (260px sidebar + 1fr steps):
  - **Sidebar card** "IA Explicável" (fundo `#0C0C14`, border, radius 16px, padding 24px)
    - Ícone estrela (36x36, fundo `rgba(140,82,255,0.06)`, radius 8px)
    - Título: "IA Explicável" (16px, Bold)
    - Bullets: "IA Explicável", "Sem caixa-preta", "Score de confiança" (14px, `#A1A1AA`, dot `#8C52FF`)
  - **4 Steps** (border-bottom `rgba(255,255,255,0.05)`, padding 32px 0):
    - Número: 56px, ExtraBold, gradient text `#8C52FF → transparent`
    - H3: "Diagnóstico Profundo" / "Mapeamento de Riscos" / "Implementação em 90 dias" / "Operação Contínua 24x7"
    - Body: descrição (16px, `#A1A1AA`)

### 4. PLATFORM DASHBOARD (padding: 120px 0)
- **Header:** "A plataforma em ação" (gradient text no "ação")
- **Dashboard frame** (max 1100px, fundo `#0A0B14`, border `rgba(140,82,255,0.1)`, radius 24px, padding 20px, shadow 0 20px 80px `rgba(140,82,255,0.08)`)
- 3 colunas: 240px | 1fr | 240px, gap 12px
- Cada card: fundo `#12131E`, border `rgba(255,255,255,0.04)`, radius 12px, padding 14px
- **Conteúdo:** KPIs, Matriz de Risco, Aderência, Classificação de Dados, RIPD, Donut chart
- Tudo em PT-BR legível

### 5. USE CASES / SOLUÇÕES (padding: 120px 0, fundo: `#0C0C14`)
- **Header:** "Soluções para quem\ndecide sob pressão" (48px)
- **5 cards** (scroll horizontal, 250px cada, gap 16px):
  - Cada card: fundo `#10101C`, border, radius 16px
  - Imagem (aspect 16:10, border-radius top)
  - Título + descrição + "Saiba mais →" (link roxo)
  - Card central: `.featured` (border roxo, shadow, translateY -6px)
- **Cards:** Governança de Dados | MDR com IA 24x7 | Conformidade Regulatória | CISO como Serviço | DPO como Serviço

### 6. WHY CHOOSE (padding: 120px 0)
- **Header:** "Por que gestores\nescolhem a GRIX" (gradient text no "GRIX")
- **3 cards** (grid 3 colunas, gap 16px):
  - Fundo `#0C0C14`, border, radius 16px, padding 32px 28px
  - Card 1: border-left 2.5px `#8C52FF`, "01 — Explica, não reporta"
  - Card 2: "02 — Ex-cliente no comando"
  - Card 3: Badge ISO "🛡️ ISO 27001 / 27701 · 37001"

### 7. CTA FOUNDER (padding: 120px 0, fundo: `#0C0C14`)
- **Grid** (0.9fr | 1.1fr, gap 64px):
  - **Esquerda:** Foto founder (aspect 3:4, max-height 480px, radius 16px)
  - **Direita:**
    - "Vamos blindar\nsua gestão\njuntos. ⚙" (48px, ExtraBold)
    - "Lucien Rocha" (16px, SemiBold) + "Founder & CISO, GRIX" (14px, `#636370`)
    - Quote italic: "Vou pessoalmente revisar seus dados..." (16px, `#A1A1AA`)
    - CTAs: "Agendar diagnóstico" + "Como funciona"

### 8. FOOTER (padding: 72px 0 32px, fundo: `#0C0C14`)
- **Grid** (1.5fr | 1fr | 1fr | 1fr | auto, gap 40px):
  - Col 1: Logo + copyright + Privacy + Terms
  - Col 2: Produto (5 links)
  - Col 3: Empresa (3 links)
  - Col 4: Recursos (4 links)
  - Col 5: Social icons + CTA button

---

## Efeitos Especiais

### Glassmorphism (Navbar)
- `backdrop-filter: blur(24px) saturate(1.4)`
- Background: `rgba(6,6,11,0.8)`
- Border-bottom: `rgba(255,255,255,0.05)`

### Accent Glow (Botões hover)
- `box-shadow: 0 0 40px rgba(140,82,255,0.2), 0 4px 15px rgba(140,82,255,0.3)`

### Hero Portrait Blend
- Opacity: 75%
- Filter: saturate(0.15) brightness(0.55) contrast(1.3)
- Mix-blend-mode: screen
- Mask: linear-gradient vertical (transparent → black → transparent)

### Card Hover
- Border: `rgba(140,82,255,0.2)`
- Transform: translateY(-3px)
- Transition: 0.3s cubic-bezier(0.16, 1, 0.3, 1)

---

*Specs gerados em Abril 2026 para recriar no Penpot.*
