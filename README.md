# pve-patch
PVE 去虚拟化(仅供学习) ，喜欢的话点个star吧

# xiaodi sec yyds NO.1

下载2个 releases安装包 传到服务器 然后执行下面的命令
```bash
# 安装QEMU
apt install -y pve-qemu-kvm=9.0.2-2
dpkg -i pve-qemu-kvm_9.0.2-2_amd64.deb

# 安装edk2
dpkg -i pve-edk2-firmware-ovmf_4.2023.08-4_all.deb

# 设置args信息 <100 为PVE的VM ID 可自行调整>
qm set 100 -args '-cpu host,hypervisor=off,vmware-cpuid-freq=false,enforce=false,host-phys-bits=true'

# 下一步就是重装windwos去吧(防止注册表残留信息)
```

使用文档参考飞书: 

https://uehkns5636.feishu.cn/docx/JhJHdw4X6ofYC7xq94IcwQBbnpf?from=from_copylink


PVE去虚拟化，在原版基础上实现了众多传感器设备
![image](https://github.com/user-attachments/assets/1c7e44bf-e0c0-4e0c-a7dd-64fe0b81a8ea)




# Awesome Proxmox VE

![Proxmox VE](https://www.proxmox.com/images/proxmox/Proxmox-logo-800.png)

This repo is a collection of **AWESOME** [Proxmox VE](https://pve.proxmox.com) documentation and tools for **any users/developers**.

Feel free to **contribute** / **star** / **fork** / **pull request** . Any **recommendations** and **suggestions** are welcome.

# License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

The [Proxmox VE](https://pve.proxmox.com)

## Table of Contents

- [Api](#api)
- [Article](#article)
- [Blog](#blog)
- [Documentation](#documentation)
- [Site](#site)
- [Tools](#tools)
- [Video](#video)

## Api
- [Proxmox API](https://pve.proxmox.com/wiki/Proxmox_VE_API) Proxmox Documentation API

- go
  - [proxmox-api-go](https://github.com/Telmate/proxmox-api-go) Consume the proxmox API in golang

- .Net
  - [cv4pve-api-dotnet](https://github.com/Corsinvest/cv4pve-api-dotnet) Proxmox VE Client API .Net C#
  - [ProxmoxSharp](https://github.com/ionelanton/ProxmoxSharp) Proxmox C# API client

- Php
  - [cv4pve-api-php](https://github.com/Corsinvest/cv4pve-api-php) Proxmox VE Client API PHP
  - [ProxmoxVE](https://github.com/ZzAntares/ProxmoxVE) This PHP 5.5+ library allows you to interact with your Proxmox server API.
  - [pve2-api-php-client](https://github.com/CpuID/pve2-api-php-client) Proxmox 2.0 API Client for PHP

- Java
  - [cv4pve-api-java](https://github.com/Corsinvest/cv4pve-api-java) Proxmox VE Client API JAVA
  - [pve2-api-java](https://github.com/Elbandi/pve2-api-java) Proxmox 2.0 API Client for Java

- Python
  - [Proxmoxer](https://pypi.org/project/proxmoxer/) Python Wrapper for the Proxmox 2.x API (HTTP and SSH)
  - [pyproxmox](https://pypi.org/project/pyproxmox/) Python Wrapper for the Proxmox 2.x API
  - [Proxmoxia](https://github.com/baseblack/Proxmoxia) Yet another Python wrapper for the Proxmox REST API.

- Perl
  - [Net-Proxmox-VE-0.006](https://metacpan.org/release/DJZORT/Net-Proxmox-VE-0.006) Pure perl API for Proxmox virtualization
  
- Ruby
  - [Proxmox](https://github.com/nledez/proxmox) You need to manage a proxmox host with Ruby? This library is for you.
 
- NodeJs
  - [Proxmox](https://www.npmjs.com/package/proxmox) node.js proxmox client
  - [cv4pve-api-javascript](https://github.com/Corsinvest/cv4pve-api-javascript) Proxmox VE Client API Javascript

- PowerShell
  - [cv4pve-api-powershell](https://github.com/Corsinvest/cv4pve-api-powershell) 

## Article
- [Setup Docker on Proxmox VE Using ZFS Storage](https://www.servethehome.com/setup-docker-on-proxmox-ve-using-zfs-storage/)
- [Recommended settings for Windows 10 and 2019 Server on Proxmox](https://davejansen.com/recommended-settings-windows-10-2016-2018-2019-vm-proxmox/)
- [Proxmox Training](https://github.com/ondrejsika/proxmox-training)
- [Proxmox: Automatische Snapshots einrichten](https://techlr.de/proxmox-automatische-snapshots-einrichten/)
- [Installing macOS 12 “Monterey” on Proxmox 7](https://www.nicksherlock.com/2021/10/installing-macos-12-monterey-on-proxmox-7/)

## Monitoring
- [Monitoring Proxmox with InfluxDB and Grafana in 4 Easy steps](https://www.linuxsysadmins.com/monitoring-proxmox-with-grafana/)
- [Efficient Proxmox monitoring with Checkmk](https://checkmk.com/blog/proxmox-monitoring)
- [Proxmox VE Monitoring](https://pandorafms.com/blog/proxmox-ve-monitoring/)

## Blog

- [pveCLI](https://pvecli.xuan2host.com/) article Proxmox VE
- [servethehome](https://www.servethehome.com/tag/proxmox-ve/) article Proxmox VE

## Documentation

- [Official Wiki](https://pve.proxmox.com) Index Wiki
- [Official Docs](https://pve.proxmox.com/pve-docs/) Index official documentation

## Site

- [Official Forum](https://forum.proxmox.com/) Official Forum
- [Git Developer](https://git.proxmox.com/?o=age) Git Developer Proxmox VE
- [Bugzilla](https://bugzilla.proxmox.com/) Bugzilla Proxmox VE
- [pve-devel](https://www.mail-archive.com/pve-devel@pve.proxmox.com/index.html) Mailing List Developer Proxmox VE
- [pve-user](https://www.mail-archive.com/pve-user@pve.proxmox.com/) Mailing List User Proxmox VE
- [cv4pve-tools](https://www.cv4pve-tools.com) cv4pve-tools Utility for Proxmox VE
- [cv4pve-metrics](https://metrics.cv4pve-tools.com) Metrics cloud for Proxmox VE
- [Reddit Proxmox](https://www.reddit.com/r/Proxmox/) Reddit
- [Reddit Proxmox VE](https://www.reddit.com/r/ProxmoxVE/) Reddit
- [Facebook Group](https://www.facebook.com/groups/proxmox/) Facebook Group

## Tools

- [cv4pve-autosnap](https://github.com/Corsinvest/cv4pve-autosnap) Automatic snapshot tool for Proxmox VE
- [cv4pve-barc](https://github.com/Corsinvest/cv4pve-barc) Backup And Restore Ceph for Proxmox VE
- [cv4pve-cli](https://github.com/Corsinvest/cv4pve-cli) Cli for Proxmox VE (Command Line Interfaces)
- [cv4pve-botgram](https://github.com/Corsinvest/cv4pve-botgram) Telegram Bot for Proxmox VE
- [cv4pve-diag](https://github.com/Corsinvest/cv4pve-diag) Diagnostic tool for Proxmox VE
- [cv4pve-node-protect](https://github.com/Corsinvest/cv4pve-node-protect) Proxmox VE protect configuration file nodes
- [cv4pve-pepper](https://github.com/Corsinvest/cv4pve-pepper) Launching SPICE remote-viewer having access VM running on Proxmox VE
- [cv4pve-metric](https://github.com/Corsinvest/cv4pve-metric) Metrics for Proxmox VE
- [cv4pve-metrics-exporter](https://github.com/Corsinvest/cv4pve-metrics-exporter) Metric exporter Prometheus for Proxmox VE
- [cv4pve-api-pwsh](https://github.com/Corsinvest/cv4pve-api-powershell) Power Shell for Proxmox VE
- [pve-cli-utils](https://github.com/aheahe/pve-cli-utils) ProxmoxVE Command Line Interface Utilities
- [proxmox-utils](https://github.com/remofritzsche/proxmox-utils) Useful shell (python) scripts for managing proxmox virtual environment.
- [proxmove](https://github.com/ossobv/proxmove) Migrate virtual machines between different Proxmox VE clusters
- [pvekclean](https://github.com/jordanhillis/pvekclean) Easily remove old/unused PVE kernels on your Proxmox VE system
- [xshok-proxmox](https://github.com/extremeshok/xshok-proxmox) proxmox post installation scripts
- [pve-patches](https://github.com/ayufan/pve-patches) Incremental backup
- [proxmox-tools](https://github.com/marrobHD/proxmox-tools) 📦 A collection of stuff that I wrote for Proxmox 📦
- [Proxmox-Launcher](https://github.com/domingoruiz/Proxmox-Launcher) Proxmox Launcher

## Video
- [Resizing Virtual Hard Drives in Proxmox](https://www.youtube.com/watch?v=hRP7u3QPNOM)
- [Creating a Ubuntu LXC in Proxmox for Docker](https://www.youtube.com/watch?v=1EYAGl96dZY&t)
- [Proxmox 6.1 and 6.2 PCIe Passthrough](https://www.youtube.com/watch?v=_fkKIMF3HZw)
- [Proxmox Monitoring Tools: InfluxDB2 + Grafana](https://www.youtube.com/watch?v=f2eyVfCTLi0)
