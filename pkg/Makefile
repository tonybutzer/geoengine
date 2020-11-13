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

python:
	sudo yum install gcc openssl-devel bzip2-devel libffi-devel
	(cd /opt/scratch; sudo wget https://www.python.org/ftp/python/3.8.1/Python-3.8.1.tgz)
	(cd /opt/scratch; sudo tar xzf Python-3.8.1.tgz)
	(cd /opt/scratch/Python-3.8.1; sudo ./configure --enable-optimizations; sudo make altinstall)
	python3.8 --version


nodejs:
	echo more work needed here - see Readme.md
	#(cd /opt/scratch; curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash)
	#(cd /opt/scratch; sudo . ~/.nvm/nvm.sh)
	#sudo nvm install node
	#node -e "console.log('Running Node.js ' + process.version)"

docker:
	# Install Docker
	# Start the Docker Service
	# Add the ec2-user to the docker group so you can execute Docker commands without using sudo.
	sudo yum update -y
	sudo yum install docker -y
	sudo service docker start
	sudo usermod -a -G docker ec2-user


publish: 
	(cd .. ; make publish)

