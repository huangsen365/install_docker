# check if there is any update on below page
https://github.com/docker/docker.github.io/tree/master/install/linux/docker-ce
# install_docker
mkdir /root/data1

yum install wget unzip -y

wget https://github.com/huangsen365/install_docker/archive/master.zip -O /root/data1/install_docker.zip

cd /root/data1

unzip install_docker.zip

cd /root/data1/install_docker-master

sh ./step1_Uninstall_old_versions.sh

sh ./step2_SET_UP_THE_REPOSITORY_part1.sh

sh ./step2_SET_UP_THE_REPOSITORY_part2.sh

sh ./step3_INSTALL_DOCKER_CE.sh

sh ./step4_START_ENABLED_DOCKER.sh

sh ./step5_HELLOW_WORLD.sh
