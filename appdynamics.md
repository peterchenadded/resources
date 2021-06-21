# Overview
* 15 day free trial
* https://www.appdynamics.com/free-trial/
* https://data202106170231052.saas.appdynamics.com/ (A dedicated controller)

# Infrastructure Monitoring

* No curl commmand to download package

```
jre/bin/java -jar machineagent.jar
```

* Didn't see option to install as a systemctl service, even though it is in the documentation

![image](https://user-images.githubusercontent.com/10074427/122390778-af2e2800-cfb5-11eb-9677-9c33fda56b77.png)

* Not sure why it didn't work

![image](https://user-images.githubusercontent.com/10074427/122393446-3bd9e580-cfb8-11eb-8602-45163d7f5f54.png)


# Distributed Tracing

```
JAVA_OPTS="${JAVA_OPTS} \
    -javaagent:${APP_HOME}/appdynamics/javaagent.jar"
```

* No idea what it has traced
    
<img width="1643" alt="Screen Shot 2021-06-17 at 11 43 35 pm" src="https://user-images.githubusercontent.com/10074427/122408585-db51a500-cfc5-11eb-9431-a574e1b382a5.png">

* Trace not representative

![image](https://user-images.githubusercontent.com/10074427/122408868-09cf8000-cfc6-11eb-9b84-23a3f2c846ec.png)

* Database calls

<img width="1392" alt="Screen Shot 2021-06-17 at 11 47 35 pm" src="https://user-images.githubusercontent.com/10074427/122409988-e953f580-cfc6-11eb-9f30-926382e0dd6d.png">

* Example trace

![image](https://user-images.githubusercontent.com/10074427/122411140-db52a480-cfc7-11eb-93ad-2b703719553b.png)

* Errors after shutdown down one container

![image](https://user-images.githubusercontent.com/10074427/122410695-7eef8500-cfc7-11eb-91c3-394c37e497a1.png)

* Error trace

![image](https://user-images.githubusercontent.com/10074427/122411475-21a80380-cfc8-11eb-94e8-d8e574f9c15a.png)


# Dashboarding

<img width="1282" alt="Screen Shot 2021-06-17 at 11 49 06 pm" src="https://user-images.githubusercontent.com/10074427/122409949-e2c57e00-cfc6-11eb-9d94-d0b456a59c30.png">

![image](https://user-images.githubusercontent.com/10074427/122409732-b9a4ed80-cfc6-11eb-899c-ea8155f423e7.png)


# Alerting

