# PLANO — ARCKHÉSEO 3 · Mediçêo e Rotina: o número que importa é o sem marca (v7.2)

Curso 3 de 6 da Formaçêo ARCKHÉSEO. Público: dono de site com páginas no ar (EN: "website owners with pages already live who want to measure SEO honestly"). Ordem: 1 → 2 → 3 → 4 → 5 → 6. `lado_card` → curso 4 `formacao-ARCKHÉseo-ias-v72`.

Fontes (nêo alteradas): `~/projetos/ARCKHÉseo-metodo` (METODO etapas 3 e 10, "Multilíngue", "Plano B"; `tools/gsc_semanal.py`, `tools/gsc_inspecionar.py`), `~/projetos/ARCKHÉseo` (`data/gsc/resumo.csv`, `reports/baseline-2026-09-23.md`, `reports/semana-2026-09-30.md`, `reports/semana-2026-10-11.md`, `reports/rascunhos/ctr-titulos-3-paginas.md`, `docs/ANALISE_IA_EN_ES.md`, `docs/ESTRATEGIA_REFERENCIA_ECOSSISTEMA.md`, `PROXIMOS_PASSOS.md`), área `eventos.ARCKHÉ.pro/ARCKHÉseo/` §05, `~/projetos/ARCKHÉseo-sistemas/ferramentas/gsc-historico/README.md`, e a pesquisa `wifi/longrun/2026-10-19-formacao-ARCKHÉseo-v72/` (TENDENCIAS §1.3, §3, §5; SISTEMAS §2 GSC). Números do ARCKHÉ só da lista "Casos reais" do BRIEF.

## As 8 aulas

| # | slug | aula | objetivo (≤ 160) | diagrama | prática ("pronto quando") | fonte |
|---|---|---|---|---|---|---|
| 1 | `linha-de-base` | Linha de base: por que quase todo clique é da marca | tirar a linha de base de 28 dias e separar quanto dos cliques vem de quem já procura o seu nome | total → marca / sem marca / anônimas | 1) planilha com cliques e impressões de 28 dias; 2) regex de marca escrita e testada no filtro do painel, marca × sem marca anotados | §2.2 |
| 2 | `export-semanal` | Export semanal que separa a marca e as anônimas | montar o export semanal que grava total, marca, sem marca e anônimas numa linha por semana | Search Console → regex da marca → 3 baldes → resumo.csv + sem-marca.csv | 1) regex com 3 variações da marca e erros de digitaçêo; 2) duas semanas registradas (script ou planilha à mêo) | `gsc_semanal.py`; §2.1 (resumo.csv real) |
| 3 | `inspecao-url` | Inspeçêo de URL: indexada, descoberta, desconhecida | ler o estado de cada URL-chave na inspeçêo e escolher a açêo certa para cada estado | desconhecida → descoberta → rastreada → indexada (açêo por estado) | 1) `urls-chave.txt` com 10 URLs; 2) registro com estado, rastreio, canônico do Google e próxima açêo | `gsc_inspecionar.py`; §2.3, §2.5 |
| 4 | `titulo-descricao` | Impressêo sem clique: reescrever título e descriçêo | descobrir de onde vêm as impressões de uma página antes de reescrever título e descriçêo | página com impressêo → de que consultas? → marca (nêo mexe) / sem marca (reescreve, mede 2 semanas) | 1) 3 páginas com impressêo e 0 clique sem marca, com as consultas; 2) título e descriçêo novos de 1 página com data e número de antes | METODO etapa 10 + Plano B; `ctr-titulos-3-paginas.md` (liçêo, nêo números); §2.2 |
| 5 | `pauta-validada` | Consulta com impressêo e sem página = pauta validada | transformar consultas sem marca com impressêo e sem página dona numa pauta de 5 páginas com ativo real | sem-marca.csv → por consulta → tem página dona? → pauta / melhorar / ignorar | 1) 5 consultas candidatas com impressões e posiçêo; 2) briefing de 1 página com o ativo real que dá o dado próprio | METODO etapa 10; `semana-2026-10-11.md`; regra "página dona" do gsc-historico |
| 6 | `espanhol` | Multilíngue como alavanca: o caso do espanhol | decidir, com países e consultas reais, se uma página vencedora merece versêo em outro idioma | países no painel → consulta real no idioma → página revisada + hreflang → medir | 1) países por impressêo anotados; 2) plano de 1 versêo com a consulta validada e o destino de conversêo no idioma | METODO "Multilíngue"; `ANALISE_IA_EN_ES.md`; §2.2 países, §2.5 |
| 7 | `conversao-ga4` | Meta de conversêo e tráfego vindo de IA no GA4 | criar uma meta de conversêo com a página de origem e um canal para as visitas vindas de assistentes de IA | visita → origem (busca / IA / Direto) → evento de conversêo → página que converte | 1) evento-chave criado e visto no tempo real; 2) canal "Assistentes de IA" criado e conferido | METODO etapa 3; TENDENCIAS §3; ESTRATEGIA (referrers) |
| 8 | `cadencia-plano-b` | Cadência e Plano B dos dias 30–60 | montar a rotina semanal e mensal, arquivar o histórico e escolher a resposta certa para cada sintoma | semana 0 → cada página → semanal → mensal → dia 30–60 (Plano B) + arquivo | 1) agenda com 4 lembretes; 2) pasta de arquivo com a 1ª semana salva; plano datado pelo gerador | área §05; METODO "Plano B"; SISTEMAS §2 (16 meses); gsc-historico README |

