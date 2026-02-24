# VMagency — Portfolio: Briefing Completo para Desenvolvimento
> Documento técnico e estratégico para construção do site portfolio da VMagency.
> Referência de identidade visual, copy, estrutura e cases.

---

## 1. IDENTIDADE DA MARCA

### Conceito
**VMagency** (Visão & Materialização) — Agência digital fundada por três sócios jovens.
Proposta de valor: *"Transformamos a visão do cliente em presença digital real."*

### Personalidade
- Jovem com substância — 25 anos, streetwear refinado
- Moderna, inovadora, próxima, atenciosa
- NÃO é: arrogante, genérica, distante, preguiçosa
- Tom de voz: direto, acessível, profissional sem ser engessado
- Provoca no cliente: **ambição ativada**

### Serviços
- Desenvolvimento Web (sites, landing pages, aplicações)
- Social Media (gestão, criativos, estratégia)
- Criativos com IA (imagens, vídeos Veo3)
- Motion Graphics
- Automação com IA (chatbots, geração de conteúdo)
- Tráfego Pago (Meta Ads, Google Ads)

---

## 2. IDENTIDADE VISUAL

### Paleta de Cores
```
--black:   #090909   /* Void — Background principal */
--white:   #F0EDE8   /* Bone — Texto principal, off-white */
--volt:    #C8FF00   /* Volt — Acento primário, chamadas de ação */
--signal:  #6B5CE7   /* Signal — Acento secundário, gradientes */
--mid:     #111111   /* Surface escura */
--surface: #1A1A1A   /* Cards, superfícies */
--border:  #252525   /* Bordas sutis */
--muted:   #555555   /* Texto desabilitado */
--gray:    #888888   /* Texto secundário */
```

**Regras de uso:**
- Dark-first: fundo sempre `#090909`
- Volt (`#C8FF00`) aparece cirurgicamente — só em acentos, CTAs, destaques. Nunca como fundo de seção inteira (exceto variações de logo)
- Signal (`#6B5CE7`) usado em gradientes, elementos decorativos, segunda hierarquia
- Bone (`#F0EDE8`) para texto principal — nunca branco puro `#FFFFFF`

### Tipografia
```
Display / Headlines grandes:  Bebas Neue — bold, condensado, sem serifa
Subtítulos / Interface / CTA: Syne 800 — geométrico, contemporâneo
Body / Parágrafos:            Syne 400 — clean, legível
Labels / Tags / Dados / UI:   DM Mono — monospace, tech, industrial
```

**Hierarquia:**
- H1 hero: Bebas Neue, ~10-12vw, line-height 0.9
- H2 seções: Bebas Neue, ~6-7vw
- Subtítulos: Syne 700/800
- Corpo: Syne 400, 15-16px, line-height 1.7
- Labels/tags: DM Mono, 10-11px, letter-spacing 4-5px, UPPERCASE

### Logo Mark
Símbolo geométrico: fusão do V (branco, traço bold, stroke-cap square) com M (volt `#C8FF00`, traço secundário, sobreposição) em um único ícone dentro de círculo. Burst radial de 8 linhas finas em volt com baixa opacidade. Ponto central em volt.

Wordmark: "VMagency" em Bebas Neue. Tagline: "VISÃO & MATERIALIZAÇÃO" em DM Mono, muito pequeno, espaçado.

### Estética Geral
- Minimalismo com atitude — não genérico
- Visual dark sofisticado (referência Apple + Nude Project)
- Geometria limpa, sem ornamentos desnecessários
- Animações suaves e intencionais — não decorativas
- Grid-breaking onde fizer sentido
- Cursor customizado (dot volt + ring com lag)
- Sem gradientes purple-on-white, sem Inter/Roboto

---

## 3. ESTRUTURA DA PÁGINA

### Fluxo narrativo estratégico
```
1. NAV          → Presença imediata da marca
2. HERO         → Gancho + autoridade com números reais
3. TICKER       → Serviços em movimento (respiro visual)
4. CASES        → Prova. O coração da página.
5. CAPACIDADES  → O que mais a gente faz (IA, Motion)
6. SOBRE        → Quem são os founders (humaniza a marca)
7. CTA FINAL    → Conversão
8. FOOTER       → Encerra com marca
```

