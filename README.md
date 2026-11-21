# Awesome-Cloud-Infrastructure-Self-Hosted-PAAS

# Top Cloud Infrastructure & Self-Hosted PaaS Ecosystem

**Curated List of SaaS/Hosted Platforms & Open-Source GitHub Projects**  
*Focused on Self-Hosted Platform-as-a-Service (PaaS), Git-Push App Deployment, Docker/Kubernetes Orchestrators & Developer Cloud Platforms*  
**Last updated: November 2026**

This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **Cloud Infrastructure & Self-Hosted PaaS**. These tools deploy, scale, route, monitor, and manage web applications, databases, containers, and microservices across developer-friendly cloud PaaS providers and self-hosted VPS/bare-metal servers using Nixpacks/Buildpacks, Docker Compose, and Kubernetes.

**Examples** include Railway, Render, Fly.io, Heroku, DigitalOcean App Platform, Koyeb, Northflank, Porter, Coolify, CapRover, and karlo-ks/Infradeck (the category leaders and popular runtimes). 

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted Heroku/Railway/Render alternatives (`Coolify`, `Dokploy`, `CapRover`, `Dokku`, `karlo-ks/Infradeck`), Kubernetes-based open-source PaaS platforms (`Porter`, `Kubero`, `Cozystack`), and zero-downtime Docker deployment tools (`Kamal`) — ideal for indie hackers, DevOps/platform engineers, startup teams, and homelab self-hosters.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Support & Share](#support--share)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Railway](https://railway.com)**  
  Modern developer cloud PaaS featuring instant Git-push deployments, visual service canvases, built-in PostgreSQL/Redis databases, and usage-based infrastructure scaling.

- **[Render](https://render.com)**  
  Unified cloud application platform offering managed web services, static sites, cron jobs, private networking, and zero-downtime deployments via `render.yaml`.

- **[Fly.io](https://fly.io)**  
  Edge-first cloud application platform running Docker containers inside lightweight Firecracker microVMs close to users across global regions.

- **[Heroku (Salesforce)](https://heroku.com)**  
  Pioneering cloud Platform-as-a-Service (PaaS) offering Git-based deployments, Buildpacks, managed Postgres/Redis add-ons, and simple horizontal dyno scaling.

- **[DigitalOcean App Platform](https://digitalocean.com)**  
  Managed PaaS built on DigitalOcean infrastructure enabling automated builds and deployments directly from GitHub/GitLab repositories and container registries.

- **[Koyeb](https://koyeb.com)**  
  Developer-friendly serverless PaaS providing global edge deployment, auto-scaling, native GPU instances, and Git-driven container execution.

- **[Northflank](https://northflank.com)**  
  Full-stack cloud deployment platform uniting multi-cloud Kubernetes orchestration, CI/CD builds, preview environments, and managed databases.

- **[Porter Cloud](https://porter.run)**  
  Managed PaaS running directly inside your own AWS, GCP, or Azure account, combining a Heroku-like developer experience with underlying Kubernetes scalability.

- **[Coolify Cloud](https://coolify.io)**  
  Official managed control-plane hosting for Coolify, allowing teams to connect and manage their own VPS servers without maintaining the Coolify dashboard instance.


## Open-Source GitHub Projects

- **[karlo-ks/Infradeck](https://github.com)**  
  Open-source self-hosted cloud infrastructure and PaaS management dashboard designed for streamlined application deployment, server orchestration, and container monitoring.

- **[Coolify (`coollabsio/coolify`)](https://github.com)**  
  Flagship open-source, self-hostable Heroku/Netlify/Vercel alternative enabling one-click deployments of apps, databases, and 280+ services on any VPS or Raspberry Pi via SSH.

- **[Dokploy (`Dokploy/dokploy`)](https://github.com)**  
  Modern open-source self-hosted PaaS built on Docker Swarm and Traefik featuring multi-server deployments, Nixpacks/Dockerfile builds, database backups, and real-time monitoring.

- **[CapRover (`caprover/caprover`)](https://github.com)**  
  Extremely easy-to-use open-source PaaS and web server manager powered by Docker, Nginx, and Let's Encrypt for one-click app and database deployments.

- **[Dokku (`dokku/dokku`)](https://github.com)**  
  Battle-tested, lightweight open-source mini-Heroku powered by Docker that turns any Linux server into a single-host `git push` PaaS with Buildpacks and plugin ecosystems.

- **[Porter (`porter-dev/porter`)](https://github.com)**  
  Open-source Kubernetes-powered PaaS transforming AWS EKS, GCP GKE, and Azure AKS clusters into an intuitive Heroku-style application platform.

- **[Kamal (`basecamp/kamal`)](https://github.com)**  
  Open-source zero-downtime deployment tool from 37signals that deploys containerized web applications and accessories across bare-metal VMs or cloud servers using Docker and Kamal Proxy.

- **[Kubero (`kubero-dev/kubero`)](https://github.com)**  
  Self-hosted open-source Heroku-compatible PaaS built natively on Kubernetes featuring GitOps pipelines, review apps, and multi-language buildpacks.

- **[Cozystack (`cozystack/cozystack`)](https://github.com)**  
  Free open-source PaaS and private cloud platform built on Talos Linux and Kubernetes for running managed databases, virtual machines, and tenant K8s clusters on bare metal.

- **[Ptah.sh (`ptah-sh/ptah-server`)](https://github.com)**  
  Open-source self-hosted PaaS engineered for deploying Docker Swarm services, managing SSL certificates, and orchestrating multi-node server clusters cleanly.

- **[Nixpacks (`railwayapp/nixpacks`)](https://github.com)**  
  Open-source build engine (created by Railway and used by Coolify/Dokploy) that automatically detects application source code and generates optimized OCI Docker images without a Dockerfile.

### Additional Strong Open-Source Options

- **[Paketo Buildpacks (`paketo-buildpacks`)](https://github.com)** for cloud-native open-source buildpacks converting application source code into secure, production-ready OCI container images.
- **[Traefik (`traefik/traefik`)](https://github.com)** and **[Caddy (`caddyserver/caddy`)](https://github.com)** for automatic HTTPS/Let's Encrypt reverse proxying and dynamic container service discovery.
- **[Komodo (`moghtech/komodo`)](https://github.com)** and **[Portainer (`portainer/portainer`)](https://github.com)** for self-hosted multi-server Docker Compose deployment, Git-sync automation, and container management UIs.
- **[Piku (`piku/piku`)](https://github.com)** for an ultra-lightweight, zero-Docker Python/uWSGI/Nginx `git push` PaaS capable of running on low-RAM ARM/Raspberry Pi boards.
- **[Cloudron (`cloudron-io/box`)](https://github.com)** and **[YunoHost (`YunoHost/yunohost`)](https://github.com)** for turnkey self-hosted app platforms automating DNS, SSL, backups, and SSO for self-hosted web apps.

**Frameworks for building custom systems**: Combine **Coolify** or **Dokploy** for full-featured self-hosted Railway/Heroku dashboards, **Kamal** for zero-downtime CLI Docker deployments across bare-metal servers, and **Nixpacks + Traefik** for automated builds and HTTPS routing.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Support & Share

If you find this curated list helpful, consider supporting the project:

- ⭐ **Star this repository** to help others discover it.
- 🍴 **Fork & Share** it with your team, friends, or community on X/Twitter, LinkedIn, and Reddit.
- ☕ **Buy me a coffee / Sponsor** my open-source work on [GitHub Sponsors](https://github.com) — featuring tiers for profile badges, README shoutouts, logo placements, and prioritized bug fixes/features!

[![Sponsor @ishandutta2007](https://shields.io)](https://github.com)

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Self-hosted PaaS platforms managing production servers require proper SSH key hardening, firewall rules (UFW/iptables), automated off-site database backups (S3/Backblaze B2), and regular host OS security patching.
- Always test zero-downtime rollbacks, health checks, and persistent volume mounts before migrating stateful production databases onto self-hosted PaaS setups.

---

**Made for indie hackers, DevOps/platform engineers, startup founders, homelab builders, and open-source contributors.**  
Let's make cloud infrastructure and self-hosted PaaS deployments more open, affordable, and developer-owned.
