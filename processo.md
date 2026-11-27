# Processo de trabalho — Caderneta Digital do Coordenador de Turno

**Disciplina:** Engenharia de Software I — Lab #02, ISPTEC (2026/2027)  
**Versão:** 0.1 — proposta de acordo de trabalho a aprovar pelo grupo.  
**Período:** 24/11/2026 a 13/12/2026.

Este ficheiro define como a equipa pretende trabalhar. Os acontecimentos, resultados, contribuições e métricas reais ficam registados em `sprints/sprint-N.md`. Não se devem apresentar propostas como decisões já tomadas nem criar evidências retroactivas.

## 1. Valores do grupo (Actividade 1)

Com base no Manifesto Ágil [1], propomos as seguintes decisões:

| Valor privilegiado | Decisão concreta para o projecto | O que continua a ter valor |
|---|---|---|
| Pessoas e comunicação | Realizar uma Daily Scrum e ajudar colegas a resolver impedimentos. | Git, GitHub Projects e regras de colaboração. |
| Software funcional | Demonstrar um incremento executável em cada Sprint Review. | Requisitos, diagramas, testes e documentação exigida. |
| Colaboração com o cliente | Esclarecer dúvidas com o coordenador e mostrar o produto em cada Sprint. | Registo dos pedidos, critérios de aceitação e decisões. |
| Adaptação à mudança | Actualizar o Product Backlog após feedback, sem comprometer o Sprint Goal. | Planeamento das Sprints, prioridades e prazo de entrega. |

Privilegiar a entrega funcional não significa abandonar a documentação. Produzimos apenas a documentação necessária, incluindo os entregáveis académicos, e mantemo-la actualizada com o software. Aplicamos também os princípios de entrega frequente, colaboração, qualidade técnica, simplicidade, ritmo sustentável e melhoria contínua [1].

## 2. Equipa (Actividade 2)

A Scrum Team é responsável pelo produto como um todo. Preencher os nomes reais e ajustar as linhas à dimensão do grupo antes de aprovar este documento.

| Membro | Responsabilidade | Tarefas concretas |
|---|---|---|
| Delfina Ramos | Product Owner | Gerir e ordenar o Product Backlog, esclarecer requisitos com o coordenador e maximizar o valor do produto. |
| Gustavo Guenge | Scrum Master | Ajudar a aplicar Scrum, facilitar eventos quando necessário, apoiar a remoção de impedimentos e a melhoria do fluxo. |
| Evandro Eusébio, Arquimedes Alexandre | Developers | Planear a Sprint, desenvolver, testar, integrar, rever código e adaptar diariamente o plano de trabalho. |
|---|---|---|

Neste contexto académico, quem assume Product Owner ou Scrum Master pode também participar na implementação, assumindo nesse trabalho a responsabilidade de Developer. Todos os membros devem contribuir para o produto, os testes, a documentação e as revisões;

## 3. Eventos (Actividade 3)

As durações locais abaixo são propostas adaptadas às Sprints de quatro dias reais determinadas pelo enunciado.

| Evento | Propósito | Participantes | Limite oficial (Sprint de um mês) | Duração proposta | Resultado |
|---|---|---|---|---|---|
| Sprint | Transformar ideias em valor e progredir para o Product Goal. | Scrum Team | Um mês ou menos | 4 dias reais | Incremento funcional. |
| Sprint Planning | Definir porquê, o quê e como trabalhar. | Scrum Team | Até 8 horas | 30–45 min, dia 1 | Sprint Goal e Sprint Backlog. |
| Daily Scrum | Inspeccionar progresso para o Sprint Goal e adaptar o plano. | Developers; PO/SM se estiverem a trabalhar como Developers | 15 min | 10–15 min, diariamente | Plano adaptado e impedimentos identificados. |
| Sprint Review | Inspeccionar o resultado e decidir adaptações futuras. | Scrum Team e stakeholders relevantes | Até 4 horas | 20–30 min, dia 4 | Feedback e actualização do Product Backlog. |
| Sprint Retrospective | Melhorar a qualidade e a eficácia da equipa. | Scrum Team | Até 3 horas | 15–20 min, dia 4 | Acções de melhoria concretas. |

