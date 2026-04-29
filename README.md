# doctorflow-tech-lead-agent

Repositório que centraliza **agentes**, **regras do Cursor** e **skills** de trabalho do DoctorFlow.

Este repositório **não** é o código da aplicação DoctorFlow: aqui ficam apenas instruções e governança para uso consistente de IA no desenvolvimento.

## Conteúdo

| Caminho | Função |
|--------|--------|
| [AGENTS.md](AGENTS.md) | Fluxo dos três agentes e resumo de papéis |
| [LIMITS.md](LIMITS.md) | Limites: segredos, dados, produção, decisão humana |
| `agents/` | Especificação legível por humanos (entradas, saídas, quando usar) |
| `.cursor/rules/` | Regras consumidas pelo Cursor (inclui regra global sempre ativa) |
| `.cursor/skills/` | Playbooks versionados (fluxo DoctorFlow, checklist de PR) |
| [LICENSE](LICENSE) | Licenciamento / reserva de direitos |

## Como usar no Cursor

1. **Sempre**: a regra global [`.cursor/rules/doctorflow-global.mdc`](.cursor/rules/doctorflow-global.mdc) aplica-se a todas as conversas neste workspace (`alwaysApply: true`).
2. **Por tarefa**: inclua a regra do papel adequado — Tech Lead, Software Engineer ou Code Reviewer — via seletor de regras / contexto do Agent, conforme a interface do Cursor.
3. **Skills opcionais**: em projetos que suportem skills na pasta do repo, use [`.cursor/skills/doctorflow-workflow/SKILL.md`](.cursor/skills/doctorflow-workflow/SKILL.md) e [`.cursor/skills/doctorflow-pull-request/SKILL.md`](.cursor/skills/doctorflow-pull-request/SKILL.md) para padronizar fluxo e PR.

Ordem sugerida de trabalho: **Tech Lead → Software Engineer → Code Reviewer** (ver [AGENTS.md](AGENTS.md)).

## Fonte da verdade

- **Comportamento da IA no Cursor**: `.cursor/rules/*.mdc` (autoritativo para o produto).
- **`agents/*.md`**: documentação alinhada às rules, com mais detalhe operacional para pessoas; mantenha os dois em sinc quando alterar um papel.

Alterações em governança (por exemplo [LIMITS.md](LIMITS.md)) devem passar por PR e revisão humana.
