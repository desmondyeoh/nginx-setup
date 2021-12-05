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
