# Update crontab

```
crontab -e
```

```
0 */12 * * * /bin/ash /root/update.sh
```

```
wget https://raw.githubusercontent.com/cryptodata-com/xiden-guardian-updater/master/update.sh
chmod +x ./update.sh
/etc/init.d/cron restart
echo 'alias update="/usr/bin/wget -O - https://raw.githubusercontent.com/cryptodata-com/xiden-guardian-updater/master/update-script.sh | /bin/ash"' >> /etc/profile
```
