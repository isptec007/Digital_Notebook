# Documento de requisitos — Caderneta Digital do Coordenador de Turno

**Disciplina:** Engenharia de Software I — Lab #02, ISPTEC (2026/2027)  
**Versão:** 0.1 — proposta para validação pelo grupo e pelo coordenador de turno  
**Prazo de entrega:** 13/12/2026, às 23h59.

## 1. Contextualização

Actualmente, as informações sobre alunos, ocorrências escolares e decisões disciplinares encontram-se dispersas por cadernos, documentos e folhas de cálculo. Isto dificulta a consulta e o acompanhamento dos alunos.

A Caderneta Digital pretende centralizar essas informações numa aplicação web utilizável no computador e no telemóvel, facilitando o trabalho do coordenador de turno.

## 2. Objectivo do Produto (Product Goal)

Disponibilizar uma aplicação segura, responsiva e acessível que permita ao coordenador gerir turmas e alunos, registar ocorrências envolvendo um ou vários alunos, registar as medidas aplicadas e consultar o histórico individual de cada aluno.

## 3. Escopo do produto

### 3.1. MVP obrigatório

1. Autenticação por palavra-passe e acesso por perfil.
2. Gestão de turmas e alunos.
3. Registo de ocorrências com associação de vários alunos.
4. Registo das medidas aplicadas.
5. Consulta do histórico individual do aluno.

A aplicação deve executar localmente a partir do repositório, guardar os dados, respeitar os requisitos de segurança, usabilidade e acessibilidade e utilizar apenas dados pessoais fictícios nos testes e demonstrações.

### 3.2. Funcionalidades posteriores ao MVP

Registo de testemunhas e intervenientes, acompanhamento das medidas, gestão de encarregados de educação e contactos, administração de contas, gestão independente de turnos, cursos e classes, relatórios, reuniões e notificações.

A publicação online é opcional e valorizada na avaliação. Nenhuma extensão deve comprometer o MVP.

## 4. Actores e perfis de utilizador


| Actor | Responsabilidade | Acesso à aplicação no MVP |
|---|---|---|
| Coordenador de turno | Gerir alunos, turmas, ocorrências e medidas | Sim |
| Administrador | Controlar o acesso e as permissões | Sim |
| Aluno | Pessoa cujas informações e ocorrências são registadas | Não; sem conta própria |
| Encarregado de educação | Acompanhar o educando e comunicar com o coordenador | Não; gestão de contactos pós-MVP |
| Professor / funcionário | Pode testemunhar ou intervir numa ocorrência | Não; registo como interveniente pós-MVP |


### 4.1. Matriz de permissões proposta

| Operação | Administrador | Coordenador |
|---|---|---|
| Iniciar e terminar sessão | Sim | Sim |
| Gerir turmas e alunos | Não | Sim |
| Registar e consultar ocorrências | Não | Sim |
| Registar e consultar medidas | Não | Sim |
| Consultar histórico do aluno | Não | Sim |
| Gerir contas e perfis pela interface | Pós-MVP | Não |


## 5. Requisitos funcionais e histórias de utilizador

### RF01 — Autenticação (MVP)

**História:** Como utilizador, quero iniciar e terminar sessão com as minhas credenciais, para aceder à Caderneta Digital de forma segura.

**Critérios de aceitação:**
- [ ] Credenciais válidas permitem iniciar sessão.
- [ ] Credenciais inválidas apresentam uma mensagem de erro compreensível.
- [ ] A palavra-passe é armazenada com hash seguro, nunca em texto simples.
- [ ] É possível terminar sessão e impedir o acesso posterior sem autenticação.

### RF02 — Controlo de acesso por perfil (MVP)

**História:** Como administrador, quero que cada utilizador tenha permissões de acordo com o seu perfil, para proteger as informações do sistema.

**Critérios de aceitação:**
- [ ] Existem contas fictícias com os perfis definidos.
- [ ] As operações disponíveis correspondem às permissões do perfil.
- [ ] O servidor rejeita operações não autorizadas, mesmo quando solicitadas directamente.

