# VMagency Portfolio — Progresso

## Concluído

### Estrutura & Layout
- [x] Arquivo `index.html` único, sem dependências de framework
- [x] CSS variables para toda a paleta de cores
- [x] Tipografia: Bebas Neue, Syne, DM Mono (Google Fonts)
- [x] Grid responsivo — mobile (`< 480px`, `< 768px`), tablet (`< 1024px`), desktop
- [x] **Nav hamburger** — menu mobile com slide-down, animação X, lock de scroll, fecha ao clicar no link
- [x] **Swipe touch** no carrossel Veo3 (touchstart/touchend, threshold 40px)
- [x] Cursor customizado: dot volt + ring com lag (lerp), desabilitado em touch

### Seções
- [x] **Nav** — fixa, blur backdrop, logo SVG inline, links, CTA borda volt
- [x] **Hero** — eyebrow, H1, subtítulo, 3 stats com counter animation, scroll indicator, side text rotacionado, radial gradients decorativos
- [x] **Ticker** — marquee infinito, pausa no hover, dot volt antes de cada item
- [x] **Cases** — grid com featured + 2 rows de 2 colunas
- [x] **Sobre** — 3 cards de founders com número, nome, role, quote, força
- [x] **CTA Final** — grid 2 colunas, H2 gigante, botão WhatsApp volt
- [x] **Footer** — logo, nav links, copyright

### Cases implementados
- [x] **Amor Eterno** (featured, full-width) — copy, 6 stats de resultado, insight estratégico, visual com screenshot do app, links TikTok + Instagram + App
- [x] **Limpeza Pós-Obra** — copy, screenshot da landing page, link para o site
- [x] **Click Laser** — copy com dados reais (83.3K seguidores), screenshot do Instagram, link para o perfil
- [x] **Vídeos com IA (Veo3)** — fundo volt, carrossel com 11 vídeos reais (autoplay, muted, loop, lazy-load), navegação prev/next, dots clicáveis, counter, pausa ao sair da viewport
- [x] **Motion Graphics** — anéis concêntricos animados CSS, center dot pulsante, copy

### Micro-interações & Animações
- [x] Scroll animations — `IntersectionObserver`, `opacity 0→1` + `translateY`, stagger entre cards
- [x] Stats counter — contagem animada ao entrar na viewport (hero)
- [x] Arrow line expand — `.arrow-line` expande no hover do card pai
- [x] Float animation CSS — `@keyframes float` declarada
- [x] Pulse — laser dot, center dot
- [x] Shimmer — frame Veo3
- [x] Spin — anéis Motion Graphics
- [x] Scroll indicator — linha animada descendo

---

## Pendente

### Assets em falta
- [ ] **Click Laser** — posts reais do Instagram (grid de criativos) para substituir o screenshot de perfil
- [ ] **Limpeza Pós-Obra** — posts de social media para enriquecer o card (se quiser)
- [x] **Veo3** — carrossel com 11 vídeos reais implementado
- [ ] **Motion Graphics** — frame real de uma animação entregue (opcional)
- [ ] **Foto dos founders** — fotos reais de João Pedro, Matheus e Igor para os cards de sobre (estrutura já pronta para receber `<img>`)

### Dados a confirmar / substituir
- [ ] **Número do WhatsApp** — substituir `wa.me/5511999999999` pelo número real (aparece no nav e no CTA — buscar por `999999999`)
- [ ] **Domínio** — `vmagency.com.br` no rodapé do CTA (confirmar se é esse o domínio)

### Melhorias opcionais (não bloqueiam lançamento)
- [ ] Fotos reais dos founders nos cards da seção Sobre
- [ ] Open Graph image (`og:image`) para preview no WhatsApp/redes ao compartilhar o link
- [ ] Favicon (ícone SVG da VMagency já existe inline, só exportar como `.ico`/`.svg`)
- [ ] Analytics (Google Analytics ou similar)
- [ ] Formulário de contato ou integração com ferramenta (Typeform, etc.) como alternativa ao WhatsApp direto

---

## Assets disponíveis em `assets/`

| Arquivo | Usado em |
|---|---|
| `painelamoreterno.webp` | — (disponível, não está mais no visual principal) |
| `imgaplicaçãoamoreterno.webp` | Case Amor Eterno — visual featured |
| `LimpezaGourmetpagimage.webp` | Case Limpeza Pós-Obra — visual do card |
| `instaclicklaser.webp` | Case Click Laser — visual do card |
| `videoIA.mov` | Carrossel Veo3 — slide 1 |
| `videoIA2.mov` | Carrossel Veo3 — slide 2 |
| `videoIA3.mov` | Carrossel Veo3 — slide 3 |
| `videoIA4.mov` | Carrossel Veo3 — slide 4 |
| `videoIA5.mov` | Carrossel Veo3 — slide 5 |
| `videoIA6.mov` | Carrossel Veo3 — slide 6 |
| `videoIA7.mp4` | Carrossel Veo3 — slide 7 |
| `videoIA8.mov` | Carrossel Veo3 — slide 8 |
| `videoIA9.mp4` | Carrossel Veo3 — slide 9 |
| `videoIA10.mp4` | Carrossel Veo3 — slide 10 |
| `videoIA11.mp4` | Carrossel Veo3 — slide 11 |