**Justificação:** Como cada Sprint representa duas semanas simuladas em quatro dias reais, os eventos serão curtos e focados. Quando não for possível uma Daily síncrona, cada Developer pode escrever uma actualização e a equipa deve inspeccionar conjuntamente o progresso e adaptar o plano nesse dia, conforme a adaptação pedagógica permitida. Review e Retrospective podem ocorrer na mesma sessão, mantendo propósitos e registos separados.

O refinamento do Product Backlog será realizado sempre que necessário, em pequenas conversas durante a Sprint; 

## 4. Objectivo do Produto e Definição de Pronto (Actividade 4)

### 4.1. Objectivo do Produto (Product Goal)

Disponibilizar uma Caderneta Digital segura, responsiva e acessível que permita ao coordenador de turno gerir turmas e alunos, registar ocorrências envolvendo vários alunos, registar as medidas aplicadas e consultar o histórico individual do aluno.


### 4.3. Artefactos e compromissos

| Artefacto | Compromisso | Aplicação no projecto |
|---|---|---|
| Product Backlog | Product Goal | Lista de Issues ordenadas na vista Lista do produto. |
| Sprint Backlog | Sprint Goal | Objectivo, Issues seleccionadas e plano dos Developers, visíveis na vista Sprint actual e no ficheiro da Sprint. |
| Incremento | Definition of Done | Versão funcional integrada, que respeita os critérios de qualidade e é marcada no fim da Sprint com `sprint-N`. |


### 4.4. Definition of Done — Definição de Pronto (DoD)

Uma Issue só será considerada concluída quando satisfizer as condições aplicáveis:

- [ ] Todos os critérios de aceitação foram satisfeitos.
- [ ] O trabalho está num ramo associado à Issue, com commits claros.
- [ ] As validações, a segurança e a acessibilidade necessárias foram respeitadas.
- [ ] Os testes aplicáveis foram executados com sucesso.
- [ ] Existe um Pull Request associado à Issue, revisto por outro membro.
- [ ] Os problemas identificados na revisão foram resolvidos.
- [ ] O trabalho foi integrado na `main` e a versão integrada foi verificada.
- [ ] A documentação necessária foi actualizada.
- [ ] A Issue foi encerrada e o estado no quadro está correcto.



## 5. Regras do quadro (Actividade 5)

### 5.1. As três práticas do Kanban

Segundo o Kanban Guide de Dezembro de 2020 [3], o grupo deve:

| Prática | Aplicação concreta |
|---|---|
| Definir e visualizar o fluxo | Utilizar as colunas do GitHub Projects e explicitar regras, início, fim, limites e expectativa de serviço. |
| Gerir activamente os itens | Respeitar o WIP, acompanhar a idade dos itens, resolver bloqueios e dar prioridade à conclusão. |
| Melhorar o fluxo | Analisar métricas, ajustar políticas e identificar melhorias nas Dailies e retrospectivas. |

### 5.2. Colunas e políticas

| Coluna | Significado | Regra para avançar | Limite inicial (produto) |
|---|---|---|---:|
| Backlog | Trabalho não seleccionado para a Sprint. | O item é ordenado, esclarecido e seleccionado. | — |
| A fazer | Trabalho seleccionado, ainda não iniciado. | Existem capacidade, critérios claros e dependências satisfeitas. | — |
| Em curso | Implementação ou execução iniciada. | Alterações prontas para revisão; Pull Request criado. | 2 |
| Em revisão | Outro membro está a avaliar o trabalho. | Revisão concluída, correcções feitas e aprovação segundo a regra do grupo. | 1 |
| Concluído | Trabalho integrado e validado conforme a DoD. | Estado final. | — |

- **Início do fluxo medido:** entrada em Em curso pela primeira vez.
- **Fim do fluxo medido:** entrada em Concluído após satisfação da DoD.
- Se houver erros na revisão ou nos testes, corrigir o item antes de o concluir. Se precisar de regressar a Em curso, respeitar a capacidade ou registar uma excepção explícita, sem iniciar trabalho novo.
- Quando uma coluna está cheia, ajudar a concluir o trabalho dessa etapa em vez de iniciar novos itens.



### 5.3. Issues de processo em paralelo

As Issues D02–D06 são registos do ciclo completo da respectiva Sprint, não funcionalidades. Permanecem em andamento durante o ciclo e são acompanhadas numa vista separada, com etiqueta `processo`. O responsável pelo registo pode alternar diariamente; todos participam nos eventos.