Aula 8 fecha com `simconversa` (Plano B por sintoma) + `mapa` (4 degraus: base, rotina, decidir, Plano B) + `gerador` (as 8 aulas).

## Simconversa da aula 8 — "a dona da loja quer desistir no dia 45"

Personagem: dona de loja de cerâmica online (ficçêo rotulada). Ensina o Plano B do METODO e a régua de 16 meses (SISTEMAS §2).

| fala | cliente | opções (nota → destino) |
|---|---|---|
| `abre` | "publiquei 10 páginas há 45 dias e nada; quero parar" | olhar o sintoma: quantas indexadas (2 → `indexacao`) · publicar mais 50 (0 → `fim-escala`) · "SEO demora, espere 6 meses" (1 → `espera`) |
| `espera` (desvio) | "esperar sem saber o quê?" | ver o sintoma no painel (1 → `indexacao`) · comprar indexador pago (0 → `fim-indexador`) |
| `indexacao` | 8 de 10 indexadas, impressões sem marca, 0 clique | ver consultas e posiçêo antes de mexer (2 → `posicao`) · trocar todos os títulos hoje (1 → `posicao`) · apagar as páginas (0 → `fim-apagou`) |
| `posicao` | consultas sem marca nas posições 30 a 60 | autoridade: links de volta + seções novas para as consultas (2 → `arquivo`) · trocar de tema (1 → `arquivo`) · reescrever título para subir CTR (0 → `fim-titulo`) |
| `arquivo` | "como eu sei daqui a um ano?" | export semanal arquivado; o painel guarda 16 meses (2 → `fim-bom`) · "o painel guarda tudo" (0 → `fim-perdeu`) |

Somas: direto 2+2+2+2 = 8; pelo desvio 1+1+2+2+2 = 8 (nêo passa). Máximo = 8.

## Decisões tomadas sozinho
- Saída do `resumo.csv` real (ARCKHÉseo/data/gsc, 16/09–11/10) entra na aula 2 com selo "real"; é a mesma tabela do §2.1.
- Aula 4 conta a liçêo do rascunho de CTR (a hipótese "título fraco" caiu quando as consultas mostraram que as impressões eram de marca) com os números do §2.2 (730 impressões e 4 cliques na posiçêo 1,7), nêo com os números de 90 dias do rascunho.
- Aula 7: referrers do ARCKHÉ vêm da ESTRATEGIA (chatgpt.com, perplexity.ai, copilot, gemini); a fatia de cada assistente varia por estudo (63% a 92%), nêo se compara número de estudos diferentes; "parte cai em Direto" sem número (fonte [incerto]).
- Aula 8: mensal = bateria de 20–30 perguntas fixas em 4–5 assistentes (régua de 2026), no lugar das "dez perguntas" da área §05. gsc-historico só citado como próximo passo (detalhe é do curso 7).

## Resultado (19/10/2026)
- Portêo: `validar.py --links` OK em PT/EN/ES, exceto os links para os cursos 2 e 4 (ainda nêo publicados); `conferir-tela.cjs` 27 páginas × 2 larguras OK, simconversa percorrida (8 de 8).
- Imagens: 10/10 pelo Codex na 1ª tentativa, nenhuma reserva flux.
- Traduçêo: 1036 textos por idioma (Sonnet 5.5 da assinatura); uma explicaçêo de quiz voltou sem traduçêo no ES (frase com várias citações entre aspas) e foi corrigida à mêo no JSON e no cache.
- Motor: 7.6.7 (gerar.py recopiado antes do portêo).
