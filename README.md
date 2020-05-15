# cPanel Exporter for Prometheus


Exports cPanel metrics to prometheus


## Flags
```
cpanel_exporter -h
Usage of cpanel_exporter:
  -interval string
        Check interval duration 60s by default (default "60")
  -interval_heavy string
        Bandwidth and other heavy checks interval, 1800s (30min) by default (default "1800")
  -port string
        Metrics Port (default "59117")
```

## Collectors

```
# HELP cpanel_bandwidth cPanel Metadata
# TYPE cpanel_bandwidth gauge
cpanel_bandwidth{user="aaaa"} 5.248831472e+10
# HELP cpanel_domains_configured Current Domains and Subdomains setup
# TYPE cpanel_domains_configured gauge
cpanel_domains_configured 375
# HELP cpanel_ftp_accounts cPanel FTP Accounts
# TYPE cpanel_ftp_accounts gauge
cpanel_ftp_accounts 119
# HELP cpanel_mailboxes_configured cPanel Mailboxes
# TYPE cpanel_mailboxes_configured gauge
cpanel_mailboxes_configured 27
# HELP cpanel_meta cPanel Metadata
# TYPE cpanel_meta counter
cpanel_meta{release="release",version="86.0 (build 19)"} 0
# HELP cpanel_plans cPanel Metadata
# TYPE cpanel_plans gauge
cpanel_plans{plan="DELUXE"} 9
cpanel_plans{plan="LITE"} 5
cpanel_plans{plan="PRO"} 3
# HELP cpanel_quota cPanel Disk Quota Percent
# TYPE cpanel_quota gauge
cpanel_quota{user="aaaa"} 8
cpanel_quota{user="bbbb"} 100
# HELP cpanel_sessions_email cPanel webmail session
# TYPE cpanel_sessions_email gauge
cpanel_sessions_email 17
# HELP cpanel_sessions_web cPanel session
# TYPE cpanel_sessions_web gauge
cpanel_sessions_web 10
# HELP cpanel_users_active Current Active Users
# TYPE cpanel_users_active gauge
cpanel_users_active 17
# HELP cpanel_users_suspended Current Active Users
# TYPE cpanel_users_suspended gauge
cpanel_users_suspended 6
```



