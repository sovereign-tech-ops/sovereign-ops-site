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
| `index.html` (PT standalone + JSON-LD SoftwareApplication/Product/FAQPage + OG) | ✅ pronto — faltam 3 typos (linhas ~235-237: "internar"→"ranqueada", "VOO COMPLETE...Raven"→"VOO COMPLETO...o log rolando", "caços"→"caça") e trocar placeholders de checkout p/ Hotmart |
| `robots.txt` | ✅ pronto (permite GPTBot, ChatGPT-User, PerplexityBot, ClaudeBot, Claude-Web, Google-Extended, Applebot-Extended, CCBot) |
| `sitemap.xml` | ✅ apenas /pt — ADICIONAR `/es/` + hreflang alternates |
| `llms.txt` | ✅ pronto (ES, padrão llms.txt, cláusula IP: citar ok, replicar NÃO) |
| `es/index.html` | ⏳ CRIAR (prioridade máxima, Lang es + hreflang, mesmo schema, checkout Hotmart) |
| `licencia.html` | ⏳ CRIAR (términos anti-copia/EULA nos 2 idiomas) |
| `og-cover.png` | ⏳ gerar 1200×630 (prompts em `..\campanha-era-ia.md`) |
| `style.css` e páginas multi-antigas (ferramentas/como-funciona/planos/compliance/contato/era-ia) | conteúdo já consolidado no index standalone; manter como apoio ou desativar links depois |

## 3. PLACEHOLDERS QUE O FELIPE PRECISA TROCAR (bloqueio de publicação)
- [ ] Links de checkout Hotmart (2 créditos Starter/Pro);
- [ ] Domínio real (hoje placeholder `sovereignops.com.br` no canonical/OG/sitemap/llms.txt) — trocar EM MASSA;
- [ ] `og-cover.png` (gerar imagem);
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
1. Corrigir os 3 typos do `index.html` + trocar checkout p/ Hotmart;
2. Criar `es/index.html` (foco) e re-escrever `sitemap.xml` com /es + hreflang;
3. Criar `licencia.html` (anti-cópia/EULA) e linkar no footer das duas lands;
4. Gerar `og-cover.png`;
5. Depois: Google/Bing webmasters, Hotmart produto ativo, campanhas do `..\campanha-era-ia.md`.
## 9. ARQUIVOS RELACIONADOS FORA DESTA PASTA
`comercial\campanha-era-ia.md` (públicos/criativos/prompt imagens) · `comercial\DEV-BRIEF-CLAUDE.md` (features F1-F6 p/ Claude implementar no app) · `sovereign-intel\` (produto) · `sonhos\quadro-dos-sonhos.md` (visão de longo prazo do Felipe).
