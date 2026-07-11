# Arr-Projet 

## Create directory for the apps and data
sudo mkdir -p /volume1/docker/arr-apps/{radarr,sonarr,bazarr,lidarr,whisparr,prowlarr,qbittorrent,jellyfin,plex,goaccess}  
sudo mkdir -p /volume1/arr-data/{torrents/{tv,movies,music,books,complete,incomplete,adults},media/{tv,movies,music,books,adults}}

## Create the arr-user and give permission on arr-data
sudo useradd -m -s /bin/bash arr-user  
sudo passwd arr-user  
sudo chown -R 1001:1002 /volume1/arr-data /volume1/docker/arr-apps/  
sudo chmod -R a=,a+rX,u+w,g+w /volume1/arr-data /volume1/docker/arr-apps/  

## Obtain Plex claim token
Log in to: https://www.plex.tv/claim  
Copy the new token (it looks like claim-xxxxxx…)  


## Bazarr configuration  
https://youtu.be/skLrFDUOhrk?si=eCH1shODgR_ev7Zc
