# MO STACK

Deploy the MineOnlium stack in two commands :)  

# Get started

* `git clone https://github.com/MineOnliumOfficial/Mo-Stack && cd Mo-Stack/`
* `docker compose up` 
* ...profit?

# Services Rendered:
* BlockExplorer: http://localhost:4000
* BlockExplorer API: http://localhost:8081
* Moth node: 8545(RPC) / 8456(WS) / 30303(P2P)


# Note to Windows users

If you would like to mine from your local network, one is required to create a proxy via WSL & the local network. 

This can be accomplished via the following command in an adminstrator command prompt. 
```
netsh interface portproxy add v4tov4 listenport=50001 listenaddress=0.0.0.0 connectport=50001 connectaddress=<forward-to-this-IP-address(wsl address)>
```
