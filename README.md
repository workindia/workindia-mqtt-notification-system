# workindia-mqtt-notification-system
WorkIndia Notification System Created Based on MQTT Protocol



# mosquitto-server

Its a broker to maintain light weight connections with the clients like Android device or IOT devices.
For demo purpose, we have created 3 mosquitto containers on different ports with ports exposed as

MQ1: mqtt://localhost:2083
MQ2: mqtt://localhost:2084
MQ3: mqtt://localhost:2085

Also, in order to change the password for mqtt broker
go to Dockerfile and change following line

'''
RUN mosquitto_passwd -b /etc/mosquitto/passwd <username> <password>
'''

In order to modify the configuration for mosquitto broker modify default.conf file in "dockerconfig/"

To Start the server run following command
'''
docker-compose up -d
'''
