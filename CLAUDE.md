# CLAUDE.md — SUBBEACHWEAR

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** SUBBEACHWEAR
**Nicho:** Moda e Beleza
**Keywords:** Ola Meu nome e Claudia e sou a fundadora da subbeachwear com
**Paleta de cores:** ocean | **Fonte:** poppins

Olá! Meu nome é Claudia e sou a fundadora da subbeachwear.com.br, a maior loja online de roupas femininas de Osasco. Depois de trabalhar no mundo corporativo por muitos anos, decidi perseguir meu sonho de iniciar meu próprio negócio. A roupa de baixo é um trabalho de amor para mim. Sou apaixonado por ajudar as mulheres a se sentirem bonitas e confiantes em seus trajes de banho e de praia. Acredito que toda mulher merece olhar e sentir o seu melhor, não importa o seu tamanho ou forma. Obrigado por visitar nosso site! Esperamos que você encontre algo que você ama!



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-G |
| Hero | Hero-C |
| Features | Features-E |
| About Section | About-E |
| Posts | Posts-J |
| Footer | Footer-B |
| Página Sobre | Sobre-D |
| Página Contato | Contato-E |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
