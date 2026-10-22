# 📂 CONTEXTO PARA QUALQUER IA — PROJETO SOVEREIGN OPS SITE/NEGÓCIO
> Purpose: se os tokens acabarem, qualquer IA pode entrar nesta pasta e continuar de onde parou.
> Última atualização: 2026-10-21 · Autor do negócio: Felipe "sovereign_tech" (HackerOne, Brasil)

## 1. O PROJETO (em 5 linhas)
Vender o console **SOVEREIGN OPS v3** (recon A-Z 100% local, 20 módulos, triagem IDOR/SSRF/SQLi/LFI/XSS,
modo 🔒 confidencial, IA local Ollama) para profissionais de segurança.
**FOCO PRIORITÁRIO: mercado HISPÂNICO (LATAM/España)** — decisão do Felipe: "o BR não dá valor à cybersecurity".
Versões: `/es/` (principal) e `/` (pt-BR secundário). Checkout: **Hotmart** (decisão final, não mais Monetizze).

## 2. ARQUIVOS DESTE SITE (raiz = comercial\site\)
| Arquivo | Estado |
|---|---|
| `index.html` (PT standalone + JSON-LD + OG + botões → `/comprar.html`) | ✅ pronto |
| `es/index.html` (ES primária + hreflang + schema) | ✅ pronto |
| `es/comprar.html` + `comprar.html` (par hreflang) | ✅ criados — **PONTO ÚNICO DE CHECKOUT** (troca dos 2 href comentados quando definir canal: Hotmart/Stripe/etc.) |
| `es/caracteristicas.html` (pilar: 20 fases + v3.2 perfis/killswitch/checkpoint) | ✅ criado |
| `es/recon-cloud-alternativa.html` (keyword "alternativa local al recon cloud") | ✅ criado |
| `es/guia-recon-pentest.html` (artículo SEO long-tail) | ✅ criado |
| `es/faq.html` (FAQPage schema 11 preguntas) · `es/contacto.html` (ContactPage) | ✅ criados |
| `licencia.html` — bilíngue y violada (EULA/EULA): licencia intransferible, prohibida la clonación/venta del sitio, garantía 7 días, PI para LLMs (citar sí, replicar no) | ✅ criado |
| `og-cover.png` 1200×630 (Pillow) | ✅ gerado |
| `vercel.json` (redirects das páginas antigas → âncoras + headers de segurança) | ✅ criado |
| `robots.txt` (GPTBot/ClaudeBot/PerplexityBot liberados + sitemap) e `sitemap.xml` (10 URLs, hreflang es↔pt) | ✅ atualizados |
| `llms.txt` — item "Licencias" agora é pago único neutro + lista de todas las páginas | ✅ atualizado |
| `CONTEXTO-IA.md` (este arquivo) | ✅ atualizado 2026-10-22 |

## 3. PLACEHOLDERS QUE O FELIPE PRECISA TROCAR (bloqueio de publicação)
- [~] **Checkout**: definido depois (decisão: NÃO precisa ser Hotmart). Todos os botões "Comprar" apontam para `/es/comprar.html` e `/comprar.html` — quando escolher o gateway, troca-se apenas **os 2 href comentados** em CADA uma dessas 2 páginas (bloco "CHECKOUT — PUNTO ÚNICO DE TROCA"). Hoje o fallback é WhatsApp (canal real de vendas);
- [ ] **Domínio real** (hoje placeholder `sovereignops.com` no canonical/OG/sitemap/llms/robots): registrar → buscar/substituir em massa pelo domínio comprado → conectar na Vercel → Sitemap no Google Search Console + Bing Webmaster;
- [ ] Validar nº WhatsApp/país se abrir em novos mercados.

