# dockerimages
working on arm
cd gerritview
download gerrit-3.2.3.war and rename to gerrit.war
docker build -t name:tag .
docker -itd --name gerrit --mount 'source=name,target=/var/gerrit' -p8080:8080 -p29418:29418 name:tag

