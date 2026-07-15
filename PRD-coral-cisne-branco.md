# PRD — Site Coral Cisne Branco / Instituto Cisne Branco Cultural

> Documento de requisitos para construção do site no Claude Code.
> Cole este arquivo no Claude Code e peça para construir o site inteiro com base nele.

---

## 1. Visão geral

Site institucional do **Coral Cisne Branco**, projeto do **Instituto Cisne Branco Cultural**, de Foz do Iguaçu (PR). O objetivo é apresentar a história do coral, suas ações sociais e converter visitantes em **apoiadores, voluntários (novos cantores) e contratantes de apresentações**.

- **Nome:** Coral Cisne Branco
- **Mantenedor:** Instituto Cisne Branco Cultural (instituição sem fins lucrativos)
- **Cidade:** Foz do Iguaçu — Paraná, Brasil (Tríplice Fronteira)
- **Idioma:** Português (BR)
- **Tipo de site:** Estático (HTML/CSS/JS puro ou framework leve à escolha)
- **Idiomas:** Português (padrão) + Espanhol (aba de troca de idioma, conteúdo 100% traduzido)
- **Referência visual:** ver `index.html` em anexo — é a direção de design aprovada (NÃO usar o visual genérico de gradiente roxo/emojis/cards com sombra).

## 2. Objetivos do site

Em ordem de prioridade:

1. **Receber doações / apoio** ao instituto (ação principal de destaque).
2. **Captar voluntários** — pessoas que queiram cantar no coral.
3. **Receber convites para apresentações** (contratação para eventos e ações).

> ⚠️ **Não incluir página de Agenda.** O instituto não terá quem mantenha as datas atualizadas, então evitar qualquer seção que dependa de atualização constante (calendário, "próximos eventos", etc.).

## 3. Público-alvo

- Moradores de Foz do Iguaçu e da Tríplice Fronteira.
- Potenciais doadores e parceiros (empresas, instituições, poder público).
- Pessoas interessadas em cantar / fazer voluntariado.
- Organizadores de eventos culturais e ações sociais.

## 4. Identidade visual

Direção: **editorial, elegante e atemporal** — cara de instituição cultural com história, não de template. Muito respiro, tipografia protagonista. **Evitar** a estética genérica de IA: gradientes coloridos, emojis como ícones, cards com sombra por toda parte, botões em pílula arredondada.

- **Paleta (tom de papel + tinta + acento):**
  - Papel `#F4F0E6` (fundo), papel escuro `#ECE6D6`, tinta `#1E1B16` (texto), texto suave `#56503F`.
  - Acento bordô `#6B2230` e ouro velho `#A8884E` (usar com parcimônia, em detalhes).
- **Tipografia:** serifada editorial de display — **Fraunces** (Google Fonts) — para títulos; sans-serif limpa — **Inter** — para corpo e rótulos.
- **Recursos de layout:** títulos grandes em serifa, rótulos em caixa-alta com `letter-spacing`, linhas/filetes finos (hairline) em vez de cards com sombra, grid editorial assimétrico, numeração de seções (01–04), citação em "full bleed" com fundo escuro, ilustração de cisne em traço fino (line art SVG, sem emoji), marquee discreto com o repertório, animação sutil de fade ao rolar.
- **Botões:** retangulares (sem cantos muito arredondados), preenchidos em tinta com hover invertido; links de texto com sublinhado fino e seta.

## 5. Estrutura de páginas

5 páginas, todas com a mesma navbar e footer.

### Navbar (fixa no topo, com blur)
Logo (cisne + nome) + links: **Início · Sobre · Projetos Sociais · Apoie · Contato** + botão de destaque "Apoie o coral".

### 5.1. Início (index.html)
- **Hero** com gradiente: título de impacto ("Vozes voluntárias que unem, curam e alegram"), subtítulo, e 2 botões: "Apoie o coral" e "Quero cantar" (link WhatsApp).
- **Estatísticas animadas:** 15 anos de trajetória · 40+ vozes voluntárias · 70+ nacionalidades na cidade · 100% voluntariado.
- **Resumo "Sobre"** com texto curto + link para a página Sobre.
- **Pilares / O que fazemos** (4 cards): Apresentações · Causas sociais · Visitas afetivas · Parcerias.
- **Citação** da fundadora Neusa Miguens.
- **Três formas de participar** (cards): Cante conosco · Apoie o instituto · Convide o coral.
- **CTA final** + footer.

