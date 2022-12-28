# Creating MySQL container exposed to local network
To expose the MySQL container to an local port:
```
docker run -p 3306:[local_port] --name [name] -e MYSQL_ROOT_PASSWORD=[root_password] -d mysql[:tag]
```
