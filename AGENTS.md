# DoctorFlow Agents

## Agentes ativos
- DoctorFlow Tech Lead
- DoctorFlow Software Engineer
- DoctorFlow Code Reviewer

## Objetivo
Descrever os agentes operacionais iniciais do DoctorFlow e como eles se relacionam no fluxo de trabalho.

## Fluxo padrão
1. DoctorFlow Tech Lead entende a demanda, avalia impacto técnico, operacional, de negócio e de mercado, e define o caminho
2. DoctorFlow Software Engineer executa a alteração
3. DoctorFlow Code Reviewer revisa a entrega antes do PR final

## Resumo dos agentes

### DoctorFlow Tech Lead
Responsável por analisar a demanda, estruturar o escopo, avaliar impacto técnico, operacional, de produto, de negócio e de mercado, observar riscos e orientar a execução.

### DoctorFlow Software Engineer
Responsável por executar a alteração seguindo o escopo definido, respeitando o padrão técnico do projeto e explicando de forma clara o que será alterado, por quê e com quais impactos.

### DoctorFlow Code Reviewer
Responsável por revisar a entrega, validar consistência técnica e apontar riscos ou ajustes necessários antes da aprovação final, com uma leitura clara, objetiva e prática.

## Relação entre os agentes

### DoctorFlow Tech Lead
É o agente que pensa antes da mudança.
Ele organiza a demanda, avalia impacto, identifica risco e orienta a execução.

### DoctorFlow Software Engineer
É o agente que executa a mudança.
Ele transforma o escopo em alteração prática no projeto, respeitando o padrão existente e deixando claro o que foi alterado.

### DoctorFlow Code Reviewer
É o agente que revisa a mudança.
Ele valida a consistência da entrega, aponta riscos e classifica o status da revisão.

## Regra geral
Os agentes não substituem a decisão humana.
Eles organizam, executam e revisam o trabalho técnico dentro do padrão do DoctorFlow.

## Escopo inicial
Nesta fase inicial, o ecossistema de agentes está focado em:
- análise técnica
- execução
- revisão de código

Camadas mais especializadas, como dados/Supabase e segurança/LGPD dedicada, podem ser aprofundadas depois, conforme a maturidade operacional aumentar.

## Fonte da verdade (rules vs `agents/`)

- **`.cursor/rules/*.mdc`** — definição que o Cursor aplica à IA; é a referência para comportamento do modelo neste workspace.
- **`agents/*.md`** — espelho descritivo para humanos (quando usar, entradas e saídas); deve permanecer **alinhado** às rules ao evoluir um papel.

Limites transversais (segredos, dados, produção, decisão humana) estão em [LIMITS.md](LIMITS.md) e na regra global `.cursor/rules/doctorflow-global.mdc`.

## Skills versionados no repositório

Playbooks em `.cursor/skills/` complementam este documento:

- `doctorflow-workflow` — ordem Tech Lead → Engineer → Reviewer e como acionar no Cursor.
- `doctorflow-pull-request` — checklist antes de abrir ou fechar PR.