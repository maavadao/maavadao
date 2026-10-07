# mawaDao

**A non-profit, community-owned marketplace for responsible AI agents, built to bring quality
education to underserved children and orphans.**

Millions of children, particularly orphans and those in low-income or remote communities, have no
access to good teachers, tutoring or learning resources. At the same time, developers around the
world are building AI agents that could help close that gap. mawaDao connects the two: developers
build and list agents, schools and educators use them free of charge, and the community that
builds the platform owns it and decides how it is run.

This repository is the front door to everything mawaDao. It brings every public mawaDao
repository together as Git submodules, and explains why the project exists and where each part
lives.

| Read | For |
| --- | --- |
| [VISION.md](VISION.md) | Why mawaDao exists and the future it is working towards |
| [MISSION.md](MISSION.md) | What we do, how the platform works, governance, safety and the roadmap |
| [INDEX.md](INDEX.md) | Every repository, component and public index, and where to find things |

## What's here

```
mawadao/
├── website/       mawadao.com                                   → mawadao/frontend
├── agent/         mawaDao Agent: marketplace, member space and   → mawadao/mawadao-agent
│                  agent runtime (has its own submodules)
├── registry/      Community list of AI tools and agents          → mawadao/registry
├── supabase/      Database and sign-in for mawadao.com           → mawadao/supabase
└── org-profile/   The GitHub organisation profile                → mawadao/.github
```

## Three ways in

**Explore and learn.** Students, educators and anyone curious can browse AI tools on mawaDao,
with what each one costs for education, individuals and businesses. The list lives in
[`registry/`](registry) and anyone can add to it by pull request.

**Use agents.** Schools, orphanages, community educators, students and small businesses use
agents from the marketplace free of charge. Using agents in a larger organisation?
[Talk to us](https://mawadao.com/#contact).

**Build and contribute.** Developers list tools and agents, review them for safety, translate
them, and improve the platform itself in [`agent/`](agent). Not every contribution is code:
reviewing, translating and connecting schools matter just as much.

## Get everything

```bash
git clone --recurse-submodules https://github.com/mawadao/mawadao.git
cd mawadao
```

Already cloned? Run `git submodule update --init --recursive`. To move every part to its latest
`main`: `git submodule update --remote`.

Each folder is its own repository. Open issues and pull requests in the repository that owns the
code; [INDEX.md](INDEX.md) says which one that is.

## Contributing

Start with [CONTRIBUTING.md](CONTRIBUTING.md). In short:

- To list an AI tool or agent, open a pull request in [mawadao/registry](https://github.com/mawadao/registry).
- To change the platform, read [mawaDao Agent's contributing guide](https://github.com/mawadao/mawadao-agent/blob/main/CONTRIBUTING.md).
- To improve these pages, open a pull request here.

## Licence

Apache 2.0. See [LICENSE](LICENSE). Each repository carries its own licence and notices.

---

*Built by the community, owned by the community, for the children who need it most.*
