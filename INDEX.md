# Index

Where every part of mawaDao lives. Each repository is public and open to contributions.

## Repositories

| Folder here | Repository | What it is |
| --- | --- | --- |
| `website/` | [mawadao/frontend](https://github.com/mawadao/frontend) | mawadao.com: the public website (Next.js) |
| `supabase/` | [mawadao/supabase](https://github.com/mawadao/supabase) | Database schema and sign-in for mawadao.com |
| `mawa/` | [mawadao/mawa](https://github.com/mawadao/mawa) | mawa: the member space, community and agent runtime (the marketplace itself is on [mawadao.com](https://mawadao.com/marketplace)) |
| `registry/` | [mawadao/marketplace-registry](https://github.com/mawadao/marketplace-registry) | The community list of AI tools and agents, one YAML file per listing |
| `org-profile/` | [mawadao/.github](https://github.com/mawadao/.github) | The organisation profile shown on github.com/mawadao |
| (this repository) | [mawadao/mawadao](https://github.com/mawadao/mawadao) | Vision, mission, this index, and all of the above as submodules |

## Inside mawa

`mawa/` has its own submodules and folders. Its [README](https://github.com/mawadao/mawa#readme)
and [architecture](https://github.com/mawadao/mawa/blob/main/docs/architecture.md) explain them in full.

| Folder in `mawa/` | Repository | What it is |
| --- | --- | --- |
| `apps/frontend` | [mawa-frontend](https://github.com/mawadao/mawa-frontend) | Community, sign-up and the agent workspace. The marketplace lives on [mawadao.com](https://mawadao.com/marketplace) |
| `apps/dashboard` | [mawa-dashboard](https://github.com/mawadao/mawa-dashboard) | The member space at `agent.mawadao.com/<username>` |
| `runtime/gateway` | [mawa-gateway](https://github.com/mawadao/mawa-gateway) | Per-member agent runtime (OpenClaw-based) |
| `runtime/core` | [mawa-core](https://github.com/mawadao/mawa-core) | Lightweight agent runtime (PicoClaw-based) |
| `microservices/api` | [mawa-api](https://github.com/mawadao/mawa-api) | Main API: agents, communities, marketplace |
| `microservices/mission-control` | [mawa-mission-control](https://github.com/mawadao/mawa-mission-control) | Boards, tasks and approvals for teams of agents |
| `microservices/auth`, `channels`, `deployer`, `storage`, `skills`, `platform`, `manager` | in [mawa](https://github.com/mawadao/mawa/tree/main/microservices) | Sign-in, chat channels, provisioning, storage, skills catalogue, agent builder, runtime manager |
| `db` | [mawa-db](https://github.com/mawadao/mawa-db) | Shared database schema and migrations |

## Public indexes

| Index | Where | Updated |
| --- | --- | --- |
| AI tools and agents | `https://mawadao.github.io/marketplace-registry/index.json` | On every merge to the registry, and weekly for trending |
| Listing format | [registry/schema/listing.schema.json](https://github.com/mawadao/marketplace-registry/blob/main/schema/listing.schema.json) | With the registry |
| Container images | `ghcr.io/mawadao/mawa-<component>` | On each component release |

## Where do I…

| I want to… | Go to |
| --- | --- |
| List an AI tool or an agent | [mawadao/marketplace-registry](https://github.com/mawadao/marketplace-registry): copy a template and open a pull request |
| Report a safety concern about an agent | An issue in [mawadao/marketplace-registry](https://github.com/mawadao/marketplace-registry/issues) naming the agent |
| Report a security vulnerability | Private vulnerability reporting ("Report a vulnerability") on the affected repository |
| Fix or improve the marketplace, member space or runtime | [mawadao/mawa](https://github.com/mawadao/mawa) and its [contributing guide](https://github.com/mawadao/mawa/blob/main/CONTRIBUTING.md) |
| Change mawadao.com | [mawadao/frontend](https://github.com/mawadao/frontend) |
| Understand why mawaDao exists | [VISION.md](VISION.md) and [MISSION.md](MISSION.md) |

## Releases

Each repository is versioned on its own with tags. mawa's
[RELEASING.md](https://github.com/mawadao/mawa/blob/main/RELEASING.md) describes how
components and platform releases work.
