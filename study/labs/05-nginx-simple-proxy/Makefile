help:
	docker swarm init

up:
	docker-compose up

down:
	docker-compose down


stop-tomcat:
	/usr/local/tomcat9/bin/shutdown.sh


install-compose:
	sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
	sudo chmod +x /usr/local/bin/docker-compose


publish:
	(cd /opt/geoengine; make)
