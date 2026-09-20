# RunicTools · manutenção

[← README](../README.md)

## Fluxo de mudança

1. Identifique o componente na tabela de arquitetura do README.
2. Confirme o contrato nos arquivos de entrada e manifests; documentação não substitui o código.
3. Faça a alteração em um branch, preservando dados locais e arquivos de origem.
4. Execute as verificações relacionadas ao fluxo e revise `git diff --check`.
5. Descreva evidências e limites; publicar documentação não equivale a publicar uma aplicação.

## Contrato de dados

Defaults da organização se aplicam aos repositórios que não fornecem seus próprios arquivos equivalentes. Código e instruções específicas de execução pertencem aos produtos. Consulte docs/ORGANIZATION_SETUP.md para contexto de administração; essa referência não substitui conferir a configuração atual do GitHub.

## Execução e distribuição

Este repositório não é uma aplicação: não exige build, servidor ou banco. Leia os documentos abaixo e edite apenas o contrato correspondente ao objetivo da mudança.

O início rápido descreve desenvolvimento local. Antes de expor o serviço, revise a configuração de hospedagem específica do repositório, permissões, persistência e procedimento de atualização. Segredos e dados de usuários não pertencem aos exemplos nem ao Git.

## Diagnóstico inicial

| Sintoma | Primeiro ponto a conferir |
| --- | --- |
| Template não aparece em um produto | Confira se o repositório do produto tem arquivo próprio que substitui o default. |
| Perfil da organização não mudou | A superfície pública usa profile/README.md; o README da raiz descreve o repositório. |
| Política diverge entre projetos | Leia a política específica do produto; não sobrescreva o contrato local por inferência. |

## Limites de interpretação

Alterar uma política compartilhada afeta outros projetos. Esta atualização de apresentação não altera regras de segurança, permissões, contribuição ou automações. Nunca armazene credenciais, dumps, backups ou .env aqui.

## Base desta documentação

A apresentação foi confrontada com os seguintes arquivos e diretórios do checkout. Essa revisão foi estática; não executou o produto, coletores, instalações ou deploys.

- [profile/README.md](../profile/README.md) — Apresentação pública da organização.
- [COLLABORATION.md](../COLLABORATION.md) — Fluxo recomendado entre mantenedores.
- [CONTRIBUTING.md](../CONTRIBUTING.md) — Contrato de contribuição.
- [SECURITY.md](../SECURITY.md) — Orientação de reporte privado.
- [CODE_OF_CONDUCT.md](../CODE_OF_CONDUCT.md) — Conduta da comunidade.
- [.github/ISSUE_TEMPLATE/](../.github/ISSUE_TEMPLATE/) — Formulários de trabalho compartilhados.
