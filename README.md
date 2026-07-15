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

## Entidades (não confundir)
- **Instituto Cisne Branco Cultural** — mantenedor, CNPJ 46.369.725/0001-52, fundado em 05/05/2022.
- **Coral Cisne Branco** — projeto do instituto, fundado em 28/06/2011.

Os dois aparecem separados nos dados estruturados do `index.html` (`NGO` + `MusicGroup` ligados por `parentOrganization`) e no `llms.txt`. Ao editar textos, cuidado para não atribuir "desde 2011" ao instituto.

## Publicação
- Domínio: `https://www.institutocisnebranco.com`
- Repositório: https://github.com/annie488/cisnebranco (público)
- Hospedagem: Hostinger, via Git deploy no hPanel (branch `main` → `public_html`).

## O que ainda falta
1. Adicionar fotos reais em `images/` e encaixá-las no layout (topo, galeria).
2. Opcional: adicionar vídeo (arquivo `.mp4` ou embed do YouTube/Instagram).
3. Preencher dados de contato: chave Pix (doação), e-mail e redes sociais — hoje estão como "a definir" no rodapé e no `llms.txt`.
4. Adicionar `images/og-cover.jpg` e `images/logo.png` (já referenciados no HTML; sem eles, o compartilhamento em rede social fica sem imagem).

## Como rodar localmente
É só abrir o `index.html` no navegador. Não precisa de build nem servidor.
