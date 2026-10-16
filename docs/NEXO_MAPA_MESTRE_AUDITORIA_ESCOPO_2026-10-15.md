# Nexo Cirúrgico — Mapa Mestre do Produto e Inventário de Escopo
**Versão do inventário:** 1.0 | **Data de referência:** 15/10/2026 | **Base auditada:** aplicativo v1.4.5, commit GitHub `aaced6139a3ad90de44b1cbd48fff4636e0516ed` (branch `main`).

**Finalidade:** documento único de controle. Conservar o planejamento vigente dos oito macroblocos; evitar duplicação de conteúdo e novas funcionalidades fora de escopo. **Não altera código nem o conteúdo existente.**

## 1. Decisões congeladas para a conclusão do programa
A plataforma é uma biblioteca **operacional de técnicas médicas** para estudantes e médicos em treinamento supervisionado. **Não é** enciclopédia de doenças, livro didático clássico, rede social, certificado de habilitação profissional ou prontuário. Marca provisória: **Nexo Cirúrgico**; crédito institucional: **Product by InMed**. Idiomas: português e espanhol. Infraestrutura: GitHub + Vercel em camada estática gratuita enquanto for suficiente. Recursos dos usuários armazenados localmente por enquanto.

Conservar **28 módulos** e **227 tópicos catalogados** como escopo curricular inicial, com **224 procedimentos canônicos** para eliminar duplicação. Nem todo tópico precisará de ficha independente se for contextualização, pré-requisito ou conteúdo teórico; cada tópico deverá terminar o projeto vinculado a uma ficha operacional, aula de apoio, contexto claramente identificado, ou justificativa de exclusão. Não ampliar o catálogo automaticamente a cada novo livro ou diretriz. Novos itens entram em lista de sugestões para a fase de refinamento.

## 2. Inventário exato do código, sem confundir conteúdo com planos
| Estrutura | Confirmado no código | Leitura correta |
|---|---:|---|
| Trilhas da biblioteca | 33 | Trilhas teóricas/de apoio, diferentes dos 28 módulos técnicos |
| Aulas da biblioteca | 115 | Aulas disponíveis; não são 115 procedimentos realizados |
| Duração estimada das aulas | 2.068 minutos | Estimativa de estudo cadastrada |
| Módulos técnicos | 28 | Categorias curriculares |
| Tópicos da matriz | 227 | Entradas planejadas; não equivalem a fichas concluídas |
| Procedimentos canônicos | 224 | IDs para reutilizar conhecimentos em vários módulos |
| Fichas procedimentais | 46 | 14 campos estruturais; 46 em revisão técnica no banco |
| Tópicos apenas catalogados | 181 | Aguardam cobertura prática ou contextual adequada |
| Relacionamentos aula ↔ módulo | 254 | Relações contextuais; não significam cobertura completa |
| Materiais do Atlas | 41 | 8 categorias e 158 variantes |
| Questões | 210 | Banco para avaliações de conhecimento |
| Casos | 30 | Casos situacionais/decisão |
| Flashcards | 137 | Revisão ativa |
| Planos de estudo | 3 | Percurso progressivo para biblioteca |
| Competências avaliadas | 28 | Competências cognitivas do banco |
| Checklists globais | 90 | 20 grupos de preparação/revisão, diferentes dos checklists das fichas |
| Vídeos externos | 9 | Links por trilha, ainda nenhum link individual nas 46 fichas |
| Referências do acervo | 72 | 41 com data de checagem no campo consultado |

**Indicadores de cobertura**: 46/227 = **20,3%** das entradas têm ficha; **21/28** módulos técnicos não têm ficha prática própria. Isso mede preenchimento editorial, não aptidão clínica. As 115 aulas devem continuar preservadas como biblioteca de apoio.

