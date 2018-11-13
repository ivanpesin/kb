# firewalld

Port-forwarding based on destination IP address:

```
firewall-cmd --add-rich-rule='rule family="ipv4" destination address="1.1.1.1"
   forward-port port="8022" protocol="tcp"
   to-addr="2.2.2.2" to-port="22"'
```
