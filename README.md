<div align="center">

# Vaibhav Jain

Backend systems, forensics, and the occasional 80,000-camera architecture problem.

[![Portfolio](https://img.shields.io/badge/portfolio-jainvaibhav.me-black?style=flat-square)](https://jainvaibhav.me)
[![GitHub followers](https://img.shields.io/github/followers/VaibhavJain2609?style=flat-square&label=followers)](https://github.com/VaibhavJain2609)

</div>

I build systems that have to hold up under an adversary or a deadline — access
control that survives an audit, filesystem parsers that don't trust the disk,
and platform architectures that get load-tested rather than assumed. Currently
at National Forensic Sciences University, Gujarat.

## Building right now

**[PRAHARI](https://github.com/VaibhavJain2609/prahari)** — a statewide
CCTV registry and video-analytics platform for a state police hackathon
(~80,000 cameras, 26 departments, 34 districts). The design keeps video at
the edge and centralises only protobuf metadata — camera health, plates,
tracks, alerts — cutting projected backhaul 650× (160 Gbps → <250 Mbps) and
30-day storage 8,600× (52 PB → 6 TB/month) versus a naive central-VMS
design. Three planes (control / data / metadata), confusion-aware fuzzy
plate matching, spatio-temporal route feasibility gating, hash-chained
audit log. Deployed on Kubernetes via Helm + Terraform with a single
`profile` switch between a laptop and a rented GPU.

## Selected work

| | |
|---|---|
| **[btrfsparser](https://github.com/VaibhavJain2609/btrfsparser)** | Forensic BTRFS parser — walks the chunk tree and B-trees directly off a raw disk image to recover inodes, directory entries, and file contents from inline/compressed/regular extents, validating CRC32C along the way. Full technical writeup in the repo. |
| **MedConnect** | Multi-tenant clinic platform with an ABDM-compliant patient consent system (link codes, approval workflows, revocation). Resolved 12+ production issues — N+1 queries, race conditions, security misconfigurations. |
| **KK Society** | Member portal for a 970-member society. Audited and hardened RBAC and rate limiting across 90+ endpoints, closing broken access control and DoS exposure; built a stateful service-request workflow and a RazorPay integration for member collections. |
| **[Wikipedia Search Engine](https://github.com/VaibhavJain2609/Wikipedia_Search_Engine)** | tf-idf ranking combined with PageRank over the article link graph, over a local Wikipedia dump. |

More at **[jainvaibhav.me](https://jainvaibhav.me)** — every project there ships with a real
screenshot or it doesn't get one; no stock images standing in for client work.

## Toolbox

`Python` `TypeScript` `FastAPI` `Next.js` `PostgreSQL` `PostGIS` `Docker` `Redis`
· filesystem & memory forensics (Volatility 3), RBAC/audit design, gRPC/protobuf services

## Stats

<div align="center">
<img height="165em" src="https://github-readme-stats.vercel.app/api?username=VaibhavJain2609&show_icons=true&theme=default&hide_border=true&count_private=true" />
<img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=VaibhavJain2609&layout=compact&hide_border=true" />
</div>
