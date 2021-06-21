# Overview
* 15 day trial
* Data centers in US, EU, Sydney
* https://sso.dynatrace.com/

# Infrastructure Monitoring
* Agent installation on host

![Screen Shot 2021-06-16 at 12 02 03 am](https://user-images.githubusercontent.com/10074427/122066485-1de47780-ce36-11eb-92e6-94ea00381473.png)

* Host view

![image](https://user-images.githubusercontent.com/10074427/122066616-3f456380-ce36-11eb-83b4-2e4f0697a5ac.png)

![image](https://user-images.githubusercontent.com/10074427/122066782-613ee600-ce36-11eb-82e2-213398ac119e.png)

* Autodetection of technologies

<img width="1403" alt="Screen Shot 2021-06-16 at 12 10 56 am" src="https://user-images.githubusercontent.com/10074427/122067999-5f295700-ce37-11eb-8d93-bcefdd984aa0.png">

* Docker monitoring

![image](https://user-images.githubusercontent.com/10074427/122068192-8aac4180-ce37-11eb-978a-9fdf1f1c82e8.png)

![image](https://user-images.githubusercontent.com/10074427/122068256-97c93080-ce37-11eb-84a7-a74ec39b1cdd.png)

* Database monitoring

![image](https://user-images.githubusercontent.com/10074427/122068760-04dcc600-ce38-11eb-9221-f664d8a4ab10.png)

![image](https://user-images.githubusercontent.com/10074427/122068817-0e662e00-ce38-11eb-9649-fd5cc92e31d7.png)

* After sometime everything is auto detected

![image](https://user-images.githubusercontent.com/10074427/122068401-b8918600-ce37-11eb-9363-8063b28e7b16.png)

# Distributed Tracing
* Auto detects services

![image](https://user-images.githubusercontent.com/10074427/122069018-33f33780-ce38-11eb-9a2a-909f0dcc2909.png)

* Even detected dependency to the database correctly

![image](https://user-images.githubusercontent.com/10074427/122071430-11621e00-ce3a-11eb-967a-cc48a39ba4c3.png)

![image](https://user-images.githubusercontent.com/10074427/122071474-1a52ef80-ce3a-11eb-9a97-b3c42a051b5e.png)


* Rename the services on the ui

![image](https://user-images.githubusercontent.com/10074427/122069496-964c3800-ce38-11eb-89bb-ea4005efe18f.png)

<img width="1158" alt="Screen Shot 2021-06-16 at 12 20 22 am" src="https://user-images.githubusercontent.com/10074427/122070815-9d277a80-ce39-11eb-9886-01df672c111c.png">


* Uses purepaths for tracing
<img width="1394" alt="Screen Shot 2021-06-16 at 12 21 47 am" src="https://user-images.githubusercontent.com/10074427/122070868-a7497900-ce39-11eb-9ec8-ba4691e9a6f6.png">

<img width="1403" alt="Screen Shot 2021-06-16 at 12 22 36 am" src="https://user-images.githubusercontent.com/10074427/122070084-035fcd80-ce39-11eb-87a5-3631e1366323.png">

<img width="1378" alt="Screen Shot 2021-06-16 at 12 22 51 am" src="https://user-images.githubusercontent.com/10074427/122070095-0490fa80-ce39-11eb-87d5-d60e525bdbdb.png">

* Failures - one provider killed

![image](https://user-images.githubusercontent.com/10074427/122071834-6aca4d00-ce3a-11eb-8af5-43aadd943029.png)

<img width="693" alt="Screen Shot 2021-06-16 at 12 33 23 am" src="https://user-images.githubusercontent.com/10074427/122071966-87ff1b80-ce3a-11eb-9f16-0ed8559e158c.png">

<img width="1375" alt="Screen Shot 2021-06-16 at 12 34 19 am" src="https://user-images.githubusercontent.com/10074427/122072103-a1a06300-ce3a-11eb-9958-e292f980e057.png">

![image](https://user-images.githubusercontent.com/10074427/122072247-be3c9b00-ce3a-11eb-8e80-28eba2498c56.png)

![image](https://user-images.githubusercontent.com/10074427/122072288-c85e9980-ce3a-11eb-88cd-63985fb28496.png)

# Dashboards
* Very quick to create a dashboard
* Not able to use SQL/XML

![image](https://user-images.githubusercontent.com/10074427/122073060-779b7080-ce3b-11eb-836d-1b98b2aa421d.png)

* Charts

![image](https://user-images.githubusercontent.com/10074427/122073429-c1845680-ce3b-11eb-9a58-35cd140e02de.png)

![image](https://user-images.githubusercontent.com/10074427/122073517-d19c3600-ce3b-11eb-804c-7a6f98bf47d2.png)

* Lots of panels but no custom panels e.g. tables

![image](https://user-images.githubusercontent.com/10074427/122073670-f2fd2200-ce3b-11eb-9604-2ee597aabfe7.png)

# Logs
* Lists of logs for host
* Needs to be enabled in settings
* Restart takes quite long sudo systemctl restart oneagent
* Need to update /var/lib/dynatrace/oneagent/agent/config/ruxitagentloganalytics.conf to actually view logs in ui

![image](https://user-images.githubusercontent.com/10074427/122074151-51c29b80-ce3c-11eb-832c-56c1138bfaf2.png)

![image](https://user-images.githubusercontent.com/10074427/122077554-3016e380-ce3f-11eb-848b-bee93e409b89.png)

* Maybe a config issue on my side - should only have one peter testing error but got two

![image](https://user-images.githubusercontent.com/10074427/122078028-9bf94c00-ce3f-11eb-8214-14cf06a82143.png)

![image](https://user-images.githubusercontent.com/10074427/122078057-a3205a00-ce3f-11eb-9f64-91c8402a2ee7.png)

# Alerts
* Alert seems to be very simple and fully abstracted
* No custom searches for alerts

![image](https://user-images.githubusercontent.com/10074427/122079257-93eddc00-ce40-11eb-8237-d8fadf180f43.png)

![image](https://user-images.githubusercontent.com/10074427/122079193-83d5fc80-ce40-11eb-8ca6-57f72b74c30e.png)

* Anomaly detection for infrastructure

![image](https://user-images.githubusercontent.com/10074427/122079527-d8797780-ce40-11eb-8c48-3d1ee6107b86.png)

![image](https://user-images.githubusercontent.com/10074427/122079579-e4653980-ce40-11eb-9594-051f9dd9386d.png)

* Anomaly detection for services

![image](https://user-images.githubusercontent.com/10074427/122079647-f3e48280-ce40-11eb-8273-c6dacc8c7790.png)

![image](https://user-images.githubusercontent.com/10074427/122079776-124a7e00-ce41-11eb-855c-331967e4ec39.png)
