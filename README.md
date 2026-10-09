# maavaDao
### Community-Governed AI & Blockchain Technologies for Education

**Build it. Own it. Share it. Free for everyone, with a share of every success going to
children who need it most.**

maavaDao brings together agentic AI and blockchain technologies to create an open,
community-owned ecosystem for education. Developers build and list AI agents on the maava
Marketplace. Educators, students and content creators use them to teach, learn, research and
inform. The community decides, through the DAO, what gets built next.

There are no listing fees, no creation fees and no commissions. When a product earns money,
**75% goes to the community who built it and 25% goes to maava** to educate deserving children,
orphans and street children.

maava already runs **two schools for deserving children**, and maavaDao extends that mission into
the age of AI: we're now setting up **Maava School for AI**.

This repository is the front door to everything maavaDao. It brings every public maavaDao
repository together as Git submodules, and explains why the project exists and where each part
lives.

| Read | For |
| --- | --- |
| [VISION.md](VISION.md) | Why maavaDao exists and the future it is working towards |
| [MISSION.md](MISSION.md) | What we do, how the platform works, governance, safety and the roadmap |
| [INDEX.md](INDEX.md) | Every repository, component and public index, and where to find things |

## What's here

```
maavadao/
├── website/       maavadao.com, including the marketplace         → maavadao/frontend
├── maava/          maava: member space, community and agent        → maavadao/maava
│                  runtime (has its own submodules)
├── registry/      Community list of AI tools and agents          → maavadao/marketplace-registry
├── supabase/      Database and sign-in for maavadao.com           → maavadao/supabase
└── org-profile/   The GitHub organisation profile                → maavadao/.github
```

## Three ways in

**Explore and learn.** Students, educators, content creators and anyone curious can browse AI
tools on maavaDao, with what each one costs for education, individuals and businesses. The list
lives in [`registry/`](registry) and anyone can add to it by pull request.

**Use agents, free.** Schools, colleges, universities, teachers and students use agents from the
maava Marketplace free of charge, for teaching, tutoring, research and learning. Using agents in a
larger organisation? [Talk to us](https://maavadao.com/#contact).

**Build and contribute.** Developers list agents for free, propose projects the community can
vote on through the DAO, and improve the platform itself in [`maava/`](maava). When a product is
monetised, 75% of the revenue goes back to the contributors who built it, and 25% funds the
education of deserving children, orphans and street children.

## Get everything

```bash
git clone --recurse-submodules https://github.com/maavadao/maavadao.git
cd maavadao
```

Already cloned? Run `git submodule update --init --recursive`. To move every part to its latest
`main`: `git submodule update --remote`.

Each folder is its own repository. Open issues and pull requests in the repository that owns the
code; [INDEX.md](INDEX.md) says which one that is.

## Contributing

Start with [CONTRIBUTING.md](CONTRIBUTING.md). In short:

- To list an AI tool or agent, open a pull request in [maavadao/marketplace-registry](https://github.com/maavadao/marketplace-registry).
- To change the platform, read [maava's contributing guide](https://github.com/maavadao/maava/blob/main/CONTRIBUTING.md).
- To improve these pages, open a pull request here.

## Licence

Apache 2.0. See [LICENSE](LICENSE). Each repository carries its own licence and notices.

---

*maavaDao: no fees, no commissions, community owned. Built by the community, for every child.*