### RF03 — Navegação (MVP)

**História:** Como utilizador, quero navegar entre os módulos autorizados, para realizar as minhas actividades sem dificuldades.

**Critérios de aceitação:**
- [ ] O menu apresenta as opções autorizadas para o perfil.
- [ ] O utilizador consegue identificar a página activa e terminar sessão.
- [ ] A navegação funciona no computador e no telemóvel.

### RF04 — Gestão de turmas (MVP)

**História:** Como coordenador, quero cadastrar, consultar e actualizar turmas, para organizar os alunos da instituição.

**Critérios de aceitação:**
- [ ] É possível cadastrar, listar e editar turmas.
- [ ] O identificador da turma é obrigatório e não pode ser duplicado.
- [ ] É possível consultar os alunos associados à turma.
- [ ] Os dados são guardados de forma persistente.

### RF05 — Cadastro de alunos (MVP)

**História:** Como coordenador, quero cadastrar alunos e associá-los às respectivas turmas, para manter os dados académicos organizados.

**Critérios de aceitação:**
- [ ] É possível registar nome, número de identificação e turma.
- [ ] O número de identificação é único.
- [ ] O sistema rejeita campos obrigatórios em falta e turmas inexistentes.
- [ ] O aluno permanece registado após reiniciar a aplicação.

### RF06 — Consulta e edição de alunos ( MVP)

**História:** Como coordenador, quero pesquisar e actualizar os dados dos alunos, para encontrar informações correctas.

**Critérios de aceitação:**
- [ ] É possível listar alunos e pesquisar por nome ou número de identificação.
- [ ] É possível filtrar por turma.
- [ ] É possível consultar os detalhes e editar os dados do aluno.
- [ ] As validações de cadastro também se aplicam à edição.

### RF07 — Registo de ocorrências (MVP)

**História:** Como coordenador, quero registar ocorrências escolares, para documentar os acontecimentos na instituição.

**Critérios de aceitação:**
- [ ] É possível informar título, data, hora, local e descrição detalhada.
- [ ] O sistema identifica o utilizador que fez o registo.
- [ ] Os campos obrigatórios são validados.
- [ ] A ocorrência é guardada de forma persistente.

### RF08 — Associação de vários alunos (MVP)

**História:** Como coordenador, quero associar vários alunos à mesma ocorrência, para identificar todos os envolvidos sem duplicar o acontecimento.

**Critérios de aceitação:**
- [ ] É possível pesquisar e seleccionar alunos existentes.
- [ ] Uma ocorrência pode envolver alunos de turmas diferentes.
- [ ] O mesmo aluno não pode ser associado duas vezes à mesma ocorrência.
- [ ] Os detalhes mostram todos os alunos envolvidos.
- [ ] A versão integrada de registo exige pelo menos um aluno, se esta regra for validada com o coordenador.

### RF09 — Consulta e edição de ocorrências (MVP)

**História:** Como coordenador, quero consultar e actualizar ocorrências, para acompanhar os acontecimentos escolares.

**Critérios de aceitação:**
- [ ] É possível listar, pesquisar pelo título e filtrar por data ou turma.
- [ ] Os detalhes mostram a descrição e os alunos envolvidos.
- [ ] Utilizadores autorizados podem editar a ocorrência.
- [ ] Uma alteração não deixa medidas associadas a alunos que já não pertencem à ocorrência.

### RF10 — Registo de medidas aplicadas (MVP)

**História:** Como coordenador, quero registar as medidas aplicadas aos alunos envolvidos numa ocorrência, para documentar as decisões tomadas.

**Critérios de aceitação:**
- [ ] É possível seleccionar uma ocorrência e um aluno envolvido.
- [ ] É possível registar a descrição da medida e a data da decisão.
- [ ] Alunos da mesma ocorrência podem receber medidas diferentes.
- [ ] O sistema rejeita medidas para alunos que não estejam associados à ocorrência.

