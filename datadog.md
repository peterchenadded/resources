# Overview

* Hosted in US, EU
* * 14 day trial

# Infrastructure Monitoring

* Simple installation through curl and managed through systemctl

```
sudo systemctl start datadog-agent
```

![image](https://user-images.githubusercontent.com/10074427/122413876-10f88d00-cfca-11eb-97a2-a0acc09e4a95.png)

![image](https://user-images.githubusercontent.com/10074427/122413963-1f46a900-cfca-11eb-842e-ac849d8500fc.png)

![image](https://user-images.githubusercontent.com/10074427/122414090-39808700-cfca-11eb-89e5-ee00dc395e53.png)

* Limited time range

![image](https://user-images.githubusercontent.com/10074427/122414773-bd3a7380-cfca-11eb-952f-f5c61bce52f2.png)

* Process monitoring can be enabled

![image](https://user-images.githubusercontent.com/10074427/122414935-d8a57e80-cfca-11eb-8804-339521600731.png)

* Network monitoring can be enabled - though it did not work for some reason

* Docker containers

![image](https://user-images.githubusercontent.com/10074427/122426655-c1b75a00-cfd3-11eb-9be3-10e126e85ddd.png)


# Distributed Tracing

![image](https://user-images.githubusercontent.com/10074427/122421590-d1cd3a80-cfcf-11eb-9571-a8141f266f96.png)

* Services actually 6 services not 5 (1 ui, 1 api, 2 providers, 2 dbs)

![image](https://user-images.githubusercontent.com/10074427/122422403-7780a980-cfd0-11eb-8147-b4c574f98122.png)

* Services map view

![image](https://user-images.githubusercontent.com/10074427/122422521-8f582d80-cfd0-11eb-8ff5-79cb4552a5f0.png)

* Trace listing

![image](https://user-images.githubusercontent.com/10074427/122421786-fc1ef800-cfcf-11eb-9a76-cfd7ae1fe29f.png)

* Trace view

![image](https://user-images.githubusercontent.com/10074427/122422046-2b356980-cfd0-11eb-8170-e436900d32f8.png)

* Span list

![image](https://user-images.githubusercontent.com/10074427/122422246-57e98100-cfd0-11eb-9070-ea6a71f76bca.png)

* Errors

<img width="1486" alt="Screen Shot 2021-06-18 at 1 07 33 am" src="https://user-images.githubusercontent.com/10074427/122423853-97649d00-cfd1-11eb-810d-4cfd1892c088.png">

![image](https://user-images.githubusercontent.com/10074427/122423981-b2371180-cfd1-11eb-9d49-9470aa72fd68.png)


# Dashboarding

* Example dashboard

![image](https://user-images.githubusercontent.com/10074427/122424837-5faa2500-cfd2-11eb-988e-143d5cffce62.png)

* types of panels that can be added

![image](https://user-images.githubusercontent.com/10074427/122425068-92541d80-cfd2-11eb-87b1-8dd8fd370b85.png)

* Uses a json query

<img width="1592" alt="Screen Shot 2021-06-18 at 1 15 25 am" src="https://user-images.githubusercontent.com/10074427/122425238-b0218280-cfd2-11eb-87f5-8d6294306884.png">

* Time picker

![image](https://user-images.githubusercontent.com/10074427/122425476-dba46d00-cfd2-11eb-8afa-672cf2ed7377.png)

# Logs

![image](https://user-images.githubusercontent.com/10074427/122427230-4904cd80-cfd4-11eb-955d-2f4889e5606e.png)

* Search by keyword

![image](https://user-images.githubusercontent.com/10074427/122427336-6043bb00-cfd4-11eb-987f-2ff9470fa4f5.png)


# Alerting
