RiotKit server tweaking starter
===============================

Basic role to pre-configure RiotKit managed server.


Default variables
-----------------

```yamlex
# turns off Debian/Ubuntu automatic updates, as those updates often breaks applications in docker containers after docker upgrade
remove_unattended_upgrades: yes

# removes spies from hosting companies
remove_qemu_guest_agent: yes

# sets "journald" as logging driver for better performance and logs rotation managed by systemd
tune_docker: yes

# sets swapiness (for servers recommended is 10)
adjust_swappiness: yes
swappiness: 10
```
