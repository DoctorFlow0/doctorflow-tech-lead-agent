---
name: doctorflow-workflow
description: Fluxo DoctorFlow no Cursor — Tech Lead, Software Engineer e Code Reviewer; quando usar cada etapa.
---

# Fluxo DoctorFlow (três agentes)

Use este skill quando precisar alinhar **ordem de trabalho** e **qual regra** pedir no Cursor.

## Ordem sugerida

1. **DoctorFlow Tech Lead** — entender demanda, escopo, impactos e riscos antes de codar.
2. **DoctorFlow Software Engineer** — implementar com base no escopo acordado.
3. **DoctorFlow Code Reviewer** — revisar a entrega antes do PR final.

## No Cursor

- Inclua a regra de papel correspondente (`.cursor/rules/*.mdc`) na conversa ou no Agent, conforme a UI do Cursor.
- A regra **DoctorFlow — limites e governança comuns** (`doctorflow-global.mdc`) aplica-se sempre neste workspace.

## Documentação

- Visão geral e papéis: `AGENTS.md`.
- Limites (segredos, LGPD, produção): `LIMITS.md`.
- Detalhe por papel (onboarding humano): pasta `agents/`.

## Quando pular etapas

- Tarefa trivial e já totalmente especificada: pode ir direto ao Software Engineer, mantendo limites globais.
- Ainda assim, mudanças com risco estrutural ou multi-time voltam ao Tech Lead.