Para manter o limite de desenvolvimento útil, propomos medir separadamente o fluxo do produto e o acompanhamento de processo. O fluxo principal inclui as Issues T01–T30 e os itens de documentação do produto que efectivamente percorrem as etapas de execução, revisão e testes aplicáveis. As Issues D01–D10 devem ser explicitamente identificadas na análise: por simplicidade, a medição principal proposta usa apenas T01–T30; pode ser apresentada uma contagem complementar das Dxx.


### 5.4. Sistema Pull e expectativa de serviço (SLE)

Os Developers puxam o próximo item prioritário disponível quando há capacidade. Antes de iniciar outro, verificam os itens já em revisão, em testes ou bloqueados. Um responsável pode receber ajuda de outros integrantes.

Como ainda não existem dados históricos confirmados, a expectativa inicial proposta é concluir 85% dos itens do fluxo de produto em até 2 dias reais, desde o início até à conclusão. Trata-se de uma hipótese a validar, não de uma garantia nem de um resultado medido. Rever após recolher tempos de ciclo e dividir itens demasiado grandes.

### 5.5. Configuração do GitHub Projects

| Campo | Valores |
|---|---|
| Status | Backlog, A fazer, Em curso, Em revisão, Concluído |
| Priority | P0, P1, P2, P3 |
| Iteration | Sprint 1 a Sprint 5, com as datas do calendário |
| Assignees | Membros que executam o item |
| Module | Setup, Autenticação, Turmas/Alunos, Ocorrências, Medidas, Histórico, Qualidade, Extensões, Processo |
| Start Date / End Date | Datas de início e conclusão do item; guardar hora em registo complementar para métricas em horas |

Etiquetas sugeridas: `mvp`, `setup`, `enhancement`, `documentation`, `testing`, `processo`, `blocked`.

Vistas obrigatórias: **Lista do produto** (todas as Issues ordenadas) e **Sprint actual** (Issues da iteração em curso). Vistas adicionais propostas: Desenvolvimento e Scrum/documentação, com filtros por etiqueta ou módulo.

O repositório e o quadro devem ser públicos, a conta `judsonp` deve ser convidada com permissão Write no quadro, e a visibilidade deve ser testada numa janela anónima. 

- Repositório: [Adicionar link real]
- GitHub Projects: [Adicionar link real]

## 6. Desafio a vigiar (Actividade 6)

A revisão de literatura de Ahmad, Markkula e Oivo (2013) [4] identifica benefícios e dificuldades da adopção do Kanban.

| Tipo | Resultado relatado no estudo | Aplicação ao projecto |
|---|---|---|
| Benefício | Menor tempo de entrega do software. | Acompanhar o tempo de ciclo e reduzir períodos de espera. |
| Benefício | Melhor comunicação e coordenação. | Tornar o trabalho visível e resolver dependências em conjunto. |
| Desafio | Conhecimento e formação insuficientes. | Ler os guias e praticar as regras do quadro em conjunto. |
| Desafio | Dificuldades organizacionais na adopção. | Acordar responsabilidades, prioridades e políticas claras. |

**Desafio inicial proposto:** falta de experiência prática na gestão do fluxo, que pode levar a iniciar demasiadas tarefas e acumular Pull Requests em revisão.

**Acções:** respeitar os limites de WIP, verificar bloqueios diariamente, rever Pull Requests antes de iniciar trabalho novo e dividir Issues demasiado grandes. Na retrospectiva, analisar o WIP máximo, a idade dos itens e o tempo de ciclo para perceber se as acções ajudaram.

| Sprint | Observação real | Acção de melhoria | Resultado na Sprint seguinte |
|---|---|---|---|
| 1 | [Preencher na retrospectiva] | [Preencher] | [Preencher] |
| 2 | [Preencher na retrospectiva] | [Preencher] | [Preencher] |
| 3 | [Preencher na retrospectiva] | [Preencher] | [Preencher] |
| 4 | [Preencher na retrospectiva] | [Preencher] | [Preencher] |
| 5 | [Preencher na retrospectiva] | [Preencher] | [Não aplicável ou aprendizagem futura] |

A secção deve ser actualizada em todas as retrospectivas. A síntese do estudo baseia-se no resumo publicado e no manuscrito disponibilizado pelos autores; cada integrante deve consultar o artigo indicado pelo professor.

## 7. Como combinamos o Scrum e o Kanban (Actividade 7)

