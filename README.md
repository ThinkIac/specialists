# specialists

Catálogo e construtor de especialistas do Runtime — AGENT.md genéricos + especialistas personalizados (prompt, tools, provider/modelo)

Repositório: https://github.com/ThinkIac/specialists.

## Uso no ThinkIac

Este pacote foi extraído de `packages/specialists`. Preserve a identidade `specialists` do manifest ao instalá-lo em um workspace Lógos. Views, rotas, ferramentas e hooks são descobertos pelo runtime e dependem dos provedores correspondentes. Esta extração publica o código atual; não converte JavaScript para LógosType nem implementa instalação por perfil.

Entrada declarada: `index.js`.

## Dependências e validação

Dependências declaradas: `logos`.

Scripts disponíveis: `npm run test`.

## Segurança e dados locais

Credenciais devem ser configuradas no ambiente de destino. Não acompanham esta extração bancos, sessões, uploads, perfis pessoais, arquivos `.env`, caches ou backups. As exclusões foram registradas em relatório externo à publicação. Configure segredos pelo host, sem incluí-los em commits.


## Registros encontrados no código

- `router`: `agents`, `catalog`, `catalog/:id`, `preview`, `session`, `system/action`, `system/view`.
- `tool`: `createSpecialist`, `deleteSpecialist`, `getSessionSpecialist`, `getSpecialist`, `listComposableAgents`, `listSpecialists`, `previewSpecialistPrompt`, `setSessionSpecialist`, `updateSpecialist`.

A lista é um inventário estático e pode incluir registros em testes; não garante disponibilidade sem os provedores do host.

Há imports relativos para diretórios superiores. A instalação isolada e a composição por perfil precisam resolver esses vínculos antes de remover a cópia da base.

