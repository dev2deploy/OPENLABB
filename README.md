# OPENLABB

```diff
@@An opensource (premised) development lab for localized testing of modernizing, emergent technologies.@@
```
xxx
The repository is mostly focused on a modest kubernetes cluster with one control plane/node running all of our self hosted services and storage,
but it also serves as the Infrastructure-as-Code (IaC) for an entire homelab network and devices, to include: a VyOS gateway/firewall,
a couple of workstations, wireless devices, and a Ubiquiti Unifi switch.
Ultimately, this will include all applications for managing home IT systems.

# `devlab` build deets 
![dev2deploy-cover-1500x500](https://github.com/dev2deploy/OPENLABB/assets/170257998/7f375c7c-f1da-4cec-b0c6-00a9754268b0)

This **OPENLABB** Repository contains devlab documentation files: notes, setups, and configurations for infrastructure, applications, networking, +more.

> :warning: Be aware, products can change over time. We do our best to keep up with the latest changes and releases, but please understand that this won’t always be the case.

Info is created as free resources to be used in your own specific use cases. If you're searching for detailed, in-depth tutorials on some tools or technologies, check out our [YouTube Channel](https://www.youtube.com/@dev2deploy) or [BLOG](https://dev2deploy.io).

## `devlab` Features
Primary deployments and features within the devlab:  
- [x] OpenStack and Red Hat OpenShift as bare-metal hypervisors for AI-ML-HPC, blockchain and container development and testing
- [x] VyOS implemented as a firewall with Bitdefender Gravity Zone for security are deployed via Proxmox-Ceph ha-clusters
- [x] TrueNas Scale cluster has also been implemented as NAS
- [x] Kubernetes cluster deployment using kubeadm
- [x] Infrastructure Automation with Ansible to provision hosts, clusters, devices, etc.
- [x] Offline Root CA / Scripted PKI management using `openssl(1)`
- [x] Manage cluster state and apps using GitOps and ArgoCD
- [x] FreeIPA server
- [ ] RADIUS server
- [ ] Remote access via VPN

## `devlab` Getting Started

```console
python3 -m venv .venv
source .venv/bin/activate
pip install -U -r requirements.txt
ansible-galaxy collection install -U -r requirements.yaml
ansible-playbook homelab.yml
```

## `devlab` Tech Stack
|[Click Here](https://github.com/dev2deploy/OPENLABB/devlab-techstack/)|
|---|

## Contribution

As this is our personal devlab documentation, we do not accept any contributions. Feel free to fork the repository and use it for your own documentation.

## Other Resources

- [Dotfiles](https://github.com/christianlempa/dotfiles) - Our config files on macOS
- [Boilerplates](https://github.com/christianlempa/boilerplates) - Templates for various projects like Docker, K8S, Ansible, etc
- [Cheat-Sheets](https://github.com/christianlempa/cheat-sheets) - Command Reference for various tools and technologies
- [Videos](https://github.com/christianlempa/videos) - Documentation and project files for all our video tutorials on YouTube

## Support Us

Creating high-quality videos and valuable resources that are accessible to everyone, free of charge, is a huge challenge. With your contribution, we can dedicate more time and effort into the creation process, which ultimately enhances the quality of the content. So, all your support, by becoming a member, truly makes a significant impact on what we do. And you’ll also get some cool benefits and perks in return, as a recognition of your support.

Remember, ***supporting us is entirely optional.*** Your choice to become a member or not won't change your access to my videos and resources. You are also welcome to reach out to us on Discord, if you have any questions or feedback.

[https://www.patreon.com/dev2deploy](https://www.patreon.com/dev2deploy)




<h1 tabindex="-1" dir="auto" style="bottom-border:none;"><img src="https://camo.githubusercontent.com/0b88a728a74d44cb11f842cbed1cacb61f4d67f09b3dcf5926ac4767a1bb1c27/68747470733a2f2f692e696d6775722e636f6d2f7031527a586a512e706e67" width="144px" height="144px" align="left"/>

<!-- markdownlint-disable-next-line MD013 -->
<a id="user-content-homelab" class="anchor" aria-hidden="true" href="#homelab"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>
Homelab
</h1>

> K8S cluster built with Ansible and managed using ArgoCD for GitOps

<div align="center">

[![Discord](https://img.shields.io/badge/discord-chat-7289DA.svg?maxAge=60&style=flat-square&logo=discord)](https://discord.gg/DNCynrJ)&nbsp;&nbsp;&nbsp;
[![k8s](https://img.shields.io/badge/k8s-v1.29.2-blue?style=flat-square&logo=kubernetes)](https://k8s.io/)&nbsp;&nbsp;&nbsp;
[![debian](https://img.shields.io/badge/debian-bookworm-C70036?style=flat-square&logo=debian&logoColor=C70036)](https://debian.org)&nbsp;&nbsp;&nbsp;
[![GitHub last commit](https://img.shields.io/github/last-commit/clearlybaffled/homelab/main?style=flat-square&logo=git&color=F05133)](https://github.com/clearlybaffled/homelab/commits/main)

[![WTFPL](https://img.shields.io/github/license/clearlybaffled/homelab?style=flat-square&color=darkred)](http://www.wtfpl.net/)&nbsp;&nbsp;&nbsp;
[![Linters](https://github.com/clearlybaffled/homelab/actions/workflows/linters.yaml/badge.svg)](https://github.com/clearlybaffled/homelab/actions/workflows/linters.yaml)&nbsp;&nbsp;&nbsp;
[![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/clearlybaffled/homelab?style=flat-square)](https://libraries.io/github/clearlybaffled/homelab)
</div>
<br/>

# 🍇 Cluster

## Infrastructure Automation

Host buildout is handled by [Ansible][ansible-uri] automation.
The whole lab is built out from a [top level playbook](./homelab.yml), with segment specific playbooks under the [`playbooks/`](./playbooks/) directory.
(As a convention, all Ansible yaml files are suffixed `.yml` to allow VSCode to distinguish between those and all other yaml files.)
The full task list can be found in the [infrastructure](./infrastructure/README.md) folder, but as an overview, it will:

- Install system packages and any other necessary system related setup
- Pull down cluster images and binaries
- Install container runtime and start kubelet
- Run `kubeadm` to setup to create cluster
- Creates a separate user to continue setting up the cluster with to get away from using the admin credentials
- Applies CNI configuration
- Generates Application files for every cluster app and drops them into [`cluster/bootstrap`](./cluster/bootstrap) and Kustomization files into[`cluster/apps`](./cluster/apps) for the respective apps
- Bootstraps the cluster by starting ArgoCD and then applying [`cluster/cluster.yaml`](./cluster/cluster.yaml)

## GitOps

[ArgoCD][argocd-uri] watches all subfolders under the [`cluster`](./cluster) folder (see Directories below) and makes the changes to my cluster based on the YAML manifests.

The way Argo works for me here is (almost) every file in the [`cluster/bootstrap`](./cluster/bootstrap) directory will define an `argoproj.io/v1alpha1/Application` that points to a corresponding folder under [`cluster/apps`](./cluster/apps).
The `Application` will apply any manifest files it finds in that directory,
in addition to any Helm Charts or Kustomizations [that may also be defined](https://argo-cd.readthedocs.io/en/stable/user-guide/multiple_sources/) within the `Application`'s spec.
One or more Helm `values.yaml` files are in each directory and each helm definition in the `Application` refers to the specific values file to apply to that chart.

## Directories

This Git repository contains the following top level directories.
<!-- markdownlint-disable MD013 -->
```sh
📁 cluster         # Kubernetes cluster defined in code
├─📁 apps          # Apps deployed into my cluster grouped by namespace
├─📁 argocd        # Main Argo configuration of repository
└─📁 bootstrap     # Cluster initialization flies (Argo Applications) also grouped by namespace
📁 infrastructure  # Ansible files
├─📁 inventory     # Defines Host configurations and widest scoped variables
├─📁 pki           # Self-signed CA and subordinate CA certs for whole house and cluster
├─📁 roles         # Ansible roles that define the actual steps to accomplish these tasks
└─📁 terraform     # Terraform config for building VM hosts
📁 playbooks       # Ansible playbooks
```
<!-- markdownlint-enable MD013 -->

# 🎩 Tip of the Cap:

- [cloudconsulted](https://github.com/cloudconsulted)
- [röötfoo](https://github.com/R00TFOO)
- [ChristianLempa/homelab](https://github.com/ChristianLempa/homelab)
- [clearlybaffled/homelab](https://github.com/clearlybaffled/homelab)
- [bjw-s/home-ops](https://github.com/bjw-s/home-ops)
- [onedr0p/home-ops](https://github.com/onedr0p/home-ops)
- [khuedoan/homelab](https://github.com/khuedoan/homelab)
- [gruberdev/homelab](https://github.com/gruberdev/homelab)
- [RickCoxDev/home-cluster](https://github.com/RickCoxDev/home-cluster)
- [billimek/k8s-gitops](https://github.com/billimek/k8s-gitops)
- [blackjid/k8s-gitops](https://github.com/blackjid/k8s-gitops)
- [carpenike/k8s-gitops](https://github.com/carpenike/k8s-gitops)
- [K8s-At-Home Project](https://k8s-at-home.com)



[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=dev2deploy&repo=OPENLABB)](https://github.com/anuraghazra/github-readme-stats)
