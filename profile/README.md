# Tech Curse

Plataforma de cursos online: catálogo, cadastro de alunos, matrículas e área do aluno. É um projeto pessoal com dois objetivos: ser usado de verdade por um grupo pequeno de pessoas e servir de portfólio e base de estudos de engenharia de software, do código à operação.

## Repositórios

| Repositório | O que é | Stack |
| --- | --- | --- |
| [tech-curse-api](https://github.com/tech-curse/tech-curse-api) | API REST | .NET 10, ASP.NET Core, PostgreSQL, Redis, JWT |
| [tech-curse-web](https://github.com/tech-curse/tech-curse-web) | Front-end | Angular 22, Tailwind CSS, spartan/ui |

A infraestrutura de implantação fica num repositório privado.

## Como o projeto é conduzido

- Desenvolvimento trunk-based: branch curta, pull request e squash merge; a `main` está sempre pronta para implantar.
- Commits e títulos de PR em [Conventional Commits](https://www.conventionalcommits.org/pt-br/), em português.
- Versionamento semântico, com as mudanças de cada versão registradas no `CHANGELOG.md` de cada repositório.
- Segredos fora do código: cada repositório traz apenas um `.env.example` sem valores reais.

Para contribuir, veja o [guia de contribuição](https://github.com/tech-curse/.github/blob/main/CONTRIBUTING.md). Vulnerabilidades seguem a [política de segurança](https://github.com/tech-curse/.github/blob/main/SECURITY.md).

Mantido por Luiz Gabriel dos Santos Nogueira ([@Liuizn](https://github.com/Liuizn)).
