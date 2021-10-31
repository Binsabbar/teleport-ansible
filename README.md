🚧 **WARNING: THIS IS STILL IN PROGRESS** 🚧

# Ansible Playbook for Teleport Setup

This repo contins a simple ansible playbook to quickly get started setting up Teleport cluster and optionally, create trusted clusters

# Note
There is an existing [Helm chart](https://goteleport.com/docs/kubernetes-access/helm/reference/#highavailabilityreplicacount). This playbook is intended for [VM/standalone deployment](https://goteleport.com/docs/getting-started/linux-server/). The deployment is assuming [Trusted Cluster Architecture](https://goteleport.com/docs/setup/admin/trustedclusters/). Note that, the Root Cluster Proxy is deployed separately from Root cluster Auth server. Whereas for all leaf clusters (which are behind FW), have Proxy and Auth SVCs deployed in the same VM.

## Reuirements
* Basic Teleport Knowledge
* Servers with SSH access to them (so Ansible can run plays).
* Ansible >= 2.9
* Coffee

## Play Variables
