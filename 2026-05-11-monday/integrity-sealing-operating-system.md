# Integrity sealing your entire operating system

How do we prove our operating system (OS) hasn't been tampered with—not just at boot, but continuously at runtime? Integrity sealing answers this question by combining container-native Open Container Initiative (OCI) image workflows with a complete cryptographic chain of trust: customer-owned secure boot keys, signed unified kernel images, and composefs with fsverity for per-file verification on every access.

In this lightning talk, we'll cover how it works, who needs it (hint: anyone deploying to untrusted environments, meeting compliance mandates, or building zero-trust architectures), and how to get started. The technology is available upstream in bootc today and ships as a tech preview in Red Hat Enterprise Linux.

Mark Russel, Senior Principal Product Manager - Technical, Red Hat

Colin Walters, Distinguished Engineer, Red Hat

Session type: Lightning talk
Mon, May 11th
3:15 PM - 3:35 PM EDT
B308-B309 - Level 3

## Talk

composefs root digest

composefs + fs-verity on every read from disk

`/etc` and `/var` in a mutable state

LUKS volume encryption only if checksum of composefs is valid

Linux security module - [IPE](https://docs.kernel.org/next/admin-guide/LSM/ipe.html)

Trust chain - UEFI secure boot, systemd boot, unified kernel image, composefs + fs-verity

Building a sealed image - Generate keys, build rootfs, sign bootloader, flatten image, sign uki, verify

## Demo

`bcvk` package

verity hash checksum

cat /proc/cmdline

ls -lah /boot/EFI/Linux/bootc

findmnt /|cat

[`just` package](https://packages.fedoraproject.org/pkgs/rust-just/just/)

bootctl cmd/package