| Aspecto | Scrum | Kanban |
|---|---|---|
| Ritmo de trabalho | Ciclos fixos com objectivo e eventos; incrementos podem ser disponibilizados durante a Sprint. | Fluxo contínuo com controlo da capacidade; não exige Sprints. |
| Responsabilidades | Product Owner, Scrum Master e Developers. | Não impõe novas responsabilidades específicas. |
| Mudanças durante o ciclo | O plano pode ser adaptado sem colocar em risco o Sprint Goal; o escopo é renegociado com o PO quando necessário. | Novos itens são puxados conforme prioridade, políticas e capacidade. |
| Medidas | Progresso para os objectivos e qualidade do incremento; não prescreve Story Points ou velocidade. | WIP, Throughput, Work Item Age e Cycle Time. |

O Scrum será utilizado para organizar as cinco Sprints, definir objectivos e recolher feedback. O Kanban será utilizado para gerir o fluxo de Issues dentro das Sprints, controlar o trabalho em curso e identificar impedimentos. As métricas apoiarão a adaptação do plano na Daily e a melhoria do processo na Retrospective, conforme o guia de Kanban para Scrum Teams [5].

## 8. Ferramentas (Actividade 7)

| Ferramenta | Finalidade | Evidência prevista |
|---|---|---|
| Git | Versionamento e colaboração em ramos. | Commits, ramos, histórico e etiquetas. |
| GitHub | Repositório, Issues, Pull Requests e revisões. | Links e histórico de contribuições. |
| GitHub Projects | Product Backlog, Sprints e Kanban. | Vistas, estados, prioridades e imagens do quadro. |
| ChatGPT | Apoio na compreensão dos conceitos, revisão e estruturação de requisitos. | Declaração de uso de IA e verificação das respostas. |
| [Ferramenta de desenvolvimento] | [Confirmar linguagem/framework e justificação] | [Código e instruções no README] |
| [Armazenamento] | [Confirmar base de dados ou ficheiros e justificação] | [Modelo e execução local] |
| [Ferramenta de prototipagem, se utilizada] | [Confirmar e justificar] | [Protótipos reais] |

O WhatsApp e a aula são os canais previstos no enunciado para dúvidas e demonstrações ao coordenador. Se forem acrescentadas outras ferramentas, devem funcionar, ser utilizadas por todos os membros, ter evidência no relatório e ser justificadas nesta secção.

## 9. Regras de uso da IA (Actividade 8)

1. Consultar primeiro o enunciado e os guias oficiais quando houver dúvidas sobre o processo.
2. Usar IA como apoio, não como substituto da análise, implementação, revisão ou validação humana.
3. Verificar o código gerado, executar testes e confirmar as afirmações com fontes fiáveis.
4. Garantir que cada integrante consegue explicar sozinho o código e o relatório.
5. Não enviar dados pessoais reais nem segredos à IA.
6. Declarar no relatório a ferramenta, finalidade e partes em que foi utilizada.
7. Nunca inventar reuniões, feedback, testes, métricas, commits ou revisões.

### 9.1. Verificação de uma resposta de IA

A actividade pede que a equipa pergunte a uma IA: **«Quais são os papéis do Scrum e os seus eventos?»**, guarde a resposta e a compare com o Scrum Guide 2020 [2].

- Ferramenta: ChatGPT (ou outra escolhida pelo grupo).
- Data da consulta: [Preencher com data real].
- Pergunta: Quais são os papéis do Scrum e os seus eventos?
- Resposta obtida: [Colar a resposta real, sem a alterar].
- Diferença, omissão ou termo desactualizado: [Identificar na resposta real].
- Secção do Scrum Guide: [Indicar a secção que fundamenta a análise].

**Exemplo de verificação, não apresentado como resultado já realizado:** se a IA afirmar que existem apenas quatro eventos, a resposta está incompleta, porque a Sprint é também um evento e contém os outros quatro. Se usar apenas o termo «papéis», comparar com as responsabilidades definidas na secção Scrum Team. A equipa deve identificar uma diferença que esteja efectivamente presente na resposta obtida.

### 9.2. Registo de utilização de IA

| Ferramenta | Finalidade | Parte do trabalho | Verificação |
|---|---|---|---|
| ChatGPT | Estruturar o backlog, requisitos e acordo de trabalho | `docs/requisitos.md`, `processo.md` e propostas de Issues | [Registar revisão e validação real pelo grupo] |
| [Preencher] | [Preencher] | [Preencher] | [Preencher] |

