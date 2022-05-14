# packed-ctf
A repository of Packer images and Ansible templates for building out vulnerable CTF targets for contests.

# Overview
The goal of this repository is to store automation scripts to allow for the quick and easy deployment of vulnerable target machines for Capture the Flag (CTF) contests.  The initial batch will focus on targets that can be uploaded to TryHackMe to allow for extended and more distributed use.  TryHackMe is restricted to AWS compatible images, which need to be one of the following operating systems:

| Operating System / Distribution | Supported versions (64 bit only) |
| ------------------------------- | ------------------ |
| Windows                         | Windows 7 or 2012 or newer (64 bit only) |
| Ubuntu                          | 12.04, 12.10, 13.04, 13.10, 14.04, 14.10, 15.04, 16.04, 16.10, 17.04, 18.04, 20.04 (64 bit only ) |
| Red Hat Enterprise Linux        | 5.1 - 5.11, 6.1 - 6.9, 7.0 - 7.3 |
| SUSE                            | SUSE Linux Enterprise Server 11 with Service Pack 1 and kernel 2.6.32.12-0.7, SUSE Linux Enterprise Server 11 with Service Pack 2 and kernel 3.0.13-0.27, SUSE Linux Enterprise Server 11 with Service Pack 3 and kernel 3.0.76-0.11,3.0.101-0.8, or 3.0.101-0.15, SUSE Linux Enterprise Server 11 with Service Pack 4 and kernel 3.0.101-63, SUSE Linux Enterprise Server 12 with kernel 3.12.28-4, SUSE Linux Enterprise Server 12 with Service Pack 1 and kernel 3.12.49-11, SUSE Linux Enterprise Server 12 with Service Pack 2 and kernel 4.4, SUSE Linux Enterprise Server 12 with Service Pack 3 and kernel 4.4 (64 bit only) |
| CentOS                       | 5.1 - 5.11, 6.1 - 6.6, 7.0 - 7.5, 8.0 - 8.2 (64 bit only) |
| Debian                       | 6.0.0 - 6.0.8, 7.0.0 - 7.8.0, 8.0.0 (64 bit only) |
| Oracle Linux | 6.1 - 6.6, 7.0 - 7.1 (64 bit only) |
| Fedora Server | 19 - 21 (64 bit only) |

Initially we'll include Ansible templates for one particular OS but the goal is to have one ready for each different repository structure (Yum / APT).

We'll likely also include binary packages ready to go for each supported OS as a lot of the OS versions supported are only available in archives, to preserve use should repositories disappear in the future.
