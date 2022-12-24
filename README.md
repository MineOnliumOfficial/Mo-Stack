# MO STACK

Deploy the MineOnlium stack in two commands :)  

# Get started

* `git clone https://github.com/MineOnliumOfficial/Mo-Stack && cd Mo-Stack/`
* replace my address with yours in the `.env` file.
* `docker compose up` 
* ...profit?

# Services Rendered:
* [Grafana](https://grafana.com/): http://localhost:3001
* [Prometeus](https://prometheus.io/): (push gateway) : http://localhost:9091
* BlockExplorer: http://localhost:4000
* BlockExplorer API: http://localhost:8081
* Stratum Mining Server: http://localhost:50001
* [NGINX Proxy Manager](https://github.com/NginxProxyManager/nginx-proxy-manager): http://localhost:81


# Note to Windows users

If you would like to mine from your local network, one is required to create a proxy via WSL & the local network. 

This can be accomplished via the following command in an adminstrator command prompt. 
```
netsh interface portproxy add v4tov4 listenport=50001 listenaddress=0.0.0.0 connectport=50001 connectaddress=<forward-to-this-IP-address(wsl address)>
```