## 3. Inventário funcional: o que já é usável e o que falta
| Funcionalidade / rota | Estado | Evidência e limitação |
|---|---|---|
| Dashboard / `#/dashboard` | **Disponível** | Exibe progresso local, atalhos, áreas e conteúdo de destaque; alguns rótulos de meta e filtros visuais são ilustrativos. |
| Biblioteca / `#/biblioteca`, `#/modulo`, `#/aula` | **Disponível** | 33 trilhas, 115 aulas; marcação individual de conclusão. |
| Matriz técnica / `#/matriz-tecnica` | **Disponível como catálogo** | 28 módulos, 227 tópicos, busca, prioridade, relações e links; 181 ainda só catalogados. |
| Procedimentos / `#/procedimentos` | **Parcial** | 46 fichas com 14 campos; profundidade variável; nenhum vídeo integrado por ficha. |
| Atlas / `#/atlas` | **Parcial** | 41 materiais, 158 variantes, escalas e compatibilidades; figuras são esquemas simples, ainda falta atlas morfológico abrangente. |
| Busca global | **Disponível** | Busca por conteúdos, termos, códigos e aliases; não garante sinônimos clínicos em todas as especialidades. |
| Idiomas PT/ES | **Parcial** | 517 pares no dicionário; títulos 115/115, nomes e aberturas 46/46; 0/345 seções textuais de aulas e 0/210 perguntas com tradução direta detectada. |
| Fonte acessível A−/A+ | **Implementado estruturalmente** | Lógica 16/18/20/22 px, padrão 18 px e preferência local; medição visual real das páginas não feita nesta auditoria. |
| Planos / `#/planos` | **Disponível** | 3 percursos sobre as 115 aulas. |
| Flashcards / `#/flashcards` | **Disponível** | 137 cartões; marcar como dominado localmente. |
| Desafio rápido / `#/desafio` | **Disponível** | 5 questões sorteadas. |
| Simulado / `#/simulado` | **Disponível** | 20 questões sorteadas de 210, explicações e resultado. |
| Casos / `#/casos` e `#/caso` | **Disponível** | 30 casos situacionais com respostas. |
| Blueprint / `#/blueprint` | **Disponível** | Matriz de 28 competências e 210 questões. |
| Progresso / `#/progresso` | **Disponível localmente** | Conclusão de aulas, cartões, casos e histórico de simulados (últimas tentativas); sem conta/sincronização. |
| Remediação / `#/remediacao` | **Disponível** | Aulas de reforço a partir de respostas de simulado; depende das competências antigas. |
| Checklist / `#/checklist` | **Disponível** | 90 itens de revisão imprimíveis; não equivale a OSCE operacional validada. |
| Videoteca / `#/videoteca` | **Disponível, escopo reduzido** | 9 vídeos externos relacionados a 4 trilhas; sem cobertura individual do MB03. |
| Fontes / `#/fontes` | **Disponível** | 72 entradas de referência e créditos; vinculação por afirmação/procedimento ainda incompleta. |
| Roadmap / `#/roadmap` | **Disponível, desatualizado** | O próprio catálogo ainda descreve MB03 com 38 fichas e MB02 com 30 materiais; corrigir com sincronização central. |
| Login, contas, sincronização em nuvem | **Não implementado** | Não prometer. Dados de estudante permanecem no navegador via localStorage. |
| Editor administrativo de aulas e vídeos | **Não implementado** | Conteúdo editado em arquivos JavaScript; não há painel de gestão de conteúdo. |
| Montar bandeja, OSCE interativo, avaliação de gestos | **Planejado** | Não confundir checklists de texto e quiz com avaliação procedimental prática. |
| Certificação profissional ou autorização de procedimentos | **Fora de escopo** | Sistema educacional não certifica habilidade clínica. |

## 4. Cobertura de todos os 28 módulos técnicos
**Legenda:** ficha = roteiro de estudo MB03; não equivale a procedimento clinicamente certificado. Vínculo = ligação a aula antiga, independentemente de cobertura direta ou complementar.

