# Main docker compose templates for development
Faster project starts with this basic docker-compose templates.

For the ssl certificates, you should run this command on the certs folder:

```bash
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout <your-domain-name>.key -out <your-domain-name>.crt
```

# Vue Docker

Base template for Vue projects. Just place the code on the root directory and start. You should change the name of your hosts on the config files. W
It works with hot-relaoad.

For prevent the Header error, disable it on your vue.config.js:


```javascript
module.exports = {
	devServer: {
		disableHostCheck: true
	}
}
```
