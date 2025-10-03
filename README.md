# SANS Workshop: Shadow Steps: Understanding and Detecting User Impersonation and Lateral Movement in Active Directory

<div>
<img src="./sans-2025.jpg"/>
</div>

This hands-on, scenario-driven workshop delves into how attackers move stealthily through Active Directory environments using user impersonation and lateral movement techniques. Participants will explore how attackers exploit credentials and trust relationships to expand their access, and how defenders can detect, prevent, and respond to such threats.

Through simulated exercises and guided labs, participants will walk through real-world attack paths such as (over)Pass-the-Hash, Kerberoasting, and token impersonation.

Learning Objectives:

- Understand the key mechanisms behind user impersonation in Active Directory.
- Demonstrate how attackers perform lateral movement via tools and techniques such as:
- Pass-the-Hash
- Pass-the-Ticket/Overpass-the-Hash
- Remote Services Abuse (SMB, WMI, RDP, WinRM)\
- SOCKS PTH
- Kerberoasting
- Token Impersonation
- Token Creation
- This hands-on workshop is ideal for Penetration Testers with limited knowledge about AD internals.

### Access the workbook here:

- https://logout.gitbook.io/lateral-movement-in-ad-with-empire 

Submit a PR to add your writeup to this list :)

## Install dependencies

> No automatic install is provided as it depend of your package manager and distribution. Here are some install command lines are given for ubuntu.

## Installation

- Installation depend of the provider you use, please follow the appropriate guide :
  - [Install with VmWare](./docs/install_with_vmware.md) [comming soon]
  - [Install with VirtualBox](./docs/install_with_virtualbox.md)  [comming soon]
  - [Install with Ludus](./docs/install_with_ludus.md)
  - [Install with AWS](./docs/install_with_aws.md) (https://logout.gitbook.io/lateral-movement-in-ad-with-empire)

- Installation is in three parts :
  1. Templating : this will create the template to use (needed only for proxmox) 
  2. Providing : this will instantiate the virtual machines depending on your provider
  3. Provisioning : it is always made with ansible, it will install all the stuff to create the lab

## Special Thanks to

- [Jean-François Maes](https://www.sans.org/profiles/jeanfrancois-maes/) for creating this SANS workshop
- M4yFly [@M4yFly](https://x.com/M4yFly) for the amazing GOAD porject and ansible playbooks (This repo is based on the work of [Mayfly277](https://github.com/Orange-Cyberdefense/GOAD/))
- [BC-SECURITY](https://github.com/BC-SECURITY/) team for their awesome tool Empire and StarKiller
- [Bad Sector Labs](https://x.com/badsectorlabs) for testing the code and guidance
- [Elastic Security](https://www.elastic.co/security) for their awesome SIEM and Stack
