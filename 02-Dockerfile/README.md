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

```
2140  ls
 2141  docker ps
 2142  curl  172.17.0.5:8081/info
 2143  curl  172.17.0.5:8081
 2144  curl  172.17.0.4
 2145  ip addr
 2146  docker network ls
 2147  docker network inspect 9c9176a54d13
 2148  docker ps
 2149  docker kill test-2 test-1
 2150  docker ps
 2151  docker ps -a
 2152  docker network inspect 9c9176a54d13
 2153*
 2154  docker run -d --name python-2 -p 8080:8081 python-web-app:v1
 2155  docker ps
 2156  curl localhost
 2157  curl localhost:8080
 2158  ip addr
 2159  docker ps
 2160  systemctl status docker
 2161  docker run -d --name python-3 -p 8080:8081 python-web-app:v1
 2162  docker run -d --name python-4 -P python-web-app:v1
 2163  docker ps
 2164  ls
 2165  cd 02-Dockerfile/
 2166  ls
 2167  cd python-web-app/
 2168  ls
 2169  cd ..
 2170  ls
 2171  docker images
 2172  docker run -d --name test-apache-1 -P myapache:v1
 2173  docker run -d --name test-apache-1 -P myapache:v2
 2174  docker run -d --name test-apache-2 -P myapache:v2
 2175  docker run -d --name test-apache-3 -P myapache:v3
 2176  docker ps
 2177  docker run -d --name test-apache-4 -p 8082:80  myapache:v1
 2178  docker run -d --name test-apache-5 -p 8083:80  myapache:v2
 2179  docker ps
```

```
2184  git add . ; git commit -m "Expose"; git push
 2185  ls
 2186  docker images
 2187  docker push python-web-app:v1
 2188  docker login
 2189  docker push python-web-app:v1
 2190  docker images
 2191  docker tag ce738ee1dfcf amitvashist7/python-web-app:v1
 2192  docker images
 2193  docker push amitvashist7/python-web-app:v1
 2194  docker logout
 2195  ls
 2196  docker imags
 2197  docker images
 2198  docker kill $(docker ps -aq)
 2199  docker rm $(docker ps -aq)
 2200  ls
 2201  docker images
 2202  docker rmi ce738ee1dfcf
 2203  docker rmi ce738ee1dfcf -force
 2204  docker rmi ce738ee1dfcf --force
 2205  docker images
 2206  docker logut
 2207  docker logout
 2208  docker run -d --name test-1-py amitvashist7/python-web-app:v1
 2209  docker ps
 2210  curl 172.17.0.2:8081
 2211  curl 172.17.0.2:8081/info
```