| Módulo | Área | Tópicos | Fichas | Aulas relacionadas (vínculos) | Expansão congelada | Macrobloco principal |
|---|---|---:|---:|---:|---|---|
| M01 | Biossegurança | 8 | **1** | 11 | Higienização, EPI, campos estéreis e assepsia | MB03 |
| M02 | Instrumentação cirúrgica | 10 | **0** | 6 | Pinças, tesouras, bisturis, mesa e manuseio | MB03/MB04 |
| M03 | Agulhas, seringas e dispositivos | 10 | **0** | 15 | Agulhas, seringas, escalas e conexões | MB03 |
| M04 | Administração de medicamentos | 10 | **8** | 9 | Intradérmica, SC, IM, IV e infusão | MB03 |
| M05 | Acessos vasculares | 8 | **3** | 6 | Coleta, cateter periférico, central, PICC, arterial e intraósseo | MB03/MB05 |
| M06 | Feridas e lesões | 10 | **10** | 7 | Classificação, irrigação, curativos, mordeduras, desbridamento | MB03 |
| M07 | Suturas e fechamento | 11 | **11** | 5 | Fios, agulhas, pontos, nós, fechamento, grampos, adesivos | MB03/MB04 |
| M08 | Anestesia e analgesia | 10 | **0** | 9 | Anestesia local, sedação, bloqueios, anestesia geral e segurança | MB04 |
| M09 | Preparo cirúrgico | 11 | **0** | 17 | Preparo pré-operatório, pele, jejum, checklist e posicionamento | MB04 |
| M10 | Via aérea e oxigenoterapia | 9 | **0** | 13 | Oxigênio, BVM, dispositivos supraglóticos, IOT e via aérea difícil | MB05 |
| M11 | Procedimentos respiratórios | 6 | **0** | 10 | Gasometria, aspiração, toracocentese e drenos | MB05 |
| M12 | Emergências | 9 | **0** | 15 | RCP/DEA, hemorragia, estabilização, emergências | MB05 |
| M13 | Ortopedia e imobilização | 11 | **11** | 4 | Talas, gesso, tipóia, exame neurovascular, traumas | MB03 |
| M14 | Sondas e cateteres | 7 | **0** | 10 | Sonda vesical, nasogástrica, enteral, ostomias | MB05 |
| M15 | Procedimentos ambulatoriais | 5 | **0** | 5 | Abscesso, corpo estranho, unhas e pequenas biópsias | MB05 |
| M16 | Cirurgia geral | 8 | **0** | 15 | Incisão, dissecção, hemostasia, ligaduras, fechamento por planos e drenos | MB04 |
| M17 | Ginecologia e obstetrícia | 8 | **0** | 4 | Especular, coleta, DIU, técnicas obstétricas supervisionadas | MB05 |
| M18 | Pediatria e neonatologia | 7 | **0** | 10 | Dispositivos e acessos pediátricos, neonatologia | MB05 |
| M19 | Neurologia | 5 | **0** | 10 | Punção lombar e cuidados neurológicos | MB05 |
| M20 | Cardiologia | 7 | **0** | 7 | ECG, monitorização, cardioversão e desfibrilação | MB05 |
| M21 | Gastroenterologia | 7 | **0** | 15 | Paracentese, sondas e apoio em procedimentos digestivos | MB05 |
| M22 | Urologia | 6 | **0** | 10 | Cateterismos, irrigação vesical e procedimentos urológicos | MB05 |
| M23 | Oftalmologia | 7 | **0** | 0 | Irrigação ocular, fluoresceína e exame básico | MB05 |
| M24 | Otorrinolaringologia | 6 | **0** | 4 | Otoscopia, epistaxe, lavagem e corpos estranhos | MB05 |
| M25 | Dermatologia | 7 | **0** | 5 | Biópsias, crioterapia e exéreses selecionadas | MB05 |
| M26 | Cuidados pós-operatórios | 10 | **0** | 14 | Curativos, drenos, SRPA e vigilância de complicações | MB04 |
| M27 | Diagnóstico à beira-leito | 6 | **2** | 11 | Glicemia, ECG, coleta, POCUS e punções diagnósticas | MB03/MB05 |
| M28 | Documentação e comunicação | 8 | **0** | 7 | Consentimento, registro e transferência estruturada | MB04/MB08 |

**Distorções que precisam ser corrigidas em interface**: M16 (Cirurgia geral) está categorizado como “Base existente” porque tem relações de aulas, mas tem **0 de 8** fichas; não se pode exibir “coberto” sem separar aula de suporte e treino da técnica. M06/M07/M13 têm 100% dos tópicos atuais com fichas, mas a profundidade e multimídia permanecem parciais.

