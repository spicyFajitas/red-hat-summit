# Innovate in Linux and cloud-native development: Meet us upstream

Monday 1-2pm

Innovate in Linux and cloud-native development: Meet us upstream

At Red Hat, open source isn't just a development model—it's our engine for innovation. Join us for an exploration of the newest, coolest breakthroughs in open source Linux and cloud-native development, including bootc, Project Hummingbird, RISC-V, and our work with NVIDIA upstream. We'll discuss why upstream is where the real magic of innovation happens, you’ll leave with clear guidance on how to contribute to these projects and more alongside us.

Mark Russel, Senior Principal Product Manager - Technical, Red Hat

Colin Walters, Distinguished Engineer, Red Hat

Ben Breard, Senior Principal Product Manager - RHEL, Red Hat

Mike McGrath, Vice President, Core Platforms Engineering, Red Hat - first speaker

Scott Hebert, Senior Principal Software Engineer, Red Hat

Session type: Product roadmap
Mon, May 11th
1:00 PM - 2:00 PM EDT
B308-B309 - Level 3

## Notes

### Mike McGrath - Session Leader

Nagios - network/infra monitoring tool

https://nix.cz/en/ - guys shirt in front of me

Trust is everything - pace of change is continuing to speed up

Trust has two components - engineering trust, human/experience trust
    Québec bridge disaster - 75 people killed. Open source bridge designs could've helped spot this engineering flaw

AI is moving so fast. Open Source way to ensure it stays within guard rails

Red Hat core principles - innovate responsibly, be transparent, respect community

@ACTION - Fedora - published AI contribution policies

Image mode brings cloud tooling to the OS (bootc)

RHEL development - AI now triages issues, rebases packages, and backports fixes

### Colin Walters, Mark Russel speakers

RHEL Image mode elevator pitch

ComposeFS - new engine coming. Verify on disk integrity - talk on this later
Sealed image story? - 3:15. Ensure kernel matches cryptographic checksum
    Integrity sealing your entire operating system

OpenStacks talk?

Container registry distribution of updates is faster than RPM distribution

BCBK?

Bootc is a CNCF project now :tada:

universal blue project - bluefin, bazzite

New bootc features - download only flag, pre-stage image without rebooting into it, bandwidth constrained users `chunka` zstream chunked bootc / zstd:chunked

### Ben Breard, Scott Hebert speakers

Project Hummingbeard

Average 160 new CVEs per day :wowie:

Red Hat hardened images

@ACTION check if we're using red hat hardened images internally

Maintaining 0 CVEs across hardened images. Remove kernel, reduce image size, code included - remove unecessary code footprint, make SBOM smaller

Along build pipeline includes logfile with pinned images / SBOM

How long time to remediation for CVE fixes? RH can get packages out time to discovery, commit to repo and available to pull within a couple hours. GCC is a little longer, 15 hours

@ACTION Project Hummingbird / Fedora relationship? Lots of success with build system. What about OS level? Building project hummingbird on top of RHEL Image Mode. Fedora Hummingbird Linux!! - PCI compliant RHEL Image Mode VMs