# Awesome-Cloud-Infrastructure-Self-Hosted-PAAS

## Top Cloud Infrastructure & Self-Hosted PaaS Ecosystem



**Curated List of SaaS/Hosted Platforms & Open-Source GitHub Projects**  

*Focused on Self-Hosted Platform-as-a-Service (PaaS), Git-Push App Deployment, Docker/Kubernetes Orchestrators & Developer Cloud Platforms*  

**Last updated: November 2026**



This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **Cloud Infrastructure & Self-Hosted PaaS**. These tools deploy, scale, route, monitor, and manage web applications, databases, containers, and microservices across developer-friendly cloud PaaS providers and self-hosted VPS/bare-metal servers using Nixpacks/Buildpacks, Docker Compose, and Kubernetes.



**Examples** include Railway, Render, Fly.io, Heroku, DigitalOcean App Platform, Koyeb, Northflank, Porter, Coolify, CapRover, and karlo-ks/Infradeck (the category leaders and popular runtimes). 



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted Heroku/Railway/Render alternatives (`Coolify`, `Dokploy`, `CapRover`, `Dokku`, `karlo-ks/Infradeck`), Kubernetes-based open-source PaaS platforms (`Porter`, `Kubero`, `Cozystack`), and zero-downtime Docker deployment tools (`Kamal`) — ideal for indie hackers, DevOps/platform engineers, startup teams, and homelab self-hosters.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Support & Share](#support--share)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Platform-as-a-Service (PaaS) market is estimated at approximately **$133B–$196B** in 2026, expanding at an annual growth rate (CAGR) of ~15%–21% driven by cloud-native migration, containerization, and AI workloads. The sector exhibits a **barbell structure**: it is **highly concentrated** at the infrastructure foundation (dominated by hyperscalers like AWS, Azure, Google Cloud, and enterprise giants like Salesforce), while remaining **moderately fragmented** in the developer-facing application layer where specialized, indie-focused, and "neocloud" PaaS alternatives compete actively on developer experience (DX), edge performance, and simplicity.

## SaaS/Hosted Platforms

| Platform | Valuation / Company Scale | Starting Tier Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Heroku (Salesforce)](https://heroku.com)** | **$260B–$320B+** *(Parent Salesforce NYSE: CRM market cap; FY25 revenue ~$37.9B)* | **$5.00/month** (Eco dyno plan; $0.007/hr billed usage) | **No permanent free tier**; entry Eco pool provides **1,000 shared dyno hours/month** across personal apps (sleeps after 30 min inactivity; 512MB RAM cap). Basic always-on dynos start at $7/mo. | Pioneering cloud Platform-as-a-Service (PaaS) offering Git-based deployments, Buildpacks, managed Postgres/Redis add-ons, and simple horizontal dyno scaling. |
| **[DigitalOcean App Platform](https://digitalocean.com)** | **~$4.4B–$5.2B+** *(NYSE: DOCN market cap; FY25 revenue ~$901M)* | **$5.00/month** (Basic Shared CPU: 1 vCPU, 512MB RAM, 50GB transfer) | **Free forever plan** limited strictly to **static sites**: up to **3 static apps**, 1 GiB/month outbound data transfer, global CDN, and automated SSL (no container/database execution). | Managed PaaS built on DigitalOcean infrastructure enabling automated builds and deployments directly from GitHub/GitLab repositories and container registries. |
| **[Render](https://render.com)** | **$1.5B** valuation *(Series C unicorn; $258M total funding)* | **$7.00/month** (Individual Starter web service: 512MB RAM, 1 CPU, always-on) | **Free forever plan**: **750 instance hours/month** for web services (512MB RAM, spins down after 15 min idle, 30–60s cold start), free static site hosting, and 1GB Postgres (expires after 30 days). | Unified cloud application platform offering managed web services, static sites, cron jobs, private networking, and zero-downtime deployments via `render.yaml`. |
| **[Railway](https://railway.com)** | **Growth-stage** *(~$120M total funding; $100M Series B)* | **$5.00/month** (Hobby plan base fee; includes $5 usage credits, always-on execution, and custom domains) | **Free forever plan** with **$1/month recurring usage credit**, 1 project (up to 3 services, 0.5GB RAM & 1 vCPU each, sleeps after 5–10 min inactivity; no custom domains). New accounts receive a **30-day trial with a one-time $5 credit**. | Modern developer cloud PaaS featuring instant Git-push deployments, visual service canvases, built-in PostgreSQL/Redis databases, and usage-based infrastructure scaling. |
| **[Fly.io](https://fly.io)** | **~$100M–$467M** valuation *(~$110.5M total funding; Series C)* | **$2.19/month** (Micro VM: `shared-cpu-1x` 256MB RAM run 24/7; usage-based per second) | **7-day free trial** with **$1 starter credit** (no credit card required; up to 10 machines, 4GB RAM max, auto-stops after 5 min idle). Post-trial: **$0 bill waiver** for personal orgs whose total monthly usage is under $5. | Edge-first cloud application platform running Docker containers inside lightweight Firecracker microVMs close to users across global regions. |
| **[Northflank](https://northflank.com)** | **~$120M** estimated valuation *(~$24.9M total funding; Series A)* | **$2.70/month** (Micro container: 0.1 shared vCPU, 256MB RAM; pay-as-you-go) | **Free Developer Sandbox plan** (always-on): up to **2 running services**, **2 scheduled jobs**, **1 managed database addon** (PostgreSQL/Redis/MongoDB), and 1 BYOC cluster. | Full-stack cloud deployment platform uniting multi-cloud Kubernetes orchestration, CI/CD builds, preview environments, and managed databases. |
| **[Porter Cloud](https://porter.run)** | **Series A startup** *(~$21.5M total funding; $20M Series A)* | **$19.00/month baseline** ($13/mo per vCPU + $6/mo per GB RAM, prorated per minute + cloud provider cost) | **No permanent free tier or standalone trial credit pool**; operates on metered compute while deploying directly into the user's AWS/GCP/Azure account (utilizes user's underlying cloud credits). | Managed PaaS running directly inside your own AWS, GCP, or Azure account, combining a Heroku-like developer experience with underlying Kubernetes scalability. |
| **[Koyeb](https://koyeb.com)** | **Subsidiary of Mistral AI** *(Acquired Feb 2026; previously raised $8.6M; Mistral AI valued at $13.8B)* | **$29.00/month** (Pro plan base fee; includes $10 compute credit, NVMe storage, and priority builds) | **Free forever plan**: **1 web service** (512MB RAM, 0.1 vCPU, 2GB SSD, sleeps after 1 hour idle; Frankfurt/Washington DC) and **1 PostgreSQL database** (1GB storage, 5 hours active compute/month). | Developer-friendly serverless PaaS providing global edge deployment, auto-scaling, native GPU instances, and Git-driven container execution. |
| **[Coolify Cloud](https://coolify.io)** | **Bootstrapped / Open-Source** *(~$380k ARR / ~$32k MRR from cloud subscriptions & sponsorships)* | **$5.00/month** (Base cloud control plane; connects and orchestrates up to 2 external VPS servers) | **No free hosted cloud control plane** ($5/mo starting), but the underlying self-hosted open-source software is **100% free forever** on your own VPS with zero artificial feature limitations. | Official managed control-plane hosting for Coolify, allowing teams to connect and manage their own VPS servers without maintaining the Coolify dashboard instance. |





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
