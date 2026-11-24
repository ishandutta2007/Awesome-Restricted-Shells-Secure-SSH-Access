# Awesome-Restricted-Shells-Secure-SSH-Access
# Awesome-Restricted-Shells-Secure-SSH-Access

## Top Restricted Shells & Secure SSH Access Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Restricted Shells, SSH Bastion Hosts, Zero-Trust Privileged Access Management (PAM) & Session Auditing*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Restricted Shells & Secure SSH Access**. These tools enforce command allowlisting, chroot/jail isolation, ephemeral SSH certificates, session recording, and zero-trust infrastructure access across Linux servers, containers, and cloud environments.



**Examples** include Teleport, StrongDM, HashiCorp Boundary, BastionZero, CyberArk Alero, PrivX, Cloudflare Access, AWS Systems Manager Session Manager, Azure Bastion, Okta Privileged Access, and `rssh-org/rssh` (the category leaders). 



**Open-source emphasis**: This section is heavily expanded with every major active project for restricted login shells, self-hosted SSH bastion gateways, certificate authorities, and audit-logged terminal proxies — ideal for sysadmins, DevSecOps engineers, security architects, and infrastructure teams.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Teleport (Enterprise Cloud)](https://goteleport.com)**  

  Identity-native infrastructure access platform providing short-lived SSH certificates, role-based access control, and full session recording.



- **[StrongDM](https://strongdm.com)**  

  Zero-trust Privileged Access Management (PAM) platform centralizing SSH, RDP, Kubernetes, and database access with granular audit logs.



- **[HashiCorp Boundary (HCP)](https://hashicorp.com)**  

  Managed identity-based access control service enabling secure SSH and TCP sessions to dynamic hosts without exposing private networks or static credentials.



- **[BastionZero (Cloudflare)](https://cloudflare.com)**  

  Zero-trust infrastructure access solution using split-root-of-trust cryptography to eliminate static SSH keys and bastion hosts.



- **[CyberArk Remote Access (Alero)](https://cyberark.com)**  

  SaaS privileged access service combining zero-trust network access, biometric authentication, and session isolation for remote vendors and admins.



- **[SSH.COM PrivX](https://ssh.com)**  

  Keyless, on-demand privileged access management platform automating ephemeral SSH and RDP certificates across hybrid cloud infrastructure.



- **[Cloudflare Access (Zero Trust SSH)](https://cloudflare.comproducts/access/)**  

  Browser-rendered and CLI-proxied Zero Trust SSH gateway enforcing SSO identity checks before reaching origin servers.



- **[AWS Systems Manager Session Manager](https://amazon.com)**  

  Fully managed AWS capability providing auditable, IAM-authenticated browser and CLI shell access to EC2 instances without open inbound SSH ports.



- **[Azure Bastion](https://microsoft.com)**  

  Fully managed PaaS service providing secure TLS-tunneled SSH and RDP connectivity directly to Azure virtual machines without public IP addresses.



- **[Okta Privileged Access](https://okta.com)**  

  Cloud-native privileged access governance and ephemeral SSH certificate management integrated directly with Okta identity workflows.





## Open-Source GitHub Projects



- **[rssh-org/rssh](https://github.com)**  

  Classic open-source restricted shell for use with OpenSSH, allowing administrators to restrict users strictly to `scp`, `sftp`, `rsync`, `cvs`, or `rdist` without interactive shell access.



- **[lshell (Limited Shell)](https://github.com)**  

  Open-source Python-based restricted shell allowing fine-grained per-user allowlists of permitted commands, directories, SSH port forwarding, and session logging.



- **[Teleport (Open-Source Community Edition)](https://github.com)**  

  Open-source identity-aware access proxy and SSH Certificate Authority supporting MFA, RBAC, and searchable terminal session playback.



- **[HashiCorp Boundary (Open-Source)](https://github.com)**  

  Open-source identity-based access controller providing dynamic host discovery, session brokering, and credential injection for SSH workflows.



- **[Warpgate](https://github.com)**  

  Smart, lightweight open-source SSH, HTTPS, MySQL, and PostgreSQL bastion host written in Rust that requires zero client-side software.



- **[The Bastion (OVHcloud)](https://github.com)**  

  Hardened, authentication- and authorization-focused open-source SSH bastion with per-server ACLs, MFA, and tamper-evident ttyrec session recording.



- **[JumpServer](https://github.com)**  

  Popular open-source Privileged Access Management (PAM) bastion host providing Web Terminal, SSH/SFTP auditing, and fine-grained command filtering.



- **[Apache Guacamole](https://github.com)**  

  Clientless open-source remote desktop and SSH/Telnet gateway accessible entirely through an HTML5 web browser with full session recording.



- **[sshesame](https://github.com)**  

  Easy-to-set-up fake SSH server and restricted honeypot shell written in Go that logs every command, file transfer, and port-forwarding attempt.



- **[Cowrie](https://github.com)**  

  Medium-to-high interaction open-source SSH and Telnet honeypot featuring an emulated restricted filesystem and complete session replay logging.



- **[scponly](https://github.com)**  

  Alternative open-source restricted shell designed specifically to give remote users `scp` and `sftp` file transfer access without interactive shell execution.



- **[Jailkit](https://sessink.nl)**  

  Open-source suite of utilities for rapidly building and maintaining secure `chroot` jails with limited shells (`jk_lsh`) for SSH and SFTP users.



- **[Tlog](https://github.com)**  

  Open-source terminal I/O recording and playback package designed to capture restricted or privileged shell sessions into structured JSON logs for SIEM ingestion.



- **[Smallstep step-ca & step-ssh](https://github.com)**  

  Open-source online X.509 and SSH Certificate Authority for issuing short-lived, SSO-backed SSH user and host certificates.



- **[ssh-audit](https://github.com)**  

  Open-source SSH server and client configuration auditor checking key exchange algorithms, ciphers, MACs, and cryptographic hardening.



- **[Eternal Terminal (ET)](https://github.com)**  

  Open-source remote shell that automatically reconnects without interrupting terminal sessions over unstable networks while authenticating via SSH.



- **[Mosh (Mobile Shell)](https://github.com)**  

  Open-source remote terminal application bootstrapping over SSH with roaming support, intermittent connectivity resilience, and local echo prediction.



### Additional Strong Open-Source Options



- **[OpenSSH (`rbash` / `ForceCommand` / `internal-sftp`)](https://github.com)** for built-in restricted SFTP chroots, command-forced keys, and FIDO2 hardware-key authentication.

- **[Bubblewrap (`bwrap`)](https://github.com)** and **[Firejail](https://github.com)** for unprivileged Linux namespace and seccomp sandboxing around restricted user shells.

- **[sshportal](https://github.com)** for a lightweight, transparent SSH jump host configured via CLI commands and backed by SQLite/MySQL.

- **[Bastillion](https://github.com)** for an open-source web-based SSH console centralizing key management and administrative access across servers.

- Many community **PAM 2FA modules (`google-authenticator-libpam`)**, **eBPF syscall monitors (`Falco` / `Tracee`)**, and **restricted Git shells (`git-shell`)** for defense-in-depth SSH hardening.



**Frameworks for building custom systems**: Combine **OpenSSH (`ForceCommand` + `internal-sftp`)** or **Warpgate**, **Smallstep `step-ca`**, **Tlog**, and **Bubblewrap / Jailkit** with **rssh-org/rssh** or **lshell** for hardened, auditable, zero-trust SSH access.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Restricted shells (`rbash`, `rssh`, `lshell`) are notorious for breakout vectors if misconfigured (e.g., allowing editors like `vim`/`less`, tar checkpoints, or writable paths); always pair restricted shells with `chroot`, Linux namespaces, or read-only mounts.

- Test SSH configurations in a separate session before logging out to prevent administrative lockouts.



---



**Made for Linux sysadmins, DevSecOps engineers, security architects, and infrastructure defenders.**  

Let's make SSH access and shell environments more locked-down, auditable, and zero-trust.
