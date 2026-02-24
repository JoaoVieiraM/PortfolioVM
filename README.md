# VMagency — Portfolio

Site portfolio da VMagency (Visão & Materialização), agência digital fundada por três sócios.

## Stack

- HTML + CSS + JS — arquivo único (`index.html`), zero dependências de framework
- Google Fonts: Bebas Neue · Syne · DM Mono
- Assets locais em `assets/`

## Estrutura do projeto

```
portfolioVM/
├── index.html                     # Página completa (HTML + CSS + JS inline)
├── README.md
├── PROGRESSO.md
├── VMagency_info.md               # Briefing original
└── assets/
    ├── painelamoreterno.webp      # Analytics TikTok — Amor Eterno
    ├── imgaplicaçãoamoreterno.webp # Screenshot app Amor Eterno Pets
    ├── LimpezaGourmetpagimage.webp # Screenshot landing page Limpeza Gourmet
    └── instaclicklaser.webp       # Perfil Instagram Click Laser
```

## Seções da página

| # | Seção | Descrição |
|---|---|---|
| 1 | Nav | Fixa, blur backdrop, logo SVG inline |
| 2 | Hero | H1 grande, stats animados, scroll indicator |
| 3 | Ticker | Marquee infinito de serviços |
| 4 | Cases | 5 projetos em grid (featured + 2 rows) |
| 5 | Sobre | Cards dos 3 founders |
| 6 | CTA | Conversão para WhatsApp |
| 7 | Footer | Links + copyright |

## Antes de publicar

1. Substituir o número do WhatsApp nos dois lugares marcados com `<!-- SUBSTITUIR -->`:
   ```
   https://wa.me/5511999999999  →  número real
   ```
2. Adicionar assets pendentes (ver `PROGRESSO.md`)

## Paleta

| Token | Hex | Uso |
|---|---|---|
| `--black` | `#090909` | Background principal |
| `--white` | `#F0EDE8` | Texto principal (bone) |
| `--volt` | `#C8FF00` | Acento primário, CTAs |
| `--signal` | `#6B5CE7` | Acento secundário, gradientes |
| `--surface` | `#1A1A1A` | Cards |
| `--border` | `#252525` | Bordas |
| `--gray` | `#888888` | Texto secundário |
| `--muted` | `#555555` | Labels, texto desabilitado |