## 10. Calendário e plano inicial das Sprints

As datas são obrigatórias; os objectivos e Issues constituem uma previsão a confirmar em cada Sprint Planning.

| Sprint | Dias reais | Semanas simuladas | Objectivo sugerido | Issues de produto sugeridas | Processo |
|---|---|---|---|---|---|
| 1 | 24–27/11/2026 | 1: 24–25/11; 2: 26–27/11 | Preparação | T01–T08 | D01, D02 |
| 2 | 28/11–01/12/2026 | 3: 28–29/11; 4: 30/11–01/12 | Autenticação, Turmas, alunos e ocorrências | T09–T13 | D03 |
| 3 | 02–05/12/2026 | 5: 02–03/12; 6: 04–05/12 | Medidas, consulta de ocorrências e histórico | T14–T17 | D04 |
| 4 | 06–09/12/2026 | 7: 06–07/12; 8: 08–09/12 | Validar e estabilizar o MVP | T18–T20 | D05, D07 |
| 5 | 10–13/12/2026 | 9: 10–11/12; 10: 12–13/12 | Entrega, publicação e extensões se houver capacidade | T30 e selecção de T21–T29 | D06, D08–D10 |

Os testes, a acessibilidade, a documentação e as evidências são trabalhos contínuos. A Sprint 4 concentra a validação integrada, não o início dos testes. D08 e D09 começam a ser preparados desde a primeira Sprint. Cada Issue seleccionada deve ter a iteração real atribuída no quadro. Não alterar artificialmente as datas dos registos para corresponder ao plano.

## 11. Fluxo diário de trabalho

### Primeiro dia de cada Sprint

- Realizar a Sprint Planning, definir o Sprint Goal e seleccionar Issues conforme capacidade e dependências.
- Actualizar as Issues no GitHub Projects, definir a iteração e o estado A fazer.
- Criar ou actualizar `sprints/sprint-N.md` com o planeamento, através de Pull Request no próprio dia.
- Realizar a Daily Scrum para organizar o trabalho e iniciar a execução.

### Todos os dias

| Momento | Actividade | Resultado esperado |
|---|---|---|
| Início | Daily Scrum (10–15 min). | Progresso, plano e impedimentos identificados. |
| Início | Registar a Daily através de PR e consultar o quadro. | Evidência diária e estados actualizados. |
| Durante | Continuar trabalho iniciado ou puxar uma Issue prioritária. | WIP respeitado. |
| Durante | Trabalhar num ramo, fazer commits, testar e enviar alterações. | Progresso visível no GitHub. |
| Durante | Abrir e rever Pull Requests; ajudar nos bloqueios. | Código revisto e integração facilitada. |
| Durante | Validar critérios, integrar e verificar a versão final. | Issues concluídas conforme a DoD. |
| Final | Confirmar que quadro, registos e PRs reflectem o estado real. | Evidências actualizadas no próprio dia. |

As três perguntas sugeridas para a Daily são: o que fiz desde a última Daily, o que farei hoje e que impedimentos tenho. A reunião serve para adaptar o plano em relação ao Sprint Goal, não para prestar contas ao Scrum Master.

### Final de cada semana simulada (dias 2 e 4)

Guardar o resumo da evolução do grupo e os links reais de commits, Issues, Pull Requests e revisões. Deve existir progresso verificável no GitHub em cada uma das dez semanas simuladas.

## 12. Fluxo de uma Issue com Git e GitHub

`Backlog → A fazer → Em curso → Em revisão → Em testes → Concluído`

1. Seleccionar uma Issue disponível, atribuir responsável e actualizar para Em curso.
2. Actualizar a `main` local e criar um ramo associado ao número real da Issue.
3. Implementar e testar a funcionalidade, com commits claros.
4. Enviar o ramo para o GitHub e abrir um Pull Request.
5. Outro integrante realiza uma revisão. Corrigir os problemas identificados.
6. Executar a validação final, integrar na `main` e verificar a versão integrada.
7. Confirmar a DoD, o encerramento da Issue e o estado Concluído no quadro.

Exemplo para a Issue **#9** (substituir pelo número real):

