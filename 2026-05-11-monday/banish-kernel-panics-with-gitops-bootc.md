# Banish kernel panics with a GitOps workflow for your nodes using bootc

We’ve all been burned by it: a routine operating system (OS) update breaks the GPU driver, a subtle configuration drift across nodes causes days of debugging, and the dream of a stable platform is crushed by the reality of managing a fleet of mutable, "pet" servers. While Kubernetes operators help manage components inside the cluster, they can't save us from the fragility of the underlying host operating system. How do we stop firefighting and start building truly resilient infrastructure? This session introduces a modern, declarative workflow using the CNCF project bootc. We will demonstrate how to treat your entire host OS—kernel, packages, and GPU drivers—as a single, immutable artifact defined in a version-controlled Containerfile. We will show you how, by integrating bootc with other tools like podman, you can develop a GitOps pipeline for your host OS and make critical driver updates become a simple, testable pull request. Come explore atomic, transactional rollouts live, so that failures mean an automatic rollback to the last known-good state, not a production outage. Together, we will demo and share a GitHub repo on how to get started with this model to scale your OS across multiple nodes and platforms. Join us to learn how to eradicate configuration drift, simplify host management, and bring the power of GitOps to the foundational layer of your Kubernetes cluster.

Clement Verna, Senior Manager, Red Hat

Preethi Thomas, Director, Global Engineering, Red Hat

Session type: Lightning talk
Mon, May 11th
4:40 PM - 5:00 PM EDT
B308-B309 - Level 3

## Talk

Not super relevant, this is focused on GPUs attached to RHEL servers. We run GPU nodes inside our OpenShift clusters. We can easily change driver container versions which will roll new pods. Or change operator version

Neat to see more applications of bootc though