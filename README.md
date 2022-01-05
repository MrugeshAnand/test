docker run infracloudio/csvserver:latest
docker logs eb
vi gencsv.sh
chmod +x gencsv.sh
docker run -d -v /home/mrugesh/Desktop/csvserver/solution/inputFile:/csvserver/inputdata infracloudio/csvserver:latest
docker inspect 63
docker stop 63
docker rm 63
docker run -p 9393:9300 -e CSVSERVER_BORDER=Orange -d -v /home/mrugesh/Desktop/csvserver/solution/inputFile:/csvserver/inputdata infracloudio/csvserver:latest
