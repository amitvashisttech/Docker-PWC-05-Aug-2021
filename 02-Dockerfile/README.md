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