### RF11 — Consulta e edição de medidas (MVP)

**História:** Como coordenador, quero consultar e actualizar as medidas registadas, para manter as decisões documentadas.

**Critérios de aceitação:**
- [ ] É possível consultar as medidas associadas a uma ocorrência.
- [ ] Cada medida identifica o aluno, a descrição e a data da decisão.
- [ ] Utilizadores autorizados podem editar as medidas, respeitando as validações.

### RF12 — Histórico individual do aluno (MVP)

**História:** Como coordenador, quero consultar o histórico de um aluno, para conhecer as ocorrências em que esteve envolvido e as medidas que lhe foram aplicadas.

**Critérios de aceitação:**
- [ ] O histórico apresenta os dados do aluno e da sua turma.
- [ ] São apresentadas todas as ocorrências em que o aluno esteve envolvido.
- [ ] Apenas as medidas do aluno seleccionado são apresentadas como suas medidas.
- [ ] Os registos são organizados cronologicamente e permitem consultar os detalhes.
- [ ] É apresentada uma mensagem quando não existem ocorrências ou medidas.

### RF13 — Testemunhas e intervenientes (pós-MVP)

**História:** Como coordenador, quero registar testemunhas e intervenientes, para documentar quem participou ou presenciou uma ocorrência.

**Critérios de aceitação:**
- [ ] É possível associar várias pessoas a uma ocorrência, com nome e tipo de participação.
- [ ] As informações aparecem nos detalhes da ocorrência.

### RF14 — Acompanhamento das medidas (pós-MVP)

**História:** Como coordenador, quero acompanhar o cumprimento das medidas, para identificar decisões pendentes e cumpridas.

**Critérios de aceitação:**
- [ ] É possível registar estado, prazo e observações de acompanhamento.
- [ ] O estado actualizado aparece no histórico do aluno.

### RF15 — Gestão de encarregados (pós-MVP)

**História:** Como coordenador, quero registar e associar encarregados de educação aos alunos, para facilitar a comunicação com as famílias.

**Critérios de aceitação:**
- [ ] É possível cadastrar, consultar e editar nome, contacto e relação com o aluno.
- [ ] É possível associar encarregados a alunos e consultar essas associações.
- [ ] Os contactos são protegidos por permissões.

### RF16 — Registo de contactos (pós-MVP)

**História:** Como coordenador, quero registar os contactos com encarregados, para acompanhar a comunicação efectuada.

**Critérios de aceitação:**
- [ ] É possível registar aluno, encarregado, data, meio, motivo e resultado do contacto.
- [ ] Os contactos aparecem no histórico do aluno e podem ser ligados a uma ocorrência.

### RF17 — Gestão de utilizadores (pós-MVP)

**História:** Como administrador, quero gerir contas e perfis, para controlar quem pode utilizar o sistema.

**Critérios de aceitação:**
- [ ] É possível cadastrar, consultar, editar e desactivar contas.
- [ ] Apenas o perfil autorizado pode modificar contas e permissões.
- [ ] Contas desactivadas não conseguem iniciar sessão.

### RF18 — Gestão da estrutura académica (pós-MVP)

**História:** Como coordenador, quero gerir turnos, cursos e classes, para organizar a estrutura académica da instituição.

**Critérios de aceitação:**
- [ ] É possível cadastrar, consultar e editar turnos, cursos e classes.
- [ ] É possível relacionar turmas com estes elementos sem perder os dados existentes.

### RF19 — Relatórios e indicadores (pós-MVP)

**História:** Como coordenador, quero consultar indicadores de ocorrências, para apoiar as decisões e responder aos pedidos da direcção.

**Critérios de aceitação:**
- [ ] É possível consultar o total de ocorrências e medidas, por turma e período.
- [ ] Uma ocorrência envolvendo várias turmas não é duplicada no total geral.

### RF20 — Agendamento de reuniões (pós-MVP)

**História:** Como coordenador, quero agendar reuniões, para organizar o acompanhamento dos alunos.

