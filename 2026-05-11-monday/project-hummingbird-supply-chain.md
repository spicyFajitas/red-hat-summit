# The Project Hummingbird supply chain: From open source to zero CVE container

Container images are plagued by Common Vulnerabilities and Exposures (CVEs), and supply chain attacks are becoming increasingly sophisticated. Project Hummingbird achieves nearly zero CVEs through hermetic builds, automation, and distroless design—and can update, build, and test hundreds of components per day. In this session, we’ll reveal how we build production-ready container images that maintain drop-in compatibility with popular upstream images while dramatically improving security. We’ll explore Red Hat’s product supply chain process for building these simple, distroless images that are ready to meet your security scanner and certification requirements, building on decades of experience creating open source software. We’ll also review Project Hummingbird’s fully autonomous supply chain, in which AI agents monitor upstream releases, detect vulnerabilities before CVEs are published, generate package updates, build across architectures, run tests, and ship patched images—all without human intervention after policies are set. The future of container security is here.

Scott Hebert, Senior Principal Software Engineer, Red Hat, Canadian

Ben Breard, Senior Principal Product Manager - RHEL, Red Hat, not Canadian lol

Session type: Lightning talk
Mon, May 11th
3:40 PM - 4:00 PM EDT
B308-B309 - Level 3

## Talk

Need velocity and minimization to speed up CVE remediation

Foundation of Project Hummingbird

Mono repo - 440 packages within a single GitLab repo

Upstream package metadata tracked in branches

Hermetic builds via mock and cryptographically signed before entering any image

Mass rebuilds across hundreds of packages in a single commit

Write the specification, let AI execute the development

[agents.md](https://gitlab.com/redhat/hummingbird/containers/-/blob/main/AGENTS.md?ref_type=heads) governs the agent operations across the monorepo

Konflux - Tekton based secure software factory

