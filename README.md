# API-Availabillity-Monitoring-With-Prometheus-Blackbox-Exporter
This project was created as a solution-based approch for monitoring API Availabillity. Metrics to be shown in the visualization includes up/down status, SLA percentage, and hit latency. Project was created using Prometheus + Blackbox Exporter with Grafana running on Docker. Grafana API was used as the targeted API. Hermes and Notification Channel are disabled in this trial, because it's an optional function.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Installing and Running the stack

Guide to set-up repo stacks.

1. Install Docker & Docker-Compose if it hasn't been installed on your machine and run it.\
[Docker Install](https://docs.docker.com/get-docker/) & [Docker-Compose Install](https://docs.docker.com/compose/install/)

2. Clone this repository into your machine.
```
$ git clone https://github.com/revawiki/API-Availabillity-Monitoring-With-Prometheus-Blackbox-Exporter
```

3. Go to the cloned directory, and execute the bashfile.
```
$ ./up.sh
```

### Set-up Datasource and Dashboard
1. Access the grafana via (http://localhost:3000), with default password admin:admin.

2. Set Prometheus as datasource using address (http://prometheus:9090), save and test datasource.

3. Import new dashboard using .JSON schema from (../conf/template.json).

#### Expected visual
![Grafana-Dashboard](https://raw.githubusercontent.com/revawiki/ACS-Stack-For-CPE-Statistics-Monitoring/master/img/cpe-visualization.png)

## Built With

* [TIG-Stack for Monitoring RouterOS](https://github.com/revawiki/TIG-Stack-for-Monitoring-RouterOS-using-HTTP-Listener) for this case-based TIG-Stack.
* [RouterOS with TR069](https://mikrotik.com/) for CPE Device.
* [GenieACS](https://genieacs.com/) for TR069 remote management.
* [Docker](https://www.docker.com/) for Container Virtualization.

## Credits

* [ACS-Stack](https://github.com/haidlir/ACS-Stack) by Haidlir Naqvi.
* [RouterOS TR069 Data Model](https://wiki.mikrotik.com/tr069ref/current.html) by Mikrotik.
* [GenieACS for Docker](https://github.com/DrumSergio/genieacs-docker) by DrumSergio

##### Question/Inquiries
If you have any question regarding the repo, feel free to e-mail me at reva.wiki@gmail.com. Thank you.

