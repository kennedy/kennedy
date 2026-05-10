### Hi there 👋

I build and maintain a bare-metal Kubernetes homelab — Go, Python, and a lot of YAML.

#### What I'm working on

- **[taloskubecluster](https://github.com/kennedy/taloskubecluster)** — Bare-metal Kubernetes homelab running Talos Linux with full GitOps via ArgoCD. 6 nodes (3 Intel control-plane + 3 ARM RK1 workers), Cilium CNI, cert-manager, Prometheus/Grafana, and a bunch of self-hosted apps.
- **[cert-manager-webhook-omglol](https://github.com/kennedy/cert-manager-webhook-omglol)** — Go webhook that solves DNS-01 ACME challenges via the omg.lol API for Let's Encrypt wildcard certs.
- **[cluster-status](https://github.com/kennedy/cluster-status)** — FastAPI service that queries Prometheus for cluster health and returns JSON for an Adafruit MagTag e-ink display.

#### Homelab stack

| Layer      | Tech                                          |
| ---------- | --------------------------------------------- |
| OS         | Talos Linux (immutable, API-driven)           |
| GitOps     | ArgoCD (app-of-apps)                          |
| CNI        | Cilium (eBPF, kube-proxy replacement)         |
| Ingress    | Traefik v3 + MetalLB L2                       |
| TLS        | cert-manager + custom omg.lol DNS-01 webhook  |
| Secrets    | External Secrets Operator + 1Password Connect |
| Monitoring | Prometheus + Grafana + Alertmanager + Loki    |
| Storage    | NFS (Synology NAS) + local-path (RK1 NVMe)    |
| Databases  | CloudNative-PG (PostgreSQL) + Garage (S3)     |

#### Self-hosted apps

[Immich](https://photos.kennedy.sh) · [Paperless-ngx](https://paperless.kennedy.sh) · [Audiobookshelf](https://audiobooks.kennedy.sh) · [Home Assistant](https://ha.cluster.kennedy.omg.lol) · [Pi-hole](https://pihole.cluster.kennedy.omg.lol/admin/login) · [Filestash](https://filestash.cluster.kennedy.omg.lol)

#### Project board

[Homelab](https://github.com/users/kennedy/projects/2) — tracking infra and app work across repos.

#### Links

- PGP: [`89F4 69BC 33FB 8F6E`](https://keybase.io/kennedy/pgp_keys.asc)
- [omg.lol proof](https://proven.lol/b61fbe)
