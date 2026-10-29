# FSD Terminus

Docker stack of the EPFL FSD [Terminus] server (TRMNL e-ink displays) and its
EWS room-booking companion apps.

Deployed with Ansible by [terminus.ops](https://github.com/dieg0000000/terminus.ops).

## Content

* `docker-compose.yml`: Caddy, Terminus (web + worker), Postgres, Valkey, EWS API and frontend
* `ews-api/`: room events API (Exchange Web Services)
* `ews-frontend/`: `/add-event` page

## Secrets

Not in this repository. Copy `.env.sample` to `.env` and `ews-api/.env.sample`
to `ews-api/.env`, then fill them in.

[Terminus]: https://github.com/usetrmnl/terminus
