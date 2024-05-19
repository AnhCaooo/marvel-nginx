# How to create a web server with Nginx in Mac (Apple Silicon)

Nginx stores its configuration files in `/opt/homebrew/etc/nginx/`. The main configuration file is `nginx.conf`. You can edit it using a text editor like nano, vim, etc. However, it's recommended to keep the original configuration untouched and create a new server block for your API gateway.

- **Step 1 (optional)**: Check if there is a folder located in Nginx configurations directory called `servers` or not. If not, create it: 

```bash
cd /opt/homebrew/etc/nginx/

mkdir servers
```

- **Step 2**: Navigate to `servers` directory 

```bash
cd /opt/homebrew/etc/nginx/servers
```

- **Step 3**: Create a new server block for API gateway. A common naming convention is to use your domain name (e.g., `api.example.com.conf`).
Check and replace your details with [API gateway][web-server-template] template as server block


- **Step 4**: Reload Nginx server and verify your work 

```bash
# Native ways: 
sudo nginx -s reload

```


[web-server-template]: https://github.com/AnhCaooo/marvel-nginx/tree/main/Sample/webServer.conf