---

## 4. SEÇÃO: NAV

**Logo:** Ícone SVG + "VM" em branco + "agency" em volt. Sempre fixo, blur backdrop.

**Links:** Cases · Serviços · Sobre · Contato

**CTA:** "Falar com a gente" — borda volt, hover preenche volt/preto

**Comportamento:** Fixed, `backdrop-filter: blur(16px)`, `background: rgba(9,9,9,0.85)`, border-bottom sutil.

---

## 5. SEÇÃO: HERO

### Copy
```
Eyebrow (DM Mono, volt):
PORTFOLIO 2025—2026

H1 (Bebas Neue, gigante, 2-3 linhas):
Visão que
vira resultado.

Subtítulo (Syne, cinza):
Do site à automação com IA — construímos a
presença digital de quem quer crescer de verdade.
```

### Stats (números reais, impacto imediato)
```
2.7M    → Views Gerados
903K    → Views IG / 30 dias
+2985%  → Crescimento de Alcance
```

### Detalhes visuais
- Background com radial gradients sutis: signal no canto superior direito, volt no inferior esquerdo — muito baixa opacidade
- Texto rotacionado na lateral direita: "Desenvolvimento · Social Media · IA · Criativos · Motion ·" em DM Mono, color: border
- Scroll indicator: linha vertical animada + texto "Scroll" em writing-mode vertical
- Hero ocupa 100vh, conteúdo ancorado no bottom-left

---

## 6. SEÇÃO: TICKER DE SERVIÇOS

**Comportamento:** Marquee infinito, pausa no hover.

**Itens (separados por borda vertical):**
Desenvolvimento Web · Social Media · Criativos com IA · Motion Graphics · Vídeos Veo3 · Automação · Landing Pages · Tráfego Pago

**Estilo:** DM Mono 11px, letter-spacing 3px, uppercase, gray. Dot volt antes de cada item. Borda top e bottom `var(--border)`.

---

## 7. CASES — Estrutura e Copy

### Layout do grid
```
[  AMOR ETERNO — FEATURED, full width  ]
[  LIMPEZA PÓS-OBRA  |  CLICK LASER   ]
[  VEO3 / IA VIDEO   |  MOTION GFX    ]
```

### Comportamento dos cards
- Entrada com fade + translateY no scroll (IntersectionObserver)
- Hover: background levemente mais claro, arrow-line expande
- Cursor customizado expande o ring no hover

---

### CASE 1 — AMOR ETERNO (Featured / Full Width)
**Tipo:** Projeto Próprio — Case de Crescimento Orgânico

**Tag:** `Case de Crescimento` (highlight volt) · TikTok · Instagram · IA · Produto Digital

**Cliente/período:** Projeto Próprio · Set/2025 — Hoje

**Headline:** Amor Eterno

**Copy do case:**
> Criamos do zero uma marca de luto pet — do nome à identidade, do conteúdo à tecnologia. Em menos de 6 meses, chegamos a 12K seguidores no TikTok e 5.8K no Instagram com crescimento 100% orgânico. 2.7M de visualizações no TikTok e 903K views no Instagram em 30 dias. O projeto vai além das redes: inclui um app de homenagens com IA e uma comunidade ativa no WhatsApp — prova de que conteúdo estratégico + produto digital é uma combinação poderosa.

**Números (resultados):**
```
2.7M    → Views TikTok
903K    → Views IG / 30d
+2985%  → Crescimento de Alcance
192K    → Interações IG / 30d
17.8K   → Seguidores Total (TikTok + IG)
96.8%   → Interações de não seguidores (conteúdo viral)
```

