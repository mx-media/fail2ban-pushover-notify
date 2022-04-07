# fail2ban-pushover-notify

curl required

# example jail

[sshd]

port    = ssh  
logpath = %(sshd_log)s  
backend = %(sshd_backend)s  
action  = pushover #pushover notify on startup,exit,ban & unban  
          iptables-allports #bans all ips with iptables  
