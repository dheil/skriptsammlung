# Iterates over all Domains to find Wordpress Core files that have been altered and prints results to sysout

```bash
 ls /var/www/vhosts | xargs -n1 -I_percent -- sh -c "echo _percent && wp core verify-checksums --path='/var/www/vhosts/_percent/httpdocs'"
```