**Visual do card (mockups):**
- Lado esquerdo: layout dividido TikTok | Instagram
- TikTok: mockup de tela de celular dark com @amoreterno, badge "12K", paw emoji animado com float
- Instagram: ring circular animado (gradiente signal→pink, estilo analytics do IG), seguidores no centro
- Stats cards ao lado de cada plataforma
- Linha divisória vertical sutil entre as duas plataformas

**Insight estratégico (exibir no card):**
> 96.8% das interações vêm de não seguidores. O conteúdo não cresce porque tem seguidores — tem seguidores porque o conteúdo cresce.

---

### CASE 2 — LIMPEZA PÓS-OBRA & ESTOFADOS
**Tipo:** Cliente Recorrente

**Tag:** Social Media · Landing Page · Criativos

**Cliente/período:** Cliente Ativo · Recorrente

**Headline:** Limpeza Pós-Obra

**Copy do case:**
> Primeiro cliente recorrente da VMagency. Gestão completa de social media com posts 3x por semana — criativos profissionais que transmitem limpeza, confiança e resultado. Landing page desenvolvida e entregue, convertendo visitas em orçamentos. Do post ao site, tudo alinhado.

**O que foi entregue:**
- Posts 3x por semana (criativos com IA)
- Landing page desenvolvida e paga
- Identidade visual nos materiais

**Visual do card:**
- Stack de posts empilhados (rotação leve, sobreposição)
- Mockup de landing page (browser frame minimal, hero bar em volt)
- Paleta de tons verdes escuros para o background do visual

---

### CASE 3 — CLICK LASER
**Tipo:** Cliente Recorrente

**Tag:** Social Media · Estética · Criativos

**Cliente/período:** Cliente Ativo · Recorrente

**Headline:** Click Laser

**Copy do case:**
> Clínica de estética e laser com posicionamento premium. Gestão de social media com posts 3x por semana — criativos que comunicam resultado, sofisticação e confiança. Visual alinhado ao universo estético: roxo profundo, luz, precisão.

**O que foi entregue:**
- Posts 3x por semana
- Criativos com identidade premium
- Estratégia de conteúdo para estética

**Visual do card:**
- Grid 2x2 de posts com tons roxos profundos
- Dot animado (pulse) representando o laser
- Paleta: gradientes roxos `#150040 → #350d70`

---

### CASE 4 — VÍDEOS COM IA (Veo3)
**Tipo:** Capacidade / Serviço

**Tag:** Veo3 · IA · Conteúdo · `highlight volt`

**Card accent:** fundo volt, texto preto

**Headline:** Vídeos com IA

**Copy:**
> Produção de vídeos com Veo3 — a ferramenta de geração de vídeo por IA da Google. Conteúdo visual profissional sem equipe de filmagem, sem locação, sem espera. Mais rápido, mais barato, mesma qualidade visual. Do roteiro ao arquivo final.

**Diferencial:**
> Entregamos o que leva semanas de produção em dias.

**Visual:** Frame de vídeo com play button, badge "Veo3 · IA Video", shimmer animation sutil.

---

### CASE 5 — MOTION GRAPHICS
**Tipo:** Capacidade / Serviço

**Tag:** Motion Graphics · Animação · After Effects · `highlight volt`

**Headline:** Motion Graphics

**Copy:**
> Animações que transformam identidade em movimento. Posts animados, intros, transições, identidade visual em vídeo — do storyboard ao arquivo final. Para marcas que querem ir além do estático.

**Visual:** Anéis concêntricos animados (rotation, velocidades distintas, counter-rotation), dot volt pulsando no centro. Paleta signal/volt.

---

## 8. SEÇÃO: SOBRE (FOUNDERS)

### Copy da seção
```
Eyebrow: 03 — Quem faz

H2: A agência
    somos nós.

Subtexto:
Três sócios, três perspectivas, um objetivo:
fazer o digital funcionar de verdade para
quem tem negócio pra crescer.
```

