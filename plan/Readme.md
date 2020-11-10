# Plan

# Document Steps
- install docker pkg docker-install.sh
- read instructions
	- https://my.usgs.gov/confluence/display/ErosGeoengine5/G5+v1.0.5+Deployment+to+UCSB
- load git repo from eros gitlab
	- git clone  https://eroslab.cr.usgs.gov/SCIENCE/geoengine5
	- FAIL permission problem - BUMMER!


## Java
- cd pkg
- make java
- java -version
```
java-1.8.0-openjdk
```
## Tomcat
- install Tomcat via makefile
- study apache tomcat

## Starting Tomcat

- cd /usr/local/tomcat9/bin
- startup.sh

## geoserver
- install geoserver from the makefile

## Nodejs

## Breakdown Other Install Items

## Analyze Code
- lines of code analysis
- graphviz analysis




# Notes

Hi, Tony:
I've given you access to our Confluence space EROS GeoEngine5.  Reza wrote up a page for UCSB to deploy our v1.0.5 and it is here:   https://my.usgs.gov/confluence/display/ErosGeoengine5/G5+v1.0.5+Deployment+to+UCSB

Those instructions may need to be tweaked for later releases although I haven't had a chance to look at that.  Our current release is tagged as v1.0.7, and I think you should start with that , as the database schema has several changes from v1.0.5.

Code base is in GitLab: https://eroslab.cr.usgs.gov/SCIENCE/geoengine5
You should be able to access it, let me or Michelle know if you have problems.

Thanks!



Cheryl Holen
KBR | Software Engineer III
KBR Contractor to the USGS Earth Resources Observation and Science (EROS) Center
Web https://www.usgs.gov/centers/eros
Office: +1 605.594.2923
Email: cholen@contractor.usgs.gov


"If you can't explain it simply, you don't understand it well enough" - Albert Einstein