```bash
git switch main
git pull origin main
git switch -c feature/9-gestao-turmas
# Implementar e testar a funcionalidade
git add .
git commit -m "feat: implementar cadastro de turmas"
git push -u origin feature/9-gestao-turmas
```

Modelo de descrição do Pull Request:

```markdown
## Alterações realizadas
- [Descrever alterações reais]

## Testes realizados
- [Descrever testes e resultados reais]

Closes #9
```

O `Closes #9` fecha a Issue quando o PR é integrado no ramo padrão, desde que a ligação seja reconhecida pelo GitHub. Só utilizar o fecho quando os critérios estiverem satisfeitos. Se a verificação após o merge falhar, reabrir a Issue e corrigir o problema.

Para registos intermédios da Sprint, usar `Refs #n` e ramos como `docs/sprint-2-dia-1`, mantendo a Issue de acompanhamento aberta. O último PR deve fechar a Issue quando todos os critérios registáveis no PR estiverem cumpridos; confirmar a etiqueta e as restantes evidências no encerramento e corrigir o estado caso falte alguma condição. O número real do GitHub deve substituir `n`.

### Regras de colaboração

- Não implementar directamente na `main` nem integrar PR próprio sem revisão de outro integrante.
- Não iniciar trabalho novo se houver bloqueios que possam ser resolvidos em conjunto.
- Preferir PRs pequenos, com alterações e testes descritos.
- Cada membro deve realizar pelo menos uma contribuição relevante e uma revisão de código por Sprint, registando os links.
- Classificar os comentários das revisões (defeitos, legibilidade, alternativas, partilha de conhecimento) para a actividade 11; comparar os resultados reais com Bacchelli e Bird (2013) [6].

## 13. Encerramento de cada Sprint

No quarto dia real de cada Sprint:

- [ ] Confirmar que existe uma versão funcional e testada.
- [ ] Realizar Sprint Review e demonstrar o incremento ao coordenador na aula ou por imagens/vídeo de 1–2 minutos no WhatsApp.
- [ ] Registar feedback recebido; na sua ausência, registar que o Product Owner representou o coordenador.
- [ ] Actualizar o Product Backlog conforme as decisões e reconsiderar os itens não concluídos.
- [ ] Calcular as medidas de fluxo com dados reais.
- [ ] Realizar Sprint Retrospective e definir melhorias concretas.
- [ ] Actualizar o desafio a vigiar e as regras do `processo.md`, quando aplicável.
- [ ] Registar as contribuições e revisões de todos os membros.
- [ ] Guardar as imagens do quadro e os links das evidências.
- [ ] Integrar os registos da Sprint através dos respectivos PRs, no próprio dia.
- [ ] Criar e enviar a etiqueta Git da Sprint no último commit.
- [ ] Actualizar a versão publicada, se existir, e confirmar o encerramento da Issue de processo.

Exemplo de etiqueta para a Sprint 2:

```bash
git switch main
git pull origin main
git tag sprint-2
git push origin sprint-2
```

A etiqueta identifica o último commit da Sprint após integração dos registos. Não a mover para simular uma entrega anterior.

## 14. Medidas de fluxo do Kanban

Usar as quatro medidas definidas no Kanban Guide [3]. O enunciado exige, em cada Sprint, o WIP máximo atingido, o débito, a idade do item mais antigo ainda em curso e o tempo de ciclo de três Issues concluídas.

| Métrica | Como calcular |
|---|---|
| WIP máximo | Maior número simultâneo de itens iniciados e ainda não concluídos durante a Sprint, incluindo revisão, testes e bloqueados. |
| Throughput (débito) | Número de itens que entraram em Concluído durante a Sprint. |
| Work Item Age | Tempo decorrido desde o início do item mais antigo ainda não concluído, até ao instante de medição. |
| Cycle Time | Tempo decorrido entre o primeiro início e a conclusão efectiva de cada item, incluindo esperas. |

Registar as mudanças de estado e respectivas datas/horas para conseguir reconstruir o WIP máximo e calcular os tempos. Contar tempo corrido em horas ou dias reais, sem misturar com semanas simuladas.

Modelo a preencher em cada `sprints/sprint-N.md`:

| Métrica | Resultado real | Evidência |
|---|---|---|
| WIP máximo | [Preencher] | [Link/registo] |
| Throughput | [Preencher] | [Link/registo] |
| Idade do item mais antigo | [Issue e idade] | [Link/registo] |