### 5.2. Sobre (sobre.html)
- Cabeçalho da página.
- **O começo / história** (texto longo, ver seção 6).
- **Linha do tempo** (2011 → 2026), ver seção 6.
- **O que nos move** (4 cards): Voluntariado · Diversidade · Inclusão · Repertório plural.
- Citação da fundadora + CTA.

### 5.3. Projetos Sociais (projetos.html)
- Cabeçalho.
- **Frentes de atuação** (cards): Ações na oncologia · Outubro Rosa · Novembro Azul · Visitas a asilos · Natais na cidade · Festival de Corais das Três Fronteiras.
- **Parcerias** (Guarda Mirim e Itaipu Binacional) em destaque.
- **Reconhecimento:** Moção de Aplauso nº 18/2025 da Câmara de Foz.
- CTA.

### 5.4. Apoie (apoie.html) — página mais importante
- Cabeçalho.
- **Três formas de apoiar:** Seja voluntário(a) · Faça uma doação (destaque) · Convide o coral.
- **Bloco de doação** com chave Pix do instituto (placeholder — preencher com dados oficiais).
- Citação + CTA.

### 5.5. Contato (contato.html)
- Cabeçalho.
- **Canais de contato:** grupo de WhatsApp, localização (Foz do Iguaçu), e-mail (placeholder).
- **Formulário** (nome, e-mail, assunto, mensagem) — pode abrir o cliente de e-mail via `mailto` ou integrar com um serviço (Formspree, etc.).

### Footer (em todas as páginas)
Logo + descrição curta do instituto · links de navegação · links de participação (Apoie, WhatsApp, Convidar) · copyright.

## 6. Conteúdo real (informações verificadas)

Usar exatamente estes fatos — todos apurados em fontes públicas.

### Sobre o coral
- O **Instituto Cisne Branco Cultural** é uma instituição **sem fins lucrativos** cuja finalidade é **assistir à sociedade civil e militar em projetos de caráter beneficente**.
- Dentro desse propósito foi criado o **Coral Cisne Branco**, um coral de voluntários civis unidos pelo propósito de soltar a voz — "pois a música possui o poder de unir, curar e alegrar".
- **Fundado em 28 de junho de 2011.** O canto começou com as voluntárias Cisne Branco, num vocalize que deu origem ao coral.
- Em **2026 completa 15 anos** de história.
- Reúne **cerca de 40 vozes voluntárias**. Toda a trajetória foi construída no voluntariado.
- **Presidência:** Neusa da Motta Miguens (fundadora) e seu esposo, José Maria Pinheiro Escobar.
- **Maestros ao longo da história:** Guto Rezende, Renée Cicarelle e, atualmente, Naor.
- **Repertório:** MPB, músicas cristãs, clássicos do sertanejo e canções internacionais.
- De um encontro semanal para cantar, tornou-se **referência cultural em Foz do Iguaçu, na Tríplice Fronteira e em outras cidades do Paraná**.
- A diversidade da cidade (mais de **70 nacionalidades**) se reflete no grupo; **inclusão** é uma bandeira, com integrantes de várias idades.

### Linha do tempo
- **2011** — Fundação do Coral Cisne Branco (28 de junho), dentro do propósito beneficente do Instituto Cisne Branco Cultural.
- **2012** — O canto ganha corpo; encontros semanais e primeiras apresentações pela cidade.
- **Ao longo dos anos** — Conduzido por diferentes maestros (Guto Rezende, Renée Cicarelle e, atualmente, Naor), mantendo o propósito de dar voz às pessoas pela música.
- **2025** — Recebe a **Moção de Aplauso nº 18/2025** da Câmara Municipal de Foz do Iguaçu.
- **2026** — Completa 15 anos e se apresenta no 1∞fronteiras JAZZ Festival, em Foz do Iguaçu.

### Ações sociais (via Instituto Cisne Branco Cultural)
- Apresentações em **asilos**.
- **Ações na oncologia** (apoio a pacientes em tratamento).
- Participação em campanhas **Outubro Rosa** e **Novembro Azul** (incluindo apresentações na Câmara de Vereadores).
- **Apresentações de Natal** em espaços públicos da cidade.
- **Festival de Corais das Três Fronteiras.**
- **Parcerias** com jovens da **Guarda Mirim** e da **Itaipu Binacional**.
- Frase-síntese: *"A música, para o Coral Cisne Branco, é uma ponte entre pessoas, histórias e realidades."*

### Citações da fundadora (Neusa Miguens) — usar como blockquotes
- *"O Coral Cisne Branco nasce e se sustenta no voluntariado, e isso é a base da sua identidade. Cada integrante dedica seu tempo, sua voz e sua energia por escolha, por amor à música e compromisso com o coletivo. Esse espírito transforma o coral em mais do que um grupo artístico: ele se torna uma comunidade."*
- *"Assim como no jazz, onde diferentes vozes e instrumentos dialogam, o coral reúne histórias, timbres e vivências diversas que se encontram na música."*
- *"Os integrantes carregam diferentes histórias, origens e referências, que se encontram e se harmonizam na construção do repertório."*

## 7. Links e CTAs

- **Grupo de WhatsApp (voluntários / "Quero cantar"):** `https://chat.whatsapp.com/J5Bb1eZ4OqQCPthByuXvH0` *(link real do coral)*
- **Doação (Pix):** ⚠️ placeholder — substituir pela chave Pix oficial do instituto.
- **E-mail de contato:** ⚠️ placeholder — substituir pelo e-mail oficial.
- **CTAs principais:** "Apoie o coral" / "Quero doar" · "Quero cantar" / "Entrar no grupo" · "Convide o coral" / "Solicitar apresentação".

## 8. Dados a confirmar antes de publicar (placeholders)

| Item | Status |
|------|--------|
| Chave Pix do instituto | A preencher |
| E-mail oficial | A preencher |
| Telefone / WhatsApp direto (opcional) | A preencher |
| Redes sociais (Instagram/Facebook) | A confirmar |
| Fotos reais do coral | A adicionar (substituir áreas visuais com gradiente) |
| CNPJ do instituto (rodapé, opcional) | A confirmar |

## 9. Requisitos técnicos

- **Bilíngue PT/ES:** seletor de idioma no topo (PT como padrão), com **todo o conteúdo traduzido** (não só o menu). Pode ser feito com dicionário JS via `data-i18n` ou páginas separadas `/pt` e `/es`. Persistir a escolha do usuário.
- **Botão flutuante de WhatsApp:** fixo no canto inferior, sempre visível, apontando para o grupo do coral (`https://chat.whatsapp.com/J5Bb1eZ4OqQCPthByuXvH0`). Estilo discreto, alinhado à identidade (sem verde berrante padrão se quiser manter elegância — opcional).
- **Responsivo** (desktop, tablet, mobile) — menu hambúrguer no mobile.
- **Performance:** site leve, sem dependências pesadas; imagens otimizadas.
- **SEO básico:** `<title>` e `meta description` por página; idioma `pt-BR`; Open Graph com imagem.
- **Acessibilidade:** contraste adequado, textos alternativos em imagens, navegação por teclado.
- **Hospedagem sugerida:** GitHub Pages, Netlify ou Vercel (site estático).
- **Formulário de contato:** via `mailto` (simples) ou serviço externo como Formspree/Web3Forms (sem backend).

## 10. Fontes

- 100fronteiras.com — "Voluntariado e voz: Coral Cisne Branco de Foz do Iguaçu tem 13 anos de histórias" (23/10/2025)
- 100fronteiras.com — "Coral Cisne Branco leva 15 anos de história e quarenta vozes ao 100fronteiras JAZZ Festival" (20/04/2026)
- Câmara Municipal de Foz do Iguaçu — "Coral Cisne Branco recebe Moção de Aplauso da Câmara de Foz" (Moção nº 18/2025)
