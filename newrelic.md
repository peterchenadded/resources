# Overview

* Newrelic one free forever
* 1 full access account
* 100gb per month of data
* Data center in US and Europe
* https://newrelic.com/platform

# Infrastructure monitoring

<img width="1640" alt="Screen Shot 2021-06-15 at 11 11 34 pm" src="https://user-images.githubusercontent.com/10074427/122058601-22f1f880-ce2f-11eb-95d5-36cbd1d66bca.png">

* Process monitoring

<img width="1371" alt="Screen Shot 2021-06-15 at 11 13 20 pm" src="https://user-images.githubusercontent.com/10074427/122058803-592f7800-ce2f-11eb-89de-7c97c7164b77.png">

* Docker container monitoring - must enable when installing agent

![Screen Shot 2021-06-15 at 11 14 14 pm](https://user-images.githubusercontent.com/10074427/122059154-af042000-ce2f-11eb-9155-ac1bf70e4ea1.png)


# Distributed Tracing
* Require java agent

```
export NEW_RELIC_APP_NAME="${APP_NAME}"
export NEW_RELIC_LICENSE_KEY="${NEW_RELIC_LICENSE_KEY}"

JAVA_OPTS="${JAVA_OPTS}-javaagent:${APP_HOME}/newrelic.jar"
```

* Services view

<img width="1421" alt="Screen Shot 2021-06-13 at 11 18 14 pm" src="https://user-images.githubusercontent.com/10074427/121808816-a4b21c80-cc9d-11eb-89f0-26b379775d38.png">

* otel-ui service view

<img width="1369" alt="Screen Shot 2021-06-13 at 11 20 09 pm" src="https://user-images.githubusercontent.com/10074427/121808888-e773f480-cc9d-11eb-8289-871a053aa49e.png">

* otel-ui traces listing

<img width="1257" alt="Screen Shot 2021-06-13 at 11 20 42 pm" src="https://user-images.githubusercontent.com/10074427/121808899-fb1f5b00-cc9d-11eb-9708-8e6d727cfc67.png">

* trace view

<img width="1296" alt="Screen Shot 2021-06-13 at 11 21 41 pm" src="https://user-images.githubusercontent.com/10074427/121808927-1e4a0a80-cc9e-11eb-937d-a7c60f1d7e85.png">

* buggy trace - incomplete

<img width="1255" alt="Screen Shot 2021-06-13 at 11 22 29 pm" src="https://user-images.githubusercontent.com/10074427/121808952-3ae64280-cc9e-11eb-9fdb-b43242cfdcab.png">

* error

<img width="1197" alt="Screen Shot 2021-06-13 at 11 32 15 pm" src="https://user-images.githubusercontent.com/10074427/121809286-98c75a00-cc9f-11eb-9ede-d4d10c469465.png">

![image](https://user-images.githubusercontent.com/10074427/122150113-7e100380-cea0-11eb-930d-6ec8d1368a09.png)


# Dashboards
* For every panel you can get a query
* Seems alot easier to use and can use SQL

![Screen Shot 2021-06-15 at 11 23 16 pm](https://user-images.githubusercontent.com/10074427/122060179-b24bdb80-ce30-11eb-85ad-4154e552390c.png)

* Every panel has option to view query

![image](https://user-images.githubusercontent.com/10074427/122149704-dc88b200-ce9f-11eb-841f-18d6b42aa551.png)

* Query view

![image](https://user-images.githubusercontent.com/10074427/122149737-eb6f6480-ce9f-11eb-8879-dc04773f6a9e.png)

* PromQL-style

https://valyala.medium.com/promql-tutorial-for-beginners-9ab455142085

![image](https://user-images.githubusercontent.com/10074427/122149801-0215bb80-cea0-11eb-9505-7dbc086fa36a.png)

# Logs

* Simple grep across all logs

![Screen Shot 2021-06-15 at 11 25 12 pm](https://user-images.githubusercontent.com/10074427/122060567-11115500-ce31-11eb-8afd-1b25ce7add7d.png)

# Alerts
* Seems quite comprehensive, even when installing infra agent it will ask to send alerts or not

* Define your query

![Screen Shot 2021-06-15 at 11 26 48 pm](https://user-images.githubusercontent.com/10074427/122060727-2f775080-ce31-11eb-9707-ffdc90da791c.png)

* Settings

![Screen Shot 2021-06-15 at 11 28 36 pm](https://user-images.githubusercontent.com/10074427/122060969-6cdbde00-ce31-11eb-8f54-49697a6593a5.png)

* Example email alert

![image](https://user-images.githubusercontent.com/10074427/122150238-ac8dde80-cea0-11eb-84f8-f8a364482007.png)
