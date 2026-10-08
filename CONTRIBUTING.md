# Como contribuir

O Tech Curse é um projeto pessoal. Issues com bugs, dúvidas e sugestões são bem-vindas. Antes de abrir um pull request com uma mudança grande, abra uma issue para conversar sobre ela: pode ser que a ideia não se encaixe nos planos do projeto, e é melhor descobrir isso antes de escrever o código.

## Fluxo de trabalho

O desenvolvimento é **trunk-based**:

1. Crie uma branch curta a partir da `main`, com o nome `<tipo>/<descricao-curta>` (ex.: `fix/refresh-token-expirado`).
2. Faça a mudança, com testes quando ela altera comportamento.
3. Rode localmente o build, os testes e o lint do repositório. O README de cada repositório lista os comandos.
4. Abra um pull request para a `main` e preencha o template.
5. Depois da aprovação e do CI verde, o PR entra por **squash merge**. A `main` precisa estar sempre pronta para implantar.

## Commits e títulos de PR

Use [Conventional Commits](https://www.conventionalcommits.org/pt-br/) em português, com um destes tipos:

| Tipo | Quando usar |
| --- | --- |
| `feat` | nova funcionalidade |
| `fix` | correção de bug |
| `docs` | só documentação |
| `test` | só testes |
| `refactor` | mudança de código sem alterar comportamento |
| `ci` | pipelines e automação |
| `chore` | manutenção que não se encaixa nos anteriores |

Como o merge é squash, o título do PR vira a mensagem do commit na `main`. Capriche nele.

## Convenções

- Documentação, commits e mensagens ao usuário em português do Brasil. Nomes no código seguem o padrão já usado em cada repositório.
- **Sem comentários no código.** A justificativa de uma decisão vai na descrição do PR, na mensagem de commit ou na documentação em Markdown.
- Mudanças notáveis entram no `CHANGELOG.md`, na seção `[Não lançado]`, no mesmo PR.
- **Nunca** versione segredos, dados pessoais ou valores reais de configuração. Uma variável nova entra no `.env.example`, sem valor.

## Código de conduta

Ao participar, você concorda com o [Código de Conduta](CODE_OF_CONDUCT.md).
