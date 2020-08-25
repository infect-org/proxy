# Install the envoy proxy system service

1. `sudo nano /etc/systemd/system/proxy.service`
2. paste the content of `proxy.service` into the file, change paths as required, save it
3. reload services `sudo systemctl daemon-reload`
4. enable the service `sudo systemctl enable proxy`
5. start the server `sudo systemctl start proxy`
6. check if proxy is running `sudo journalctl -fn 699 -u proxy`