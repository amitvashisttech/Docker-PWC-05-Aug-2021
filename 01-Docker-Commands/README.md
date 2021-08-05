```
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
 1052  git add . ; git commit -m "01-Docker"; git push 
 1053  ls
 1054  docker images 
 1055  docker pull centos
 1056  docker images 
 1057  docker run centos:7  date
 1058  docker images 
 1059  docker ps -a 
 1060  docker run centos:7  date
 1061  docker ps -a 
 1062  docker run centos:7  ps -ef
 1063  docker ps -a 
 1064  docker run amitvashist7/k8s-tiny-web
 1065  docker run -d amitvashist7/k8s-tiny-web
 1066  docker images 
 1067  docker pull amitvashist7/apache-ex4
 1068  docker login 
 1069  docker pull amitvashist7/apache-ex4
 1070  docker logout 
 1071  docker images 
 1072  ls
 1073  history > 01-Docker-Commands/README.md 
 1074  vim 01-Docker-Commands/README.md
 1075  ls
 1076  git add . ; git commit -m "01-Docker"; git push 
```

```
 1077  git pull
 1078  ls
 1079  rm 01-Docker-Commands/README.md 
 1080  git pull
 1081  git rm 01-Docker-Commands/README.md 
 1082  git pull
 1083  ls
 1084  cd ..
 1085  ls
 1086  rm -rf Docker-PWC-05-Aug-2021/
 1087  ls
 1088  git clone https://github.com/amitvashisttech/Docker-PWC-05-Aug-2021.git
 1089  ls
 1090  cd Docker-PWC-05-Aug-2021/
 1091  ls
 1092  history > 01-Docker-Commands/README.md 
 1093  vim README.md 
 1094  vim 01-Docker-Commands/README.md 
 1095  git add . ; git commit -m "01-Docker"; git push 
 1096  history 
```


```
 1097  docker images 
 1098  docker run -it ubuntu:16.04
 1099  docker run -itd ubuntu:16.04
 1100  docker ps 
 1101  docker ps -a
 1102  ls
 1103  docker run -itd --name appA-cont-1 ubuntu:16.04
 1104  docker run -itd --name appA-cont-2 ubuntu:16.04
 1105  docker run -itd --name appB-cont-2 ubuntu:16.04
 1106  docker run -itd --name appB-cont-1 ubuntu:16.04
 1107  docker ps 
 1108  docker attach appA-cont-1
 1109  ls
 1110  docker ps 
 1111  docker ps -a 
 1112  docker start appA-cont-1
 1113  docker ps -a 
 1114  docker attach appA-cont-1
 1115  ls
 1116  docker ps 
 1117  docker inspect appA-cont-2
 1118  docker ps 
 1119  docker stop appB-cont-2
 1120  docker kill appB-cont-1
 1121  docker ps 
 1122  docker ps -q
 1123  docker kill $(docker ps -q) 
 1124  docker ps 
 1125  docker ps -a
 1126  docker ps -aq
 1127  docker rm $(docker ps -aq) 
 1128  docker ps 
 1129  docker ps -a
 1130  ls
 1131  git pull 
 1132  ls
 1134  history > 01-Docker-Commands/README.md 

```
