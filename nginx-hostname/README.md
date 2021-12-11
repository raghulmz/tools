# nginx-display-hostname

nginx-display-hostname is a nginx image that displays the hostname of the container. Useful for troubleshooting docker/sockerswarm/k8s etc...

```bash
╭─raghulmz@Sudersans-MacBook-Pro.local ~/gitlab.awareup.com/nihaocloud/nihao-prod-terraform-eks-cluster  ‹main*›
╰─➤  docker run -d -p 80:80 --name nginx-display-hostname raghulmz/nginx-display-hostname
1a7aac927f09...
```

```bash
╭─raghulmz@Sudersans-MacBook-Pro.local ~
╰─➤  curl localhost:80/index.sh
<html><head>
<title>1a7aac927f09</title>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">
</head><body>
HOSTNAME : 1a7aac927f09
</body></html>
```

- [fcgiwrap](https://www.nginx.com/resources/wiki/start/topics/examples/fcgiwrap/)
