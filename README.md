# nginx-setup

1. Create sites-available entry
```
sudo vim /etc/nginx/sites-available/APPNAME
```

2. link
```
sudo ln -s /etc/nginx/sites-available/APPNAME /etc/nginx/sites-enabled
```

3. run
```
sudo nginx -t
sudo systemctl restart nginx
```

## HTTPS setup
1. login to cloudflare add new entry
```
A APPNAME.dyeoh.com 116.12.55.160
```
2. create new cert using LetsEncrypt certbot.
```
sudo certbot --nginx -d APPNAME.dyeoh.com
```
