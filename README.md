# Tirol · Visibilidade no PDV · planejamento estratégico 75LAB

Planejamento estratégico da 75LAB para a Tirol em formato de apresentação navegável: transformar o espaço de exposição do **BioCiclos + Proteína 70 g** em um ponto de reconhecimento e decisão no varejo alimentar e no atacarejo, com **14 g no seu dia** como território principal.

Dois documentos no mesmo repositório (publicados pelo GitHub Pages; o endereço diferencia maiúsculas de minúsculas):

- **Planejamento estratégico** (uso interno, 40 telas): https://projetos.75lab.com.br/Tirol-Visibilidade-no-PDV/
- **Apresentação comercial** (para a Tirol, 16 telas, com roteiro de fala): https://projetos.75lab.com.br/Tirol-Visibilidade-no-PDV/apresentacao

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

## Apresentação comercial (`apresentacao/`)

Versão para o cliente (10 telas), com a linguagem do KV BioCiclos + Proteína: preto, ondas de leite e copo em SVG, amarelo, Barlow Condensed em itálico, faixas inclinadas, ícones, gráfico de barras e diagramas.
Fio: Abertura → Desafio → A ideia → As peças → Prova → Próximo passo.
1 Capa KV · 2 Quem é a 75LAB · 3 O desafio e por que agora (ver, entender, escolher + mercado e comparativo de proteína por copo) · 4 A ideia (70 g/L → 14 g/copo e três camadas) · 5 As peças (colagem e as sete peças por canal) · 6 Varejo na prateleira: display retrátil e wobblers (arte e aplicados) · 7 Varejo no bloco: stopper 3D e régua de gôndola · 8 Atacarejo: testeira, ponta de gôndola e display caixa de leite · 9 Escala e prova: kits A/B/C, leitura em 3 distâncias e piloto · 10 Próximo passo: 7 etapas, insumos e contato.

Cada tela tem roteiro de fala (`aside.roteiro`, tecla **N**). Usa o motor de `../assets/` e a pele `apresentacao/comercial.css`.

**Imagens dos MPDVs:** salve em `assets/img/mpdv/` com os nomes de `assets/img/mpdv/LEIA-ME.md` (`display-retratil-fechado`, `display-retratil-aberto`, `stopper-copo`, `wobblers`, `testeira-atacarejo`, `ponta-gondola`, `display-chao`; `.jpg`, `.png` ou `.webp`). Elas aparecem sozinhas no lugar reservado; sem a imagem, a tela mostra o nome do arquivo esperado.

Logotipo BioCiclos (`assets/img/logos/biociclos-preto.png` e `-branco.png`) recortado do banner oficial do site tirol.com.br.

## Navegação

← → ou espaço avançam · clique nas bordas da tela · **M** índice · **N** roteiro de fala (apresentação comercial) · **F** tela cheia · Home/End · os botões do topo levam ao início de cada capítulo.
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
