# Limites e governança — DoctorFlow (IA)

Este documento define o que os agentes e o uso de IA **não** substituem e o que exige **decisão ou ação humana**.

## Decisão humana

- Aprovação de produto, prazo, escopo comercial e prioridade de roadmap.
- Merge de PR, deploy e mudanças em produção.
- Interpretação final de requisitos legais, contratuais e de compliance.

## Segredos e credenciais

- Não inserir, commitar ou pedir para versionar chaves de API, senhas, tokens, connection strings com segredo ou material de produção.
- Preferir variáveis de ambiente, secret managers e documentação **sem** valores reais.

## Dados pessoais e LGPD

- Não usar dados reais de pacientes, profissionais ou operação em exemplos, fixtures, logs colados no chat ou no repositório.
- Tratar anonimização e bases legais como tema de **especialistas humanos** e políticas internas; agentes podem orientar tecnicamente, mas não substituem parecer jurídico/DPO.

## Infraestrutura e produção

- Não executar destruição de dados, migrações irreversíveis ou alterações em contas cloud sem confirmação explícita de um responsável.
- Assumir que ambientes de produção são **read-only** para a IA até o contrário ser definido por humanos.

## Escopo deste repositório

- Este repositório centraliza **regras, agentes e skills** para o Cursor no contexto DoctorFlow.
- Não é o repositório da aplicação; mudanças de código de produto seguem o fluxo do repositório de software correspondente.

## Atualização

- Alterações neste arquivo entram por PR, com revisão humana, como qualquer mudança de governança.
