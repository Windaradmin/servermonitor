# servermonitor with Gmail
VPN server monitoring with MonIT and GMail.
More : https://mmonit.com/monit/documentation/monit.html

quick fix...

try :  
#monit -t
#Control file syntax OK

#monit start all

If you get :  Cannot create socket to [0.0.0.0]:2812 -- Connection refused

Please do a :
#sudo ufw allow 2812/tcp ; monit reload
#monit start all

More info : https://www.digitalocean.com/community/questions/2812-port-not-work-for-monit