**Critérios de aceitação:**
- [ ] É possível registar assunto, aluno, participantes, data, hora e local.
- [ ] É possível consultar, reagendar e cancelar reuniões.

### RF21 — Notificações e lembretes (pós-MVP)

**História:** Como coordenador, quero receber lembretes, para não esquecer reuniões e medidas pendentes.

**Critérios de aceitação:**
- [ ] São gerados lembretes de reuniões e medidas próximas do prazo ou em atraso.
- [ ] O utilizador autorizado consegue consultar e marcar notificações como lidas.

## 6. Requisitos não funcionais

| ID | Requisito | Critério de verificação | Prioridade |
|---|---|---|---|
| RNF01 | Responsividade | Todos os módulos do MVP funcionam em computador e telemóvel. | P1 |
| RNF02 | Usabilidade | Formulários têm etiquetas claras, navegação consistente e mensagens de erro que explicam como corrigir o problema. | P1 |
| RNF03 | Acessibilidade | Navegação por teclado, foco perceptível, contraste suficiente e texto alternativo em imagens informativas. | P1 |
| RNF04 | Segurança | Palavras-passe com hash seguro, controlo de acesso no servidor, sessões protegidas e ausência de credenciais reais no repositório. | P0 |
| RNF05 | Privacidade | Dados pessoais exclusivamente fictícios em testes, demonstrações e publicação, se existir. | P0 |
| RNF06 | Persistência | Os dados continuam disponíveis após reiniciar a aplicação. | P0 |
| RNF07 | Integridade | Dados obrigatórios, unicidade de identificadores e relacionamentos são validados no servidor. | P0 |
| RNF08 | Executabilidade | Outro membro consegue instalar e executar localmente seguindo o README. | P1 |
| RNF09 | Manutenibilidade | Código organizado, versionado e revisto; alterações relevantes têm testes e documentação. | P1 |
| RNF10 | Publicação (opcional) | Se publicada, a aplicação funciona online com HTTPS e dados persistentes. | P2 |



## 7. Regras de negócio propostas

| ID | Regra |
|---|---|
| RN01 | Cada aluno possui um número de identificação único e pertence a uma turma no modelo inicial. |
| RN02 | Uma turma pode conter vários alunos. |
| RN03 | Uma ocorrência pode envolver vários alunos, inclusive de turmas diferentes; um aluno pode participar em várias ocorrências. |
| RN04 | O mesmo aluno não pode ser associado mais de uma vez à mesma ocorrência. |
| RN05 | Uma medida pertence a um aluno e a uma ocorrência em que esse aluno esteve envolvido. |
| RN06 | Alunos de uma mesma ocorrência podem receber medidas diferentes. |
| RN07 | O histórico reúne as ocorrências e medidas do aluno seleccionado. |
| RN08 | Apenas utilizadores autorizados podem consultar ou alterar registos disciplinares. |
| RN09 | Alterações não devem destruir o histórico nem deixar relacionamentos inválidos; exclusão de registos fica fora do MVP até validação. |


## 9. Cenário de aceitação do MVP (Geral)
| Passo | Acção | Resultado esperado |
|---|---|---|
| 1 | Iniciar sessão como coordenador | Acesso autorizado |
| 2 | Cadastrar três turmas e três alunos fictícios | Cada aluno fica associado à sua turma |
| 3 | Registar uma discussão no intervalo e associar os três alunos | Uma única ocorrência com três alunos de turmas diferentes |
| 4 | Aplicar medidas individuais aos alunos | Cada medida fica associada ao aluno correcto |
| 5 | Consultar o histórico de um dos alunos | Ocorrência e medidas desse aluno são apresentadas |
| 6 | Reiniciar a aplicação | Os registos permanecem disponíveis |
| 7 | Tentar aceder aos registos com uma conta sem autorização | Acesso rejeitado |
| 8 | Repetir o fluxo no telemóvel e navegar por teclado | Interface funcional e acessível |
