#Overview
This container is to keep the DNS response for the IP address up to date. It requires a configuration file to be already created and passed through.

The configuration file can be set up by using either:

(non-interactive)
```bash
/usr/local/src/noip-2.1.9-1/noip2 -C -U {update_interval} -u {user_name} -p {password} -I {network_interface}
```
or
(interactive)
```bash
/usr/local/src/noip-2.1.9-1/noip2 -C
```

##Docker Run
The container should be run with the following commands to allow for the config file to be passed through.
```bash
docker run -itd -v /usr/local/etc/no-ip2.conf:/usr/local/etc/no-ip2.conf --name {container_name} {image_name}
```
