# Como publicar o site (passo a passo)

O site é estático (só HTML/CSS/JS), então é leve, gratuito de hospedar e rápido. Você tem 3 caminhos — listados do mais fácil ao mais "de programador".

---

## O que tem na pasta

```
index.html        → o site inteiro (uma página só)
robots.txt        → instruções para buscadores e IAs
sitemap.xml       → mapa do site para o Google
llms.txt          → resumo do coral para assistentes de IA (AEO)
images/           → coloque aqui as fotos (veja o LEIA-ME.txt dentro)
```

> **Antes de publicar:** abra o `index.html`, o `robots.txt` e o `sitemap.xml` e troque
> `https://coralcisnebranco.com.br` pelo seu domínio real (ou pelo endereço que a
> hospedagem gerar). É só usar "localizar e substituir".

---

## Opção 1 — Netlify Drop (mais fácil, sem conta técnica)

1. Acesse **https://app.netlify.com/drop**
2. **Arraste a pasta inteira** do site para a área indicada na página.
3. Pronto: em segundos o site fica no ar com um endereço tipo `nome-aleatorio.netlify.app`.
4. Para um endereço bonito, crie uma conta grátis e em *Site settings → Change site name* escolha algo como `coralcisnebranco`.
5. Para usar domínio próprio (ex.: `coralcisnebranco.com.br`), vá em *Domain settings* e siga as instruções.

**Para atualizar depois** (trocar fotos, textos): só arrastar a pasta de novo.

---

## Opção 2 — Vercel

1. Crie uma conta grátis em **https://vercel.com** (pode entrar com o GitHub ou e-mail).
2. Clique em **Add New → Project**.
3. A forma mais simples sem programar: instale o "Vercel CLI" não é necessário —
   use a opção de importar do GitHub (ver Opção 3) **ou** arraste a pasta usando o
   **Vercel Deploy** (also drag-and-drop em https://vercel.com/new).
4. O site sobe com endereço `seu-projeto.vercel.app`.
5. Domínio próprio: *Settings → Domains → Add*.

> Vercel e Netlify são equivalentes para este site. Se ficar em dúvida, use o **Netlify Drop** (Opção 1) — é o caminho mais direto.

---

## Opção 3 — GitHub Pages (bom se você for usar o Claude Code / versionar)

1. Crie uma conta em **https://github.com**.
2. Crie um repositório novo (ex.: `coral-cisne-branco`), público.
3. Faça upload de **todos os arquivos** da pasta (botão *Add file → Upload files*).
4. Vá em **Settings → Pages**.
5. Em *Source*, escolha a branch `main` e a pasta `/ (root)`. Salve.
6. Em 1–2 minutos o site fica em `https://seu-usuario.github.io/coral-cisne-branco/`.
7. Domínio próprio: em *Settings → Pages → Custom domain*.

> Esse é o caminho ideal se você for continuar editando o site pelo **Claude Code**, porque ele já trabalha com Git/GitHub.

---

## Depois de publicar — para aparecer no Google e nas IAs

1. **Google Search Console** (https://search.google.com/search-console): adicione seu site, confirme a posse e envie o `sitemap.xml`. Isso acelera a indexação.
2. **Bing Webmaster Tools** (https://www.bing.com/webmasters): mesma ideia — e o Bing alimenta várias buscas com IA.
3. Confirme que o `robots.txt` e o `sitemap.xml` abrem no navegador (ex.: `seudominio.com/robots.txt`).
4. Teste os dados estruturados no **Rich Results Test**: https://search.google.com/test/rich-results — cole a URL do site e veja se a Organização e o FAQ aparecem.

> O conteúdo já foi preparado para **SEO** (busca tradicional) e **AEO** (ser citado por ChatGPT, Claude, Gemini, Perplexity): tem dados estruturados, FAQ, `llms.txt` e o `robots.txt` libera os robôs de IA.

---

## Adicionar as fotos

1. Coloque as imagens na pasta **`images/`** (veja o `LEIA-ME.txt` lá dentro).
2. Use os nomes `og-cover.jpg` (capa de compartilhamento) e `logo.png`.
3. Se quiser mostrar fotos dentro do site (no topo, numa galeria etc.), me mande as fotos que eu encaixo no layout.

---

## Domínio próprio (.com.br)

- Registre em **https://registro.br** (para `.com.br`) — custa cerca de R$ 40/ano.
- Depois aponte o domínio para a Netlify/Vercel/GitHub seguindo as instruções de "Custom domain" de cada uma (elas te dão os registros de DNS para colar no registro.br).

---

### Resumo rápido
- **Quer no ar em 2 minutos, sem complicação?** → Netlify Drop (Opção 1).
- **Vai editar com o Claude Code e versionar?** → GitHub Pages (Opção 3).
- **Já usa Vercel?** → Opção 2.
Todas as três são **gratuitas** para um site como esse.