## 5. Diagnóstico de completude das 46 fichas e do Atlas
Fichas com vínculo de material: **35/46**; sem vínculo de Atlas **11/46** (o procedimento pode conter itens em texto, mas ainda precisa de relação estruturada). Referências associadas às fichas: **74 vínculos**; vídeos nas fichas: **0**. Etapas no campo `sequence`: **4 a 7**, média **4.46**; não usar esse número como medida de qualidade.

Critério de “ficha útil para o estudo prático”: indicação e contraindicação, materiais com variantes, anatomia relevante, preparo e posição do paciente, sequência técnica concisa com pontos de parada, confirmação, complicações, pós-procedimento, referência rastreável, checklist de simulação e demonstração audiovisual externa **quando existir fonte apropriada**. Manter esquema de 14 campos no banco; condensar a experiência de leitura em 6–8 painéis operacionais. Não copiar textos ou imagens dos cinco livros protegidos. A aprendizagem digital não substitui supervisão presencial.

**Atlas**: 41 materiais/158 variantes, categorizados em: Dispositivos vasculares (5), Infusão e conexões (4), Seringas e acesso medicamentoso (3), Sondas e drenagem (4), Via aérea e oxigenação (3), Fechamento e suturas (8), Instrumentais cirúrgicos (9), Imobilização, talas e gessos (5). Os desenhos são esquemas didáticos; para reconhecimento morfológico de instrumentos são necessárias ilustrações próprias específicas.

## 6. Escopo dos oito macroblocos — manter e concluir, sem abrir um nono
| MB | Situação real | Entrega restante / critério de aceite |
|---|---|---|
| MB01 — Matriz curricular | Estrutura entregue | Preservar os 227 tópicos e 224 canônicos. Corrigir no roadmap as contagens e separar relação didática de cobertura prática. |
| MB02 — Atlas de materiais | Núcleo inicial entregue | 41 materiais/158 variantes existentes. Crescer sob demanda das fichas; validar escalas/compatibilidades e substituir ícones genéricos por desenhos específicos quando isso for necessário para aprender. |
| MB03 — Procedimentos fundamentais | Em desenvolvimento / 46 fichas | Finalizar lacunas fundamentais P0 e conexão com Atlas; assegurar roteiro de como fazer, checklist e pontos críticos; 181 tópicos ainda catalogados pertencem ao conjunto MB03–MB05 e não só ao MB03. |
| MB04 — Cirurgia e anestesia | A iniciar | Atacar M16 (0/8), M08 (0/10), M09 (0/11) e M26 (0/10), integrando preparo, técnica e recuperação; sem criar aulas genéricas duplicadas. |
| MB05 — Emergência e especialidades | Planejado | Completar sondas, via aérea, drenagens, RCP, punções e técnicas das especialidades P1/P2 conforme indicação e competência. |
| MB06 — Videoteca por procedimento | Planejado | Curadoria de links por ficha/tema, autoria, idioma, status do link, créditos e data, sem hospedar vídeo de terceiros. |
| MB07 — Treinamento e avaliação prática | Planejado | Bandejas interativas, sequenciamento da técnica e checklists OSCE para simulação; sem alegar certificação. |
| MB08 — Consolidação final | Planejado | Revisão da consistência bibliográfica e conteúdo, tradução PT/ES completa, QA visual/acessibilidade, segurança, direitos autorais, redundâncias e publicação. Revisão externa não é condição para estudar e não deve bloquear fichas; conteúdo não deve ser rotulado como protocolo certificado. |

## 7. Regras operacionais para evitar expansão sem fim
1. **Escopo congelado:** 28 módulos e 227 tópicos são a base v1. Novos capítulos de livros entram em `BACKLOG_PÓS-MB08`, salvo lacuna crítica de segurança ou erro de precisão.
2. **Uma ficha canônica por procedimento**; reutilizar relações entre especialidades e cenários, sem copiar textos em módulos diferentes.
3. **Não confundir entregas:** nova rota/funcionalidade somente com objetivo curricular identificado, usuário-alvo, critério de aceite e indicação do MB responsável.
4. **Diferenças de progresso devem ser visíveis:** `catalogado`, `ficha disponível`, `ficha com materiais completos`, `mídia vinculada`, `traduzido` e `QA conferido`. Não anunciar apenas “% concluído” sem numerador e denominador.
5. **Nenhuma aprovação externa para liberar estudo:** conteúdo será sempre acessível e atualizado editorialmente; especificar fontes/datas, sem classificar ferramenta como treinamento clínico autônomo.
6. **Sem pular regressão:** antes/depois contar trilhas, aulas, questões, fichas, materiais, tópicos, links e idiomas; comparar arquivos; correr `npm run qa:all`, conferindo no navegador real quando possível.
7. **Toda entrega:** resumo do que mudou, pontos críticos, GitHub commit e Vercel deploy, ZIP backup, status do MB e único próximo passo.
8. **Refinamento ao final do MB08:** organização visual definitiva, perfis/sincronização (se necessário), expansão de especialidades e melhorias experimentais ficam nesta fase posterior, não interrompem o roadmap.

