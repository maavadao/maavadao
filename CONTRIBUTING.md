# Contributing to mawaDao

Thank you for helping. There are many ways to contribute, and not all of them involve code:

- Build or improve AI agents for education, teaching and content creation
- Propose a project for the DAO to vote on
- List useful AI tools so students and educators can learn about them
- Review agents for safety, quality and bias
- Translate agents and learning content into local languages
- Improve documentation and guides
- Connect schools, colleges and communities to the platform

## Where to contribute

Open issues and pull requests in the repository that owns what you are changing.
[INDEX.md](INDEX.md) lists every repository and what it holds.

| You want to | Go to |
| --- | --- |
| List an AI tool or agent | [mawadao/registry](https://github.com/mawadao/registry) |
| Work on the member space or agent runtime | [mawadao/mawa](https://github.com/mawadao/mawa/blob/main/CONTRIBUTING.md) |
| Change mawadao.com or the marketplace | [mawadao/frontend](https://github.com/mawadao/frontend) |
| Improve the vision, mission or index | This repository |

## In this repository

This repository holds the vision, mission and index, and brings the others together as
submodules. Changes here are usually to the Markdown pages or to move a submodule to a newer
commit:

```bash
git submodule update --remote registry
git add registry
git commit -m "Update registry"
```

Write in British English (organisation, licence) and spell the name "mawaDao".

## Licence

By contributing you agree that your work is released under the Apache License 2.0.
