# VPN-Docker

You just have to add some module to the host kernel.
``` sh
modprobe nf_conntrack_pptp nf_nat_pptp
```

Make it permanent and never do it again !
``` sh
sudo sh -c 'echo nf_conntrack_pptp >> /etc/modules'
sudo sh -c 'echo nf_nat_pptp >> /etc/modules'
```
And never forget to use MPPE-128bits encryption !
