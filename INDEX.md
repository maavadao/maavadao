# Index

Where every part of mawaDao lives. Each repository is public and open to contributions.

## Repositories

| Folder here | Repository | What it is |
| --- | --- | --- |
| `website/` | [mawadao/frontend](https://github.com/mawadao/frontend) | mawadao.com: the public website (Next.js) |
| `supabase/` | [mawadao/supabase](https://github.com/mawadao/supabase) | Database schema and sign-in for mawadao.com |
| `agent/` | [mawadao/mawadao-agent](https://github.com/mawadao/mawadao-agent) | mawaDao Agent: the marketplace, Explore AI tools, member space and agent runtime |
| `registry/` | [mawadao/registry](https://github.com/mawadao/registry) | The community list of AI tools and agents, one YAML file per listing |
| `org-profile/` | [mawadao/.github](https://github.com/mawadao/.github) | The organisation profile shown on github.com/mawadao |
| (this repository) | [mawadao/mawadao](https://github.com/mawadao/mawadao) | Vision, mission, this index, and all of the above as submodules |

## Inside mawaDao Agent

`agent/` has its own submodules and folders. Its [README](https://github.com/mawadao/mawadao-agent#readme)
and [architecture](https://github.com/mawadao/mawadao-agent/blob/main/docs/architecture.md) explain them in full.

| Folder in `agent/` | Repository | What it is |
| --- | --- | --- |
| `apps/frontend` | [mawadao-agent-frontend](https://github.com/mawadao/mawadao-agent-frontend) | Marketplace, Explore AI tools (`/tools`), community, sign-up |
| `apps/dashboard` | [mawadao-agent-dashboard](https://github.com/mawadao/mawadao-agent-dashboard) | The member space at `agent.mawadao.com/<username>` |
| `runtime/gateway` | [mawadao-agent-gateway](https://github.com/mawadao/mawadao-agent-gateway) | Per-member agent runtime (OpenClaw-based) |
| `runtime/core` | [mawadao-agent-core](https://github.com/mawadao/mawadao-agent-core) | Lightweight agent runtime (PicoClaw-based) |
| `microservices/api` | [mawadao-agent-api](https://github.com/mawadao/mawadao-agent-api) | Main API: agents, communities, marketplace |
| `microservices/mission-control` | [mawadao-agent-mission-control](https://github.com/mawadao/mawadao-agent-mission-control) | Boards, tasks and approvals for teams of agents |
| `microservices/auth`, `channels`, `deployer`, `storage`, `skills`, `platform`, `manager` | in [mawadao-agent](https://github.com/mawadao/mawadao-agent/tree/main/microservices) | Sign-in, chat channels, provisioning, storage, skills catalogue, agent builder, runtime manager |
| `db` | [mawadao-agent-db](https://github.com/mawadao/mawadao-agent-db) | Shared database schema and migrations |

## Public indexes

| Index | Where | Updated |
| --- | --- | --- |
| AI tools and agents | `https://mawadao.github.io/registry/index.json` | On every merge to the registry, and weekly for trending |
| Listing format | [registry/schema/listing.schema.json](https://github.com/mawadao/registry/blob/main/schema/listing.schema.json) | With the registry |
| Container images | `ghcr.io/mawadao/mawadao-agent-<component>` | On each component release |

## Where do I…

| I want to… | Go to |
| --- | --- |
| List an AI tool or an agent | [mawadao/registry](https://github.com/mawadao/registry): copy a template and open a pull request |
| Report a safety concern about an agent | An issue in [mawadao/registry](https://github.com/mawadao/registry/issues) naming the agent |
| Report a security vulnerability | Private vulnerability reporting ("Report a vulnerability") on the affected repository |
| Fix or improve the marketplace, member space or runtime | [mawadao/mawadao-agent](https://github.com/mawadao/mawadao-agent) and its [contributing guide](https://github.com/mawadao/mawadao-agent/blob/main/CONTRIBUTING.md) |
| Change mawadao.com | [mawadao/frontend](https://github.com/mawadao/frontend) |
| Understand why mawaDao exists | [VISION.md](VISION.md) and [MISSION.md](MISSION.md) |

## Releases

Each repository is versioned on its own with tags. mawaDao Agent's
[RELEASING.md](https://github.com/mawadao/mawadao-agent/blob/main/RELEASING.md) describes how
components and platform releases work.
