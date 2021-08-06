```
 2005  cd 02-Dockerfile/
 2006  ls
 2007  cd apache/
 2008  ls
 2009  mkdir v1
 2010  ls
 2011  cd v1/
 2012  ls
 2013  vim Dockerfile
 2014  ls
 2015  docker build -t myapache:v1 .
 2016  docker images
 2017  docker run -d --name test-1 myapache:v1
 2018  docker ps
 2019  docker inspect test-1
 2020  curl 172.17.0.2
```

```
 2058  cd 02-Dockerfile/apache/v2
 2059  docker build -t myapache:v2 .
 2060  docker images
 2061  docker run -d --name test-2 myapache:v2
 2062  docker ps
 2063  curl 172.17.0.2
 2064  curl 172.17.0.3
```

```
2117  docker build -t python-web-app:v1 .
 2118  docker images
 2119  docker run -d --name python-1 python-web-app:v1
 2120  docker ps
 2121  docker inspect python-1
 2122  curl  172.17.0.5
 2123  docker ps
 2124  curl  172.17.0.5:8081
 2125  cat app.py
 2126  curl  172.17.0.5:8081
 2127  curl  172.17.0.5:8081/hello
 2128  curl  172.17.0.5:8081/info
```
