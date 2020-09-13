# Vuln Labs

## Prerequisites:
- [VirtualBox](https://www.virtualbox.org/) or [VMware](https://www.vmware.com/) virtualization software
- [Packer](https://www.packer.io/) >= version 1.6

## Usage
1. Open a terminal and `cd` into the desired lab folder ex `cd vuln0`.
2. Build the lab for the desired platform ex: `packer build vuln0-vmware.json`.
3. Once the build has finished, import the image that was built. It will be expecting an IP address over DHCP.
4. Configure network adapters so that the attacking machine and victim machine can communicate on all ports.
5. Try to get root!

## Why Build the Images This Way?

Since users will have access to the exact Packer and Ansible scripts used to build the vulnerable machine, there is total transparency in the build process. It is encouraged for users to look over the build scripts after rooting the box to understand how it was built and configured.
