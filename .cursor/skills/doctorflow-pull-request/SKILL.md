---
name: doctorflow-pull-request
description: Checklist antes de abrir ou finalizar PR após trabalho com os agentes DoctorFlow.
---

# PR — checklist DoctorFlow

Use após implementação e, de preferência, após passar pelo **DoctorFlow Code Reviewer** na mesma demanda.

## Antes de abrir o PR

- Escopo da mensagem de PR bate com o que foi combinado (Tech Lead / ticket).
- Não há segredos, PII real ou dumps sensíveis em diff, anexos ou descrição.
- Testes ou verificações manuais mínimas descritos na descrição do PR (o que rodou, o que não se aplica).

## Descrição do PR

- **O quê** mudou e **por quê** (1–3 parágrafos claros).
- Impacto em produto/operação, se houver.
- Riscos conhecidos e como mitigar ou validar pós-merge.

## Revisão

- Responder comentários do revisor humano; decisões de produto/arquitetura não delegar só à IA.
- Merge apenas com aprovação humana conforme política do time.

## Referência

- Limites gerais: `LIMITS.md`.
- Fluxo de agentes: `AGENTS.md`.
