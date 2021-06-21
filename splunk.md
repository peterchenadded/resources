# Overview

* Splunk Saas product for metrics, traces and logs
* 14 day free trial
* Servers are only in united states or europe
* Really just signalFx? which was acquired by splunk in aug 2019
* https://app.us1.signalfx.com/#/signin

# Infra monitoring
* Easy to setup just install agent
* Uses the otel collector agent which has lots of settings i believe
* More general ways of integration for each cloud provider

* One host dashboard

<img width="1421" alt="Screen Shot 2021-06-13 at 5 35 49 pm" src="https://user-images.githubusercontent.com/10074427/121799252-62251b80-cc6e-11eb-8ff0-69550c7a1cd1.png">

* Hosts dashboard
<img width="1075" alt="Screen Shot 2021-06-13 at 5 40 27 pm" src="https://user-images.githubusercontent.com/10074427/121799285-94cf1400-cc6e-11eb-84fe-fabf88e6ecba.png">

* Docker host dashboard need extra settings and permissionsto be added

<img width="1425" alt="Screen Shot 2021-06-13 at 5 37 31 pm" src="https://user-images.githubusercontent.com/10074427/121799245-59344a00-cc6e-11eb-8e73-7c667a7000f9.png">

* Docker container dashboard

<img width="1414" alt="Screen Shot 2021-06-13 at 5 38 05 pm" src="https://user-images.githubusercontent.com/10074427/121799235-50437880-cc6e-11eb-9cf2-f949ab4f01b0.png">

# Distributed Tracing
* Instrumentation

```
 # Splunk observability
  export OTEL_RESOURCE_ATTRIBUTES="service.name=${APP_NAME},deployment.environment=dev"
  export OTEL_EXPORTER_OTLP_ENDPOINT='http://splunk-otel-collector:4317'

  JAVA_OPTS="${JAVA_OPTS} \
    -javaagent:${APP_HOME}/splunk-otel-javaagent.jar -Dsplunk.metrics.enabled=true"
```

* Service map

<img width="1422" alt="Screen Shot 2021-06-13 at 1 28 08 am" src="https://user-images.githubusercontent.com/10074427/121781159-d320f080-cbe6-11eb-84d4-6b4f478cee70.png">

* Services overview

<img width="1413" alt="Screen Shot 2021-06-13 at 1 31 19 am" src="https://user-images.githubusercontent.com/10074427/121781217-15e2c880-cbe7-11eb-9223-e74ace8e1896.png">

* List of traces - can see ui getting very messy with lots of services

<img width="1428" alt="Screen Shot 2021-06-13 at 1 36 08 am" src="https://user-images.githubusercontent.com/10074427/121781386-cf419e00-cbe7-11eb-97a1-0a5af2b00d46.png">

* An example trace

<img width="1428" alt="Screen Shot 2021-06-13 at 1 36 08 am" src="https://user-images.githubusercontent.com/10074427/121781432-0021d300-cbe8-11eb-9646-c3cdd1d5a6ad.png">

* Trace drilldown details

<img width="1437" alt="Screen Shot 2021-06-13 at 1 39 05 am" src="https://user-images.githubusercontent.com/10074427/121781458-2e9fae00-cbe8-11eb-8c5f-3136e91f8a37.png">

# Dashboards
* Difficult to use, no SPL
* Granuality can be increased by changing collector settings
* Didn't see a way to display a table of metrics e.g. what are the processing running on host  with their cpu/memory usage

![image](https://user-images.githubusercontent.com/10074427/122061542-f55a7e80-ce31-11eb-9ca2-e41ffb1a6daf.png)

* As you onboard more data, dashboards are automatically added for you

![image](https://user-images.githubusercontent.com/10074427/122148614-22447b00-ce9e-11eb-8b9b-52513cd59390.png)

# Logs
* Not available in trial account
* If it is anything like splunk, it is good

![image](https://user-images.githubusercontent.com/10074427/122061265-af051f80-ce31-11eb-9eca-04ba9988a1c8.png)

# Alerting

![Screen Shot 2021-06-13 at 1 49 33 am](https://user-images.githubusercontent.com/10074427/121781793-bc2fcd80-cbe9-11eb-9ed4-fe9e26514c34.png)

* Alert condition

![image](https://user-images.githubusercontent.com/10074427/122148830-74859c00-ce9e-11eb-8e04-fd0291ba60ac.png)

* Alert settings

![image](https://user-images.githubusercontent.com/10074427/122148852-7e0f0400-ce9e-11eb-9f98-53f30a75b058.png)

