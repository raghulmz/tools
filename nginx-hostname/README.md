# nginx-display-hostname

nginx-display-hostname is a nginx image that displays the hostname of the container.

```bash
╭─raghulmz@Sudersans-MacBook-Pro.local ~/gitlab.awareup.com/nihaocloud/nihao-prod-terraform-eks-cluster  ‹main*›
╰─➤  docker run -d -p 80:80 --name nginx-display-hostname raghulmz/nginx-display-hostname
7abed06d6c89...
```

```bash
╭─raghulmz@Sudersans-MacBook-Pro.local ~/gitlab.awareup.com/nihaocloud/nihao-prod-terraform-eks-cluster  ‹main*›
╰─➤  curl localhost:80/index.sh
<html><head>
<title>7abed06d6c89</title>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">
</head><body>
HOSTNAME : 7abed06d6c89
</body></html>
* Connection #0 to host localhost left intact
* Closing connection 0

```
