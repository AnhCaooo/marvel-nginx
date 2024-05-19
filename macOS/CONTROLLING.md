# Commands to control Nginx on macOS (with Homebrew)

### Install 

```bash
brew install nginx 
```

### Uninstall 

```bash
# Step 1: remove nginx
brew remove nginx 

# Step 2: remove nginx's files which are not removed from the previous command 
sudo rm -rf /opt/homebrew/etc/nginx
```

## Native commands 
**Note**: Please do not mix between native commands and Homebrew commands. Otherwise, you might get permission error when run Homebrew commands after native commands
### Start 

```bash
sudo nginx
```

### Stop 

```bash
sudo nginx -s stop
```

### Restart 

```bash
```

### Reload 

```bash
```

## Homebrew commands
**Note**: Please do not mix between native commands and Homebrew commands. Otherwise, you might get permission error when run Homebrew commands after native commands
### Start 

```bash
brew services start nginx
```

### Stop 

```bash
brew services stop nginx
```

### Restart 

```bash
brew services restart nginx
```

### Reload 

```bash
brew services reload nginx
```