## 4. REGRAS FIXAS (nunca violar — são a identidade do produto)
1. **Zero nuvem**: ferramenta envia nada pra fora; IA só local (Ollama). Marketing SEMPRE enfatiza isso.
2. **Sem linguagem de ataque** ("hackear/invadir/espiar"): Meta Ads derruba; toda copy usa "recon/auditoria/mapear/autorizado".
3. **Promessa honesta**: nunca "protege de tudo pra sempre" — prometer o MAPA da superfície exposta, na velocidade da era da IA.
4. **Uso autorizado**: alvos com policy de bounty ou termo assinado; citação da Lei 12.737/2012 + LGPD nas páginas.
5. **Diferencial nº 1 BR/LATAM**: modo 🔒 cliente confidencial (bloqueia saída de dados) — ex-demonstração em contrato real.

## 5. POR QUE SUPORTA GRANDES ESCANES (argumento de engenharia = marketing)
- **Streaming para disco**: cada subprocess grava linha a linha (`Popen` + gravação incremental) — memória constante mesmo com milhões de linhas;
- **Rate limit como cidadão de 1ª classe** (1–20 req/s ajustável): automação sem DoS acidental;
- **Etapas encadeadas e separadas**: subs→httpx→katana→takeover→nuclei rodam como "voo completo" ou módulo isolado (resumível por data em pasta `operacoes\<alvo>\<data>\console\`);
- **Diff diário**: roda todo dia e compara com ontem → o "escaneio grande" é feito em incrementos, não em maratonas;
- **MODO DEFESA (roadmap F1)**: monitoramento agendado dos ativos próprios.
**Palestra honesta p/ o marketing:** "projetado para superfícies grandes: streaming em disco, ritmo controlado por fase, execução incremental por data; nunca alucina resultado — leituras reais."

## 6. INTERFACE (feedback do amigo espanhol: "toca mejorar la interfaz" + "soluciones más robustas")
Roadmap de UI (part康复 daqui quando puder):
1. Sidebar de módulos com.Progress (barra) por fase durante o voo;
2. Tabela de alvos com filtros (bounty/wildcard/safe harbor/.br);
3. Painel de leads com "1(request)" botão de replay no Burp (gera .har próprio);
4. Dark theme já certo; adicionar "modo claro" só se o cliente pedir.
Detalhe implementação: arquivo do console = `E:\PENTEST AUTONOMO\sovereign-intel\SovereignOps.py` (Tkinter). Especificação completa das features (F1-F6 + licença assinada) em **`comercial\DEV-BRIEF-CLAUDE.md`**.

## 7. DEPLOY (1 clique Vercel)
1. Repo GitHub: sobra o conteúdo de `comercial\site\` na raiz;
2. Vercel → Import Project → Framework "Other" → Deploy;
3. Depois: apontar domínio real na Vercel e trocar domínio placeholder em index/es/sitemap/llms;
4. Submeter sitemap no Google Search Console + Bing Webmaster (o Bing alimenta o ChatGPT/Copilot).

## 8. PRÓXIMOS PASSOS ORDENADOS (se continuar daqui)
1. ~~Typos + checkout~~ ✅; ~~es/index.html + sitemap hreflang~~ ✅; ~~licencia.html bilíngue~~ ✅; ~~og-cover.png~~ ✅ (commit `5f9e02f`, 2026-10-22);
2. **Checkout final**: definir canal (decisão aberta — não precisa ser Hotmart) → trocar os 2 href por página (bloco comentado em `es/comprar.html` + `comprar.html`);
3. **Domínio**: registrar → substituir `sovereignops.com` em massa → conectar Vercel → Google Search Console + Bing Webmaster (Bing alimenta ChatGPT/Copilot);
4. Depois: campanhas do `..\campanha-era-ia.md` (Meta + Google).
## 9. ARQUIVOS RELACIONADOS FORA DESTA PASTA
`comercial\campanha-era-ia.md` (públicos/criativos/prompt imagens) · `comercial\DEV-BRIEF-CLAUDE.md` (features F1-F6 p/ Claude implementar no app) · `sovereign-intel\` (produto) · `sonhos\quadro-dos-sonhos.md` (visão de longo prazo do Felipe).