## 8. Pendências prioritárias e decisão antes de novos lotes
| Severidade | Falha | Encaminhamento |
|---|---|---|
| Crítica de conteúdo | M16 Cirurgia Geral sem ficha, M08 Anestesia sem ficha, M10 Via aérea sem ficha | MB04 e MB05 na ordem já prevista |
| Alta | 21 módulos sem ficha própria; 181 tópicos só catalogados | Concluir o escopo por procedimentos, com metas reais e sem multiplicar aulas teóricas |
| Alta | PT/ES parcial: títulos traduzidos, conteúdo principal não | Tradução incremental completa ao longo de MB04–MB08 |
| Alta | 0 vídeos por ficha prática | MB06; ligação explícita, crédito e checagem técnica |
| Média | Leitura interna não validada em navegador real | QA visual desktop/celular no próximo ciclo de integração |
| Média | 11 fichas sem vínculo material estruturado | Atlas atualizado junto da ficha, sem obrigação de inventar materiais |
| Média | Roadmap em código e documentos com contagens 38/30 antigas | Synchronizar a tela Roadmap com contagens geradas dinamicamente do banco |
| Média | 92 alertas editoriais existentes no banco de questões | Revisão por criticidade no MB07; não tratar como 92 erros confirmados |
| Média | Não há painel de edição/admin, autenticação nem sincronização entre dispositivos | Fora do escopo imediato; considerar depois do MB08 se houver necessidade real |

## 9. Validação realizada para este inventário
- Repositório GitHub `eradinho-max/Nexo-Cirurgico`, branch `main`, commit `aaced6139a3ad90de44b1cbd48fff4636e0516ed` conferido; deploy Vercel vinculado ao mesmo commit reportou `READY`.
- O arquivo local `NEXO_CIRURGICO_V145_SOURCE_2026-10-15.tar.gz` possui Git blob SHA `387cfcccde7d98a86c3d04751bcf5062d976e2cd`, correspondente ao blob do projeto versionado no repositório; assim, a contagem provém do código da produção, não de documentação antiga.
- Extração da estrutura `window.NEXO_DATA` e `window.NEXO_PROCEDURES` diretamente dos arquivos JS; verificação dos IDs e status. `npm run qa:all` executado localmente com código de saída 0; QA afirmações estruturais e build. Não foi inspecionada nesta rodada a experiência em dispositivo real, tampouco auditado cada enunciado clinicamente.
- Os cinco livros enviados orientam o backlog por técnicas: Tapia Jurado, Myers & Hale, Manual FMUSP, Manual de terapêutica/urgências e Medicina de Emergência 19ª (2025). Conteúdo autoral do projeto; nenhuma reprodução integral de PDFs/figuras. A existência de livro não garante atualidade de recomendações, sobretudo nas edições antigas.

## 10. Decisão de continuidade
**Não iniciar funcionalidades novas nesta rodada de inventário.** A próxima entrega de implementação é **MB04, Lote 1 — núcleo cirúrgico operacional (M16, mais integração M02/M09)**, acompanhada da correção da tela de Roadmap para que ela apresente números reais calculados do código. Em seguida MB04 anestesia, e MB05 urgências/especialidades conforme a mesma matriz. No fechamento do MB08, executar auditoria de refinamento global e decidir eventual expansão pós-escopo.

**Backup da base analisada (SHA-256):** `aadcb3c3fcda6ea43724789f820fcbbfd39f94a164d1384b53491eb4aa4691e7`.