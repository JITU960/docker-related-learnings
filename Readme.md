1. start zookeeper and kafka docker-containers with following command

docker-compose -f kafka-docker-compose.yml up

2. Run "Docker ps" to list all docker containers currently running.

3. Go into kafka docker container with following command:

	docker exec it #image_hash /sh/bin

4. go to /opt/kafka/bin directory to see the available shell-scripts for kafka usage:

6. Followings are the commands to list and create topic

	kafka-topic --list --zookeeper zookeeper:2181

7. Run the following command in a dedicated terminal: 
	kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic topic_name

8. Run the following command in a dedicated terminal:

	kafka-console-producer --broker-list 127.0.0.1:9092 --topic topic_name.

	This will show a prompt with 'a'. Write anything on the prompt, it will be shown on the consumer terminal.


