# Repoken Agent Pack

A least-privilege Aeon skill for reading Repoken's public launch registry.

## Included skill

- `repoken-launches` — summarizes public launches from `https://repoken.fun/api/launches`.

The skill is read-only and disabled by default. It requests no Repoken secrets and returns its report in the run response, without local writes or notifications. It must not sign transactions, access wallets, post to social networks, deploy contracts, or write to Repoken. Instructions are not an enforced network sandbox: use an isolated instance without production secrets. Aeon's runtime still needs its usual model-provider configuration.

The pack is designed as a companion to the proposed Repoken ecosystem listing in Aeon's `docs/ECOSYSTEM.md`; it is not an official partnership until an upstream Aeon PR is accepted.

## Install

From an Aeon checkout:

```text
bin/install-skill-pack repoken/aeon-repoken-pack
```

Review before installation and enable it explicitly if desired; the suggested schedule is 09:00 UTC daily. No Aeon runtime execution has been verified yet. A public feed probe in this session did not receive an HTTP response, so live connectivity remains unverified.

An ecosystem listing, even if accepted, is not a partnership or endorsement. Currently this is a local draft, not a published or listed integration.