| Issue concluída | Data/hora de início | Data/hora de conclusão | Cycle Time |
|---|---|---|---|
| [#n] | [Preencher] | [Preencher] | [Preencher] |
| [#n] | [Preencher] | [Preencher] | [Preencher] |
| [#n] | [Preencher] | [Preencher] | [Preencher] |

Acrescentar um parágrafo sobre o significado das métricas, as dificuldades observadas e a melhoria a experimentar. Se não houver itens em andamento, a idade é não aplicável. Se houver menos de três itens concluídos, registar todos os disponíveis e explicar a limitação. Não inventar valores.

## 15. Organização da documentação e evidências

```text
caderneta-digital/
├── docs/
│   ├── requisitos.md
│   ├── casos-de-uso.png
│   ├── modelo-de-dados.png
│   └── prototipos/
├── sprints/
│   ├── sprint-1.md
│   ├── sprint-2.md
│   ├── sprint-3.md
│   ├── sprint-4.md
│   └── sprint-5.md
├── processo.md
├── README.md
└── [codigo da aplicacao]
```

| Informação | Local |
|---|---|
| Regras do grupo e decisões do processo | `processo.md` |
| Requisitos e critérios de aceitação | `docs/requisitos.md` e GitHub Issues |
| Product Backlog e Sprint Backlog | GitHub Projects |
| Planeamento, Daily, Review, Retrospective e métricas | `sprints/sprint-N.md` |
| Contribuições, revisões e evolução | Commits, PRs, Issues e links no ficheiro da Sprint |
| Incremento de cada Sprint | Etiqueta Git `sprint-N` |
| Instalação, manual de utilização e relatório de testes | `README.md` |

Todos os eventos devem ser registados no próprio dia por Pull Request. O relatório final deve incluir os resultados das 14 actividades, um capítulo por Sprint dividido pelas duas semanas simuladas, imagens das evidências, reflexão final, referências e declaração de uso de IA.

**Prazo de entrega:** 13/12/2026, às 23h59. Seguir o formato de nome do PDF e assunto do e-mail indicado no enunciado, substituindo turma e grupo pelos dados reais. A preparação do relatório não substitui o registo contínuo da evolução no GitHub.

## 16. Referências

1. BECK, K. et al. *Manifesto para o Desenvolvimento Ágil de Software* (2001). [Valores](https://agilemanifesto.org/iso/ptpt/manifesto.html) e [princípios](https://agilemanifesto.org/iso/ptpt/principles.html).
2. SCHWABER, K.; SUTHERLAND, J. *The Scrum Guide* (2020). [Scrum Guides](https://scrumguides.org/scrum-guide). Secções Scrum Team, Scrum Events e Scrum Artifacts.
3. VACANTI, D.; COLEMAN, J. *The Kanban Guide* (Dezembro de 2020). [Kanban Guides](https://kanbanguides.org/the-kanban-guide/2020.12/).
4. AHMAD, M. O.; MARKKULA, J.; OIVO, M. *Kanban in software development: A systematic literature review*. SEAA, 2013, pp. 9–16. [IEEE Xplore](https://ieeexplore.ieee.org/document/6619482/) e [manuscrito disponibilizado pelos autores](https://www.researchgate.net/publication/260739586_Kanban_in_Software_Development_A_Systematic_Literature_Review).
5. SCRUM.ORG. *The Kanban Guide for Scrum Teams*. [Guia online](https://www.scrum.org/resources/online-kanban-guide-scrum-teams).
6. BACCHELLI, A.; BIRD, C. *Expectations, outcomes, and challenges of modern code review*. ICSE, 2013. Referência indicada no enunciado para consulta e análise das revisões reais (actividade 11).
7. GITHUB. [GitHub Docs](https://docs.github.com/pt): Issues, Projects, iterações, Pull Requests e revisões. Referência operacional indicada no enunciado.
8. CHACON, S.; STRAUB, B. [Pro Git, 2.ª edição](https://git-scm.com/book/pt-pt/v2), 2014. Referência indicada no enunciado.
9. PAIVA, Judson. *Lab #02 — Métodos ágeis com Scrum, Kanban, Git e GitHub: Caderneta Digital do Coordenador de Turno*. ISPTEC, 2026/2027. Actividades 1–14 e calendário.

**Aprovação do acordo:** [Registar a data e decisão real do grupo].
