# High-performance, low-latency workloads on Red Hat OpenShift Virtualization at SiriusXM

In the broadcast and streaming industry, owning the most attractive content rights is not enough to stay competitive. To stand out, companies must provide end users with the best, near-real-time, innovative experience—without compromising on quality. SiriusXM was seeking a platform that would help it focus on innovation and modernization, and chose to adopt Red Hat OpenShift Virtualization.

Join this session with SiriusXM and Red Hat to explore how they migrated thousands of virtual machines (VMs) to Red Hat OpenShift Virtualization, while minimizing disruptions to their production environment. We’ll discuss key aspects of SiriusXM’s virtualization migration journey and beyond. You will learn how Red Hat OpenShift Virtualization can support your resource-intensive workloads, including:

Using an effective architecture for adopting REd Hat OpenShift Virtualization.
Optimizing VMs to run low-latency applications, including the role of storage.
Maximizing availability and workload density.
Establishing crucial quality control.

Juan Jose Floristan Jusue, OpenShift Principal Specialist SA, Virtualization, Red Hat

Grant McCarthy, Specialist Adoption Architect, Red Hat

Nate Mason, Director, Platform Operations, SiriusXM Pandora

Session type: Breakout session
Thu, May 14th
B404 - Level 4
8:30 AM - 9:10 AM EDT

## Talk

Migration toolkit for virtualization works flawlessly once network is set up properly. Completely migrated off VMware now

Feature requests from Sirius XM are being rolled into 4.22 OpenShift Virt

KubeVirt top 10 CNCF project with 100s of contributing companies

@ACTION search complete software stack offering slide (storage, DR, etc)

When conducting performance testing, define what high performance means for the workloads

understand the limiting factors and when they actually apply

Performance validation tools are more important than the tuning itself. How do we validate there is an issue?

Iterative testing to isolate variables

Tune the full stack:

- BIOS
- Node tuning operator
- machine config operator
- nmstate operator
- Hyper converged CR
- VM CR
- Qemu agent
- guest tuning


