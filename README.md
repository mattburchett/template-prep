# template-prep

Taken scripts from https://lonesysadmin.net/2013/03/26/preparing-linux-template-vms/

Notes: 

The thin script is kinda flaky. This seems to work better.

```bash
dd if=/dev/zero of=thin bs=1M
```

and for Ubuntu, make sure you use apt instead of yum and make sure that your system is set to regenerate the SSH keys upon boot.

in your rc.local file:
```bash
dpkg-reconfigure openssh-server
```



