# Password protect with httpd

First create a .htpasswd file in the config directory:

```bash
$ htpasswd -c -B -b ./config/.htpasswd <user_name> <password>
```

After you have created a .htpasswd file build the image:

```bash
$ docker build -t httpd-password .
```

If the image is created, run it with the following command on http://localhost:8080/:

```bash
$ docker run -d --name httpd-password -p 8080:80 httpd-password
```