### Cards dos founders
```
JOÃO PEDRO, 20
Dev & Criativos com IA
"Transforma o briefing em código e o código em resultado."
Força: Desenvolvimento web, criativos com IA

MATHEUS, 20
Vendas & Social Media
"O cara que faz a conversa acontecer e o conteúdo engajar."
Força: Relacionamento, organização, social media

IGOR, 27
Marketing & Estratégia
"3 anos em eventos de grande porte. Agora aplica essa visão no digital."
Força: Estratégia, marketing, visão de mercado

EUGÊNIO JUNIOR
Head de Processos & Design de Conversão
"Design não é estética — é comportamento. Cada detalhe visual tem uma razão para converter."
Formação: Análise de Dados + Engenharia de Banco de Dados (FIAP) · Designer Gráfico
Especialidade: Design por vieses inconscientes para conversão, desenvolvimento comercial, branding inteligente
Força: Inteligência de dados aplicada ao design, geração e recolhimento de leads, gestão de processos e projetos
```

**Layout:** Grid 2x2 (4 cards). Cada card: número do founder (DM Mono, volt, grande), nome em Bebas Neue, role em DM Mono. Fundo `--surface`. Hover: borda volt aparece.

**Nota estratégica para o Claude Code:** O Eugênio representa o diferencial mais difícil de copiar da VMagency — design fundamentado em dados e psicologia de conversão. O card dele deve ter uma linha de copy extra: "Cada elemento visual tem uma razão científica para converter."

---

## 9. SEÇÃO: CTA FINAL

### Copy
```
H2 (Bebas Neue, gigante):
Próximo
case
é o seu.

Subtexto (Syne, gray):
A gente cuida do digital pra você
focar no que importa — crescer.
Site, social, criativos e automação com IA.
Rápido. Com resultado.

CTA principal (botão volt, texto preto, Bebas Neue):
Falar no WhatsApp →

CTA secundário (DM Mono, muted):
@vmagency · vmagency.com.br
```

**Layout:** Grid 2 colunas, headline na esquerda, copy + CTA na direita. Fundo `--mid` diferenciado.

---

## 10. FOOTER

```
Esquerda: Logo (ícone SVG + wordmark)
Centro: nav links sutis
Direita: © 2026 VMagency · Visão & Materialização

Linha superior: border var(--border)
Background: --black
Tipografia: DM Mono, muted, uppercase
```

---

## 11. MICRO-INTERAÇÕES & ANIMAÇÕES

### Cursor customizado
```css
/* Dot principal */
width: 8px; height: 8px;
background: var(--volt);
border-radius: 50%;
position: fixed; z-index: 9999;
transform: translate(-50%, -50%);
transition: transform 0.1s;

/* Ring com lag */
width: 32px; height: 32px;
border: 1px solid rgba(200,255,0,0.4);
border-radius: 50%;
position: fixed; z-index: 9998;
/* segue com lerp: rx += (mx - rx) * 0.12 */

/* Hover em elementos interativos: ring expande para 60px, border-color vai para rgba(200,255,0,0.7) */
```

### Scroll animations
Cards entram com `opacity: 0 → 1` + `translateY(30px → 0)`, `transition: 0.6s ease`, via IntersectionObserver com `threshold: 0.1`.

### Ticker / Marquee
`animation: marquee 20s linear infinite`. Pausa no hover. Duplicate items para loop perfeito.

### Float animation (paw / ícone Amor Eterno)
```css
@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-6px); }
}
duration: 3s ease-in-out infinite
```

### Arrow line expand
`.arrow-line` tem `max-width: 40px` default, vai para `80px` no hover do card pai. `transition: max-width 0.3s ease`.

### Spin lento (logo hero / decorativo)
`animation: spin 30s linear infinite` — usado no ícone da hero ou elementos decorativos.

### Pulse (laser dot, IG ring, center dot)
```css
@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 0.8; }
  50% { transform: scale(1.3); opacity: 1; }
}
duration: 2s ease-in-out infinite
```

### Shimmer (video frame)
```css
@keyframes shimmer {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}
/* gradiente diagonal em pseudo-element, duration: 3s */
```

---

## 12. COMPONENTES REUTILIZÁVEIS

