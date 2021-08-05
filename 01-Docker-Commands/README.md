 1019  ls
 1020  cd 00-Setup/
 1021  ./install-docker.sh 
 1022  ls
 1023  cd ..
 1024  ls
 1025  docker ps 
 1026  docker images 
 1027  docker run ubuntu:16.04 echo "Welcome to the world of Docker."
 1028  docker ps 
 1029  docker ps -a
 1030  docker rm $(docker ps -qa)
 1031  docker run ubuntu:16.04 echo "Welcome to the world of Docker."
 1032  docker images 
 1033  docker run ubuntu:16.04 echo "Hello World"
 1034  docker run busybox date 
 1035  docker run busybox ping -c10 google.com
 1036  docker ps 
 1037  docker ps -a 
 1038  docker ps 
 1039  docker run busybox date 
 1040  docker ps 
 1041  docker ps -a
 1042  docker run busybox ping -c2 google.com
 1043  docker ps -a
 1044  docker run -it ubuntu:16.04
 1045  docker ps 
 1046  docker ps -a
 1047  docker run -it ubuntu:16.04
 1048  docker ps -a
 1049  ls
 1050  history 
 1051  history  > 01-Docker-Commands/README.md
