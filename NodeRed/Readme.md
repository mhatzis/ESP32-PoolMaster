1. Read up on node red and what it is if your a noob like me.
######################################

I used a raspberry pi and installed influx DB, Grafana and Node-red.
your going to have some issues with node red. make sure your up to date and npm is installed for the pallet manager. In Node red you will need to make sure the floowing are instlled

node-red-contrib-influxdb 0.6.1
node-red 2.2.2
node-red-contrib-ui_j. 1.2.19
node-red-dashboard 3.1.7

import json file to node red.
##############################
conenct to gui http://IP:1880

click on the three lines top right and select import.
Past the nodered file here.
once imported you will need to change influxdb connect (username and password) and the MQTT credentails in the "All JSON from PoolMaster" & "MQTT Broker"



InfluxDb
########

create a db called POOL (case sensative)
Create a user pi. and asign a password 


if you have it configured correctly use 'show FIELD KEYS' within teh influx CLI to see whats the db is posulated with.  


Grafana
#######

Once installed connect to http://IP:3000
admin/admin

on the left click the '+' symbol and click import. Paste the Grafana json file in here.  
add a data source influxdb and configure credentials




