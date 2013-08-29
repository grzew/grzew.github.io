---
layout: post
title:  "Installing nis server"
date:   2013-08-29 13:08:15
categories: ex423
---

In my preparations to ex423 I have used nis server installed on CentOS 5.7. 

Lab NIS domain name:
{% highlight bash %}
mylab
{% endhighlight %}

Installing NIS server:
{% highlight bash %}
[root@nissrv ~]# yum -y install ypserv
[root@nissrv ~]# ypdomainname mylab
[root@nissrv ~]# vim /etc/sysconfig/network
NETWORKING=yes
HOSTNAME=nissrv.exam.lab
NISDOMAIN=mylab


{% endhighlight %}


