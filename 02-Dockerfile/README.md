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
