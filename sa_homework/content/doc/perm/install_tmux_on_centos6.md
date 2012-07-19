---
tags:
- blog
- nanoc
- sa
- writing
permalink: install_tmux_on_centos6.html
title: install tmux on centos6
toc: true
kind: article
created_at: Thu Feb 9 2012
author_name: andy
status: publish
---

#### 在centos 6.0 上安装tmux
* add RPMforge yum repo (64bit)

                rpm --import http://apt.sw.be/RPM-GPG-KEY.dag.txt  
                wget http://apt.sw.be/redhat/el6/en/x86_64/rpmforge/RPMS/rpmforge-release-0.5.2-2.el6.rf.x86_64.rpm  
                rpm -i rpmforge-release-0.5.2-2.el6.rf.*.rpm  

* install prerequisite for tmux

                yum install -y libevent

* install tmux

                yum --enablerepo rpmforge install -y tmux