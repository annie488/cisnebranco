# Coral Cisne Branco — site

Site institucional do **Coral Cisne Branco**, do **Instituto Cisne Branco Cultural** (Foz do Iguaçu, PR). Site estático, uma página, com SEO/AEO e versão bilíngue PT/ES.

## Arquivos
- `index.html` — o site inteiro (HTML + CSS + JS em um arquivo). Bilíngue (PT padrão, ES via botão), botão flutuante de WhatsApp, FAQ, dados estruturados.
- `images/` — fotos do site (ver `images/LEIA-ME.txt`). Ainda a adicionar: `og-cover.jpg`, `logo.png`.
- `robots.txt`, `sitemap.xml`, `llms.txt` — SEO e AEO (busca + assistentes de IA).
- `PRD-coral-cisne-branco.md` — requisitos e direção de design.
- `COMO-PUBLICAR.md` — guia de deploy (Netlify / Vercel / GitHub Pages).

## Direção de design
Editorial e elegante: fundo em tom de papel, tipografia serifada (Fraunces) + sans (Inter), filetes finos, ilustração de cisne em traço fino. **Não** usar gradientes coloridos, emojis como ícones ou cards com sombra genéricos.

## O que ainda falta
1. Adicionar fotos reais em `images/` e encaixá-las no layout (topo, galeria).
2. Opcional: adicionar vídeo (arquivo `.mp4` ou embed do YouTube/Instagram).
3. Trocar o domínio placeholder `https://coralcisnebranco.com.br` pelo domínio real em `index.html`, `robots.txt` e `sitemap.xml`.
4. Preencher dados de contato: chave Pix (doação), e-mail e redes sociais.
5. Publicar seguindo o `COMO-PUBLICAR.md`.

## Como rodar localmente
É só abrir o `index.html` no navegador. Não precisa de build nem servidor.
