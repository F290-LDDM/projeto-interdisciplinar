# Projeto Prático — Laboratório de Desenvolvimento para Dispositivos Móveis

**Curso:** Tecnologia em Desenvolvimento de Software Multiplataforma (DSM)  
**Semestre:** 5º  
**Componente curricular:** Laboratório de Desenvolvimento para Dispositivos Móveis (LDDM)  
**Tecnologia principal:** Flutter / Dart  
**Backend:** API própria ou Supabase (BaaS)  
**Apresentação:** até **20 minutos no total**, por equipe

## 1. Objetivo

Desenvolver, em equipe, um aplicativo móvel em Flutter que resolva um problema real ou atenda a uma necessidade de negócio. A solução deve integrar interface, regras de negócio e persistência remota por meio de uma API própria ou do Supabase.

## 2. Proposta

Cada equipe definirá um produto e implementará um **MVP funcional**: uma jornada principal que possa ser executada do início ao fim e cujos dados sejam persistidos remotamente. Pode-se iniciar um projeto novo ou evoluir um projeto existente, desde que a equipe identifique o que foi desenvolvido para esta disciplina.

A avaliação considera a qualidade e a integração da solução, não a quantidade de telas ou funcionalidades. O tema deve ser apresentado ao docente para acompanhamento e delimitação do MVP.

## 3. Requisitos obrigatórios

### R01 — Aplicativo Flutter

- Implementar o aplicativo em Flutter/Dart.
- Executar em dispositivo ou emulador Android.
- Oferecer navegação coerente e telas adequadas à jornada proposta.
- Tratar estados relevantes, como carregamento, lista vazia e falha de comunicação.
- Aplicar princípios básicos de usabilidade e acessibilidade visual.

### R02 — Backend e persistência remota

Escolher e documentar **uma** das alternativas:

- **Backend próprio:** API da equipe, conectada a um banco de dados.
- **Supabase:** serviços apropriados ao projeto, como banco PostgreSQL, autenticação e APIs.

Em qualquer alternativa, o aplicativo deverá ler e gravar dados reais remotamente, validar entradas relevantes e apresentar o resultado das operações. A jornada principal não pode depender exclusivamente de dados estáticos ou simulados.

### R03 — Funcionalidades de negócio

Implementar operações coerentes com o domínio, incluindo cadastro e consulta e, quando fizer sentido, atualização e exclusão. A equipe deve explicar as regras de negócio e demonstrar pelo menos uma operação concluída com persistência confirmada.

### R04 — Autenticação e proteção de dados

Quando o produto tiver usuários identificados ou informações restritas, implementar autenticação e restringir o acesso conforme o papel do usuário. Não publicar senhas, tokens, chaves privadas ou dados pessoais nos repositórios. Para Supabase, usar políticas de acesso adequadas (RLS) nas tabelas expostas ao cliente e nunca incluir a `service_role key` no aplicativo.

### R05 — Organização e documentação

- Manter o código em repositório Git acessível ao docente.
- Registrar integrantes e contribuições.
- Incluir instruções para configurar e executar a solução, com variáveis de exemplo sem segredos.
- Explicar arquitetura, backend escolhido, modelo de dados essencial e limitações conhecidas.
- Registrar backlog ou lista breve de tarefas e o que foi concluído.

### R06 — Demonstração e apresentação

Apresentar o produto e demonstrar a jornada funcional em **até 20 minutos no total**. A apresentação deve evidenciar o aplicativo, a comunicação com o backend e a persistência dos dados. O detalhamento do material e do roteiro está em [Formato da entrega](#6-formato-da-entrega-e-apresentação).

## 4. Escopo e limites

Não são exigidos aplicativo web, backoffice, Message Broker, publicação em loja, suporte simultâneo a Android e iOS ou infraestrutura paga. Podem ser adicionados como extensões, mas não substituem os requisitos obrigatórios. O backend pode ser executado localmente ou em serviço de nuvem, desde que esteja acessível e preparado para a demonstração.

A equipe deve escolher um escopo viável para o semestre e informar claramente o que está implementado, o que está parcial e o que ficou fora do MVP. Uma funcionalidade demonstrada deve operar de verdade no fluxo apresentado.

## 5. Orientações de desenvolvimento

1. Descreva o problema, o público e a jornada que será resolvida.
2. Delimite um MVP que possa ser demonstrado de ponta a ponta.
3. Esboce as telas e o modelo de dados antes de ampliar funcionalidades.
4. Implemente a integração remota cedo, para validar a arquitetura.
5. Registre decisões, tarefas e contribuições no repositório.
6. Prepare dados de demonstração e ensaie o fluxo completo.

Testes automatizados, integração contínua e protótipos são recomendados quando compatíveis com o escopo. A equipe deve informar os testes ou verificações que executou; não se presume adoção de TDD apenas pela existência de testes.

## 6. Formato da entrega e apresentação

A equipe deverá disponibilizar:

1. **Apresentação do produto:** problema, público-alvo, proposta de valor e escopo do MVP.
2. **Demonstração funcional:** aplicativo Flutter em dispositivo/emulador, com uma jornada principal e evidência da operação remota no backend.
3. **Ficha resumida da equipe:** preencher o [modelo de entrega](docs/MODELO-DE-ENTREGA.md), incluindo integrantes, contribuições, links e roteiro.
4. **Repositório de código:** link acessível, README com execução/configuração e versão final identificada por commit ou tag.

### Tempo total: 20 minutos

| Parte | Tempo de referência | Conteúdo |
|---|---:|---|
| Contexto e pitch | 4 min | Problema, público, solução e valor do produto |
| Demonstração | 12 min | Jornada no Flutter, integração com backend e persistência |
| Arquitetura e decisões | 3 min | Backend escolhido, dados, segurança e principais decisões |
| Encerramento | 1 min | Limitações e próximos passos |
| **Total** | **20 min** | **Apresentação e demonstração** |

A divisão é um roteiro sugerido; o limite de 20 minutos se aplica ao conjunto. Todos os integrantes devem estar preparados para explicar suas contribuições. O docente informará data, local, ordem e eventual dinâmica de perguntas. Se houver arguição, o docente comunicará se ela integra esse limite ou terá tempo separado.

Prepare previamente o dispositivo/emulador, conectividade, credenciais de demonstração e dados necessários. Capturas de tela ou vídeo podem servir de apoio, mas não substituem a demonstração do aplicativo funcionando, salvo orientação do docente.

## 7. Avaliação

A rubrica proposta, com critérios e pesos, está em [Critérios de avaliação](docs/CRITERIOS-DE-AVALIACAO.md). Os pesos são uma proposta de organização e devem ser confirmados pelo docente antes da aplicação. A rubrica não cria regras de aprovação, nota mínima ou penalidades adicionais.

## 8. Checklist da equipe

- [ ] Problema, público-alvo e MVP definidos.
- [ ] Aplicativo Flutter executa em Android ou emulador.
- [ ] Jornada principal pode ser concluída na demonstração.
- [ ] Aplicativo lê e grava dados em backend remoto.
- [ ] Estados de carregamento, ausência de dados e erro são tratados conforme aplicável.
- [ ] Autenticação e regras de acesso foram consideradas para dados restritos.
- [ ] Repositório contém instruções, configuração de exemplo e contribuições.
- [ ] Ficha resumida preenchida e links conferidos.
- [ ] Ambiente e dados preparados; apresentação ensaiada para caber em 20 minutos.
