# Tirol · Visibilidade no PDV · planejamento estratégico 75LAB

Planejamento estratégico da 75LAB para a Tirol em formato de apresentação navegável: transformar o espaço de exposição do **BioCiclos + Proteína 70 g** em um ponto de reconhecimento e decisão no varejo alimentar e no atacarejo, com **14 g no seu dia** como território principal.

Publicação prevista: https://projetos.75lab.com.br/tirol-visibilidade-no-pdv/ (quando o GitHub Pages estiver ativo no repositório).

Fonte do conteúdo: `Tirol_Visibilidade_PDV_Planejamento_Estrategico_75LAB.pdf` (17 páginas, 19/nov/2026). O PDF fica fora do Git.

## Telas (40)

| Capítulo | Telas |
|---|---|
| Abertura | Capa · síntese em seis respostas |
| 1 · Diagnóstico | Leitura do desafio · decupagem do briefing · públicos e resposta desejada · o que sabemos · o que falta descobrir e hipóteses · contexto de marca · mercado · concorrência · quatro perfis de shopper · jornada no PDV · tendências |
| 2 · Estratégia | Insights · três insights prioritários · tensão central · oportunidade e "como podemos" · de → para · pilares · territórios (abas) · direção recomendada |
| 3 · Solução | Hero + Support + Scale · conceito 01 varejo (bloco de decisão) · conceito 02 atacarejo (bloco de visibilidade) · teste de leitura · clusters e produção · inovações |
| 4 · Execução | Entregáveis · priorização MoSCoW · KPIs e piloto · pré-mortem · conformidade regulatória · roadmap · recomendação · checklist para iniciar o design · fontes |

Cada capítulo abre com uma tela-divisória dourada.

## Navegação

← → ou espaço avançam · clique nas bordas da tela · **M** índice · **F** tela cheia · Home/End · os botões do topo levam ao início de cada capítulo.
No celular, as telas viram uma página de rolagem; tocar no topo abre o índice.
QA: `?static` (sem animação), `?desktop` (força o palco no celular).

## Estrutura

- `index.html`: todas as telas (`section.slide`, com `data-cap` para o capítulo e `data-title` para o índice).
- `assets/css/deck.css`: palco de 1600 × 900 escalado à janela, paleta da linha BioCiclos (branco, preto e dourado), componentes, esquemas de PDV (bloco, régua, stopper, testeira) e versão celular (`html.m`).
- `assets/js/deck.js`: navegação, índice, trilha de capítulos e abas (`data-abas`). Mesmo motor do projeto Danone PDV 2027.
- `assets/img/packs/`: embalagens BioCiclos (+ Proteína, Adultos, Senior 50+, Kids) do site oficial tirol.com.br, recortadas, em webp (`-p` = versão leve).
- `assets/img/logos/`: logotipo Tirol do site oficial (original, preto e branco) e 75LAB.

HTML, CSS e JS puros, sem build e sem dependências (só fontes do Google: Archivo e Figtree).

## Cuidados

Documento de planejamento: hipóteses, territórios, esquemas de PDV, clusters e avaliações são propostas da 75LAB, não decisões nem resultados da Tirol. Os esquemas das telas de solução são estudos de princípio, não artes finais. Claims ("14 g por copo de 200 ml", "zero lactose"), números de mercado e nomenclatura precisam ser conferidos no rótulo vigente e nas fontes originais antes de qualquer versão externa.
