hi:
	echo hi
java:
	sudo yum install java-1.8.0-openjdk
tomcat:
	mkdir -p /opt/scratch
	(cd /opt/scratch; wget https://mirrors.gigenet.com/apache/tomcat/tomcat-9/v9.0.39/bin/apache-tomcat-9.0.39.tar.gz)
	(cd /opt/scratch ;  tar -xvf apache-tomcat-9.0.39.tar.gz)
	(sudo mv /opt/scratch/apache-tomcat-9.0.39 /usr/local/tomcat9)

geoserver:
	(cd /opt/scratch; wget http://sourceforge.net/projects/geoserver/files/GeoServer/2.15.1/geoserver-2.15.1-war.zip)
	(cd /opt/scratch; unzip geoserver-2.15.1-war.zip)
	(cd /opt/scratch; mv geoserver.war /usr/local/tomcat9/webapps/geoserver.war)
publish: 
	(cd .. ; make publish)