### Tags / Pills
```
.tag         → border: var(--border), color: var(--muted), DM Mono 9px, letra 2px
.tag.highlight → border: var(--volt), color: var(--volt)
.pill        → border-radius: 100px, mesmas regras
```

### Section header pattern
```
[eyebrow: DM Mono volt, "01 — Label"]
[H2: Bebas Neue, grande]
[border-bottom: var(--border)]
[count / meta info: DM Mono muted, alinhado à direita]
```

### Result item
```
[número: Bebas Neue 32px, volt]
[label: DM Mono 9px, letter-spacing 2px, muted, uppercase]
```

### Case arrow CTA
```
[linha expansível volt] + [texto DM Mono volt uppercase "Ver Case →"]
```

---

## 13. RESPONSIVIDADE

### Breakpoints principais
```
Mobile: < 768px
Tablet: 768px - 1024px
Desktop: > 1024px
```

### Adaptações mobile
- Nav: esconder links, manter logo + CTA
- Hero: stats em coluna, font menor
- Cases grid: 1 coluna (incluindo featured)
- Featured case: flex-direction column
- Ticker: manter (funciona bem mobile)
- Founders: 1 coluna
- CTA: 1 coluna
- Footer: coluna centralizada
- Cursor: desabilitar em touch devices (`@media (hover: none)`)
- Section padding: reduzir de 120px para 60px laterais 24px

---

## 14. ASSETS NECESSÁRIOS

### Google Fonts (import)
```
https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Bebas+Neue&family=Syne:wght@400;600;700;800&display=swap
```

### Logo SVG (inline)
Construído em SVG puro — não requer arquivo externo. Ver seção 2.

### Ícones
Não usar bibliotecas de ícones — usar SVG inline ou caracteres unicode/arrows onde necessário.

---

## 15. COPY — REGRAS DE TOM

### O que a VMagency diz
- "A gente" (não "nós" formal)
- "Você" (nunca "senhor/senhora")
- "Rápido. Com resultado." (direto, sem enrolação)
- "Do zero." (mostra capacidade total)
- "Foca no que importa — crescer." (benefício, não ferramenta)

### O que a VMagency NÃO diz
- "Soluções inovadoras e disruptivas"
- "Especialistas em marketing digital"
- "Prezado cliente"
- "Contamos com uma equipe qualificada"
- Qualquer coisa que soe como agência de cidade pequena

### Padrão de copy por seção
```
Hero:      Impacto emocional + credibilidade (números reais)
Cases:     Resultado primeiro, processo depois
Sobre:     Humano, direto, sem auto-elogio excessivo
CTA:       Benefício imediato + ação simples
```

---

## 16. META / SEO

```html
<title>VMagency — Agência Digital | São Paulo</title>
<meta name="description" content="Agência digital especializada em desenvolvimento web, social media e criativos com IA. Cases reais: 2.7M de views gerados, crescimento orgânico comprovado.">
<meta property="og:title" content="VMagency — Visão & Materialização">
<meta property="og:description" content="Transformamos a visão do seu negócio em presença digital real.">
```

---

## 17. NOTAS FINAIS PARA DESENVOLVIMENTO

1. **Single file HTML** — tudo inline (CSS + JS + SVG). Sem dependências externas além das Google Fonts.
2. **Não usar** Bootstrap, Tailwind, jQuery ou qualquer framework CSS.
3. **CSS Variables** para toda a paleta — facilita manutenção.
4. **SVG logo** sempre inline — nunca como `<img src>`.
5. **Performance:** lazy load se houver imagens reais, sem bibliotecas pesadas.
6. **Cursor customizado:** desabilitar em dispositivos touch.
7. **Substituir mockups por screenshots reais** dos projetos quando disponíveis — estrutura já preparada para receber.
8. **Seção Airbnb:** removida do portfolio.
9. **Ordem dos cases:** Amor Eterno (featured) → Limpeza Pós-Obra → Click Laser → Veo3 → Motion Graphics.
10. O card do **Veo3 usa fundo volt** (fundo verde-limão, texto preto) — variação de cor única na página.
