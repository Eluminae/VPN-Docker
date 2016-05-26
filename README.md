# VPN-Docker

You just have to add some module to the host kernel.
``` sh
modprobe nf_conntrack_pptp nf_nat_pptp
```

Or make it permanent and do it just one time.
``` sh
echo nf_conntrack_pptp >> /etc/modules
echo nf_nat_pptp >> /etc/modules
```
