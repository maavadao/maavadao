# Index

Where every part of maavaDao lives. Each repository is public and open to contributions.

## Repositories

| Folder here | Repository | What it is |
| --- | --- | --- |
| `website/` | [maavadao/frontend](https://github.com/maavadao/frontend) | maavadao.com: the public website (Next.js) |
| `supabase/` | [maavadao/supabase](https://github.com/maavadao/supabase) | Database schema and sign-in for maavadao.com |
| `maava/` | [maavadao/maava](https://github.com/maavadao/maava) | maava: the member space, community and agent runtime (the marketplace itself is on [maavadao.com](https://maavadao.com/marketplace)) |
| `registry/` | [maavadao/marketplace-registry](https://github.com/maavadao/marketplace-registry) | The community list of AI tools and agents, one YAML file per listing |
| `maava-Community-Agents/` | [maavadao/maava-Community-Agents](https://github.com/maavadao/maava-Community-Agents) | maava Community Agents: open-source AI agents for sales, marketing and growth: an index with each agent as a submodule from its own `community-agent-<name>` repo |
| `ai-tools-directory/` | [maavadao/ai-tools-directory](https://github.com/maavadao/ai-tools-directory) | A directory of AI tools, sites and suites (open source or not), one TOML file per tool, with pricing flags and preview images read from each tool's own site |
| `open-source-ai-repos/` | [maavadao/open-source-ai-repos](https://github.com/maavadao/open-source-ai-repos) | A directory of open-source AI repos, one TOML file per repo, and the developers behind them |
| `org-profile/` | [maavadao/.github](https://github.com/maavadao/.github) | The organisation profile shown on github.com/maavadao |
| (this repository) | [maavadao/maavadao](https://github.com/maavadao/maavadao) | Vision, mission, this index, and all of the above as submodules |

## Inside maava

`maava/` has its own submodules and folders. Its [README](https://github.com/maavadao/maava#readme)
and [architecture](https://github.com/maavadao/maava/blob/main/docs/architecture.md) explain them in full.

| Folder in `maava/` | Repository | What it is |
| --- | --- | --- |
| `apps/frontend` | [maava-frontend](https://github.com/maavadao/maava-frontend) | Community, sign-up and the agent workspace. The marketplace lives on [maavadao.com](https://maavadao.com/marketplace) |
| `apps/dashboard` | [maava-dashboard](https://github.com/maavadao/maava-dashboard) | The member space at `agent.maavadao.com/<username>` |
| `runtime/gateway` | [maava-gateway](https://github.com/maavadao/maava-gateway) | Per-member agent runtime (OpenClaw-based) |
| `runtime/core` | [maava-core](https://github.com/maavadao/maava-core) | Lightweight agent runtime (PicoClaw-based) |
| `microservices/api` | [maava-api](https://github.com/maavadao/maava-api) | Main API: agents, communities, marketplace |
| `microservices/mission-control` | [maava-mission-control](https://github.com/maavadao/maava-mission-control) | Boards, tasks and approvals for teams of agents |
| `microservices/auth`, `channels`, `deployer`, `storage`, `skills`, `platform`, `manager` | in [maava](https://github.com/maavadao/maava/tree/main/microservices) | Sign-in, chat channels, provisioning, storage, skills catalogue, agent builder, runtime manager |
| `db` | [maava-db](https://github.com/maavadao/maava-db) | Shared database schema and migrations |

## Public indexes

| Index | Where | Updated |
| --- | --- | --- |
| AI tools and agents | `https://maavadao.github.io/marketplace-registry/index.json` | On every merge to the registry, and weekly for trending |
| maava Community Agents | `https://maavadao.github.io/maava-Community-Agents/index.json` | On every merge to maava-Community-Agents, and daily when an agent's repo changes |
| Open-source AI repos | `https://maavadao.github.io/open-source-ai-repos/index.json` | On every merge, and daily for stars |
| AI tools | `https://maavadao.github.io/ai-tools-directory/index.json` | On every merge, and daily |
| Contributors to open-source AI | `https://maavadao.github.io/open-source-ai-repos/contributors.json` | Daily; login, user id and commits only, with an opt-out |
| Listing format | [registry/schema/listing.schema.json](https://github.com/maavadao/marketplace-registry/blob/main/schema/listing.schema.json) | With the registry |
| Container images | `ghcr.io/maavadao/maava-<component>` | On each component release |

## Where do I…

| I want to… | Go to |
| --- | --- |
| List an AI tool or an agent | [maavadao/marketplace-registry](https://github.com/maavadao/marketplace-registry): copy a template and open a pull request |
| Build a maava Community Agent | [maavadao/maava-Community-Agents](https://github.com/maavadao/maava-Community-Agents): build it in its own repo from the template, then open a pull request adding it as a submodule |
| Suggest an AI tool | [maavadao.com/directory](https://maavadao.com/directory), or [maavadao/ai-tools-directory](https://github.com/maavadao/ai-tools-directory): `scripts/add_tool.py` and a pull request |
| Add an open-source AI repo | [maavadao/open-source-ai-repos](https://github.com/maavadao/open-source-ai-repos): copy `templates/repo.toml` and open a pull request |
| Report a safety concern about an agent | An issue in [maavadao/marketplace-registry](https://github.com/maavadao/marketplace-registry/issues) naming the agent |
| Report a security vulnerability | Private vulnerability reporting ("Report a vulnerability") on the affected repository |
| Fix or improve the marketplace, member space or runtime | [maavadao/maava](https://github.com/maavadao/maava) and its [contributing guide](https://github.com/maavadao/maava/blob/main/CONTRIBUTING.md) |
| Change maavadao.com | [maavadao/frontend](https://github.com/maavadao/frontend) |
| Understand why maavaDao exists | [VISION.md](VISION.md) and [MISSION.md](MISSION.md) |

## Releases

Each repository is versioned on its own with tags. maava's
[RELEASING.md](https://github.com/maavadao/maava/blob/main/RELEASING.md) describes how
components and platform releases work.
