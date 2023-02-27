# koha-docker-image

Start the container by:

sudo docker run --restart=always -e NO_MEMCACHED=true -v MYLOCALDIR:/var/lib/mysql -e INSTALL_LANG="tr-TR" -p 8081:8081 -p 8080:8080 -d --name koha --cap-add=SYS_NICE --cap-add=DAC_READ_SEARCH ravitejasravi/kohaserver


Get get the UI password

sudo docker exec -ti koha /opt/getpassword.sh
