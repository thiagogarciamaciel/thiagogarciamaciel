# Olá, eu sou o Thiago 👋
 
**Release Train Engineer e Project Manager** | Engenheiro da Computação | Palmital, SP, Brasil
 
Há quase sete anos trabalho com entrega de software: hoje coordeno um cluster de até 12 squads (cerca de 80 pessoas) em um grande banco, em ambiente regulado, com foco em métricas de engenharia (DORA, lead time), OKRs e coaching de Product Owners. Comecei a carreira como desenvolvedor Java e sigo próximo da tecnologia.
 
Alguns resultados do meu trabalho: lead time das features de **130 para 60 dias**, esforço por ponto de função de **120 para 35 horas** e retrabalho de **11% para 2%**.
 
## Projeto em andamento: sistema de gestão de obras (estudo e portfólio)
 
Desde julho de 2026 construo, sozinho, um sistema de gestão de obras que cobre o ciclo financeiro da operação: cotação com fornecedores concorrentes, medição quinzenal, taxa de administração, comprovantes, conciliação e indicadores por metro quadrado. A visão final é uma plataforma web com aplicativos Android e iOS. O repositório é privado e há um piloto controlado previsto para janeiro de 2027.
 
O diferencial é o **modelo de trabalho**: o código é escrito por dois agentes de IA (Claude Code e Codex) em paralelo, sob regras que eu defino e mantenho versionadas no repositório. Eu faço a arquitetura, as decisões de produto e a governança do processo.
 
**Como o processo funciona**
 
- **Autonomia em três níveis** (alta, guiada e restrita): um classificador roda em cada PR e decide, por tipo de arquivo alterado, o que um agente pode mergear sozinho e o que exige meu aceite. Um PR não consegue baixar o próprio nível.
- **Definition of Ready e Definition of Done** por história, com decisões de produto registradas e bloqueio formal quando falta decisão minha (mais de 20 histórias entregues nesse fluxo).
- **Revisão obrigatória por revisores especializados** (regras financeiras e privacidade de dados) antes de qualquer merge nessas áreas.
- **Documentação como contrato entre os agentes**: regras de negócio, contratos de API e processo; toda mudança de norma entra nos arquivos de instrução dos dois agentes no mesmo PR.
 
**Decisões técnicas**
 
- Stack: React 19, TypeScript, NestJS, Prisma, PostgreSQL 16, Docker, storage compatível com S3, Playwright, Vitest e GitHub Actions.
- Consistência financeira imposta no banco (CHECK constraints, triggers, valores em decimal), comandos idempotentes com transações serializáveis e fila de notificação em outbox transacional.
- Migrations em fases expand/contract, com contrato automatizado contra PostgreSQL real.
- Testes em camadas: unitários, integração com banco real, E2E com MFA e testes de concorrência. CI com gate multi-job e varredura de segredos a cada push.
- Segurança: MFA por TOTP, trilha de auditoria append-only, anexos em storage privado com URL assinada e autorização por objeto.
 
## Competências
 
`SAFe` · `Scrum` · `Kanban` · `DORA` · `OKRs` · `Jira` · `Azure DevOps` · `SQL` · `Power BI` · `Java` (leitura e início de carreira) · `TypeScript` · `PostgreSQL` · `GitHub Actions` · `Engenharia assistida por IA`
 
## Contato
 
[LinkedIn](https://www.linkedin.com/in/thiago-garcia-maciel)
 
---
 
# Hi, I'm Thiago 👋
 
**Release Train Engineer and Project Manager** | Computer Engineer | Palmital, SP, Brazil
 
For almost seven years I have worked in software delivery. Today I coordinate a cluster of up to 12 squads (about 80 people) at a large bank in a regulated environment, focusing on engineering metrics (DORA, lead time), OKRs and coaching Product Owners. I started my career as a Java developer and I stay close to the technology.
 
Some results: feature lead time down from **130 to 60 days**, effort per function point from **120 to 35 hours**, and rework from **11% to 2%**.
 
## Ongoing project: construction management system (study and portfolio)
 
Since July 2026 I have been building, on my own, a construction management system that covers the financial cycle of the operation: quotes from competing suppliers, bi-weekly measurements, administration fee, payment receipts, reconciliation and per-square-meter indicators. The target is a web platform with Android and iOS apps. The repository is private, and a controlled pilot is planned for January 2027.
 
The differentiator is the **way of working**: the code is written by two AI agents (Claude Code and Codex) running in parallel, under rules that I define and keep versioned in the repository. I own the architecture, the product decisions and the governance of the process.
 
**How the process works**
 
- **Three autonomy levels** (high, guided and restricted): a classifier runs on every PR and decides, by file type, what an agent can merge alone and what needs my explicit approval. A PR cannot lower its own level.
- **Definition of Ready and Definition of Done** per story, with recorded product decisions and a formal block when a decision from me is missing (20+ stories delivered this way).
- **Mandatory review by specialized reviewers** (financial rules and data privacy) before any merge that touches those areas.
- **Documentation as a contract between agents**: business rules, API contracts and process; every rule change goes into both agents' instruction files in the same PR.
 
**Technical decisions**
 
- Stack: React 19, TypeScript, NestJS, Prisma, PostgreSQL 16, Docker, S3-compatible storage, Playwright, Vitest and GitHub Actions.
- Financial consistency enforced in the database (CHECK constraints, triggers, decimal values), idempotent commands with serializable transactions and a transactional outbox notification queue.
- Expand/contract migrations with an automated contract test against a real PostgreSQL.
- Layered tests: unit, integration with a real database, E2E with MFA and concurrency tests. CI with a multi-job gate and secret scanning on every push.
- Security: TOTP MFA, append-only audit trail, private attachment storage with signed URLs and per-object authorization.
 
## Skills
 
`SAFe` · `Scrum` · `Kanban` · `DORA` · `OKRs` · `Jira` · `Azure DevOps` · `SQL` · `Power BI` · `Java` (reading and early career) · `TypeScript` · `PostgreSQL` · `GitHub Actions` · `AI-assisted engineering`
 
## Contact
 
[LinkedIn](https://www.linkedin.com/in/thiago-garcia-maciel)
