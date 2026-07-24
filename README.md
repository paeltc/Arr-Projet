# Arr-Projet 

## Create directory for wireshark
sudo mkdir -p /volume1/docker/wireshark/{config,captures}  

## Create the wireshark and give permission on wireshark
sudo useradd -m -s /bin/bash wireshark 
sudo passwd wireshark  
sudo chown -R wireshark:users /volume1/docker/wireshark 
sudo chmod -R a=,a+rX,u+w,g+w /volume1/docker/wireshark 

