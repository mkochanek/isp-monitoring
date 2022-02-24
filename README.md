# isp-monitoring

This is a setup for monitoring your ISP by using InfluxDB, Telegraf, speedtest.net CLI and Grafana

## Installation

Installation of Grafana, Telegraf and InfluxDB is out of scope. Please follow vendor's manuals in order to install the mentioned software. 

Provide Telegraf with configuration file from this repo. The Telegraf's configuration file default location is /etc/telegraf/telegraf.conf

Upload bash script speedtest.sh from this repo to /usr/bin/. Set the server ID (-s <serverID>) that you wish to monitor against. This is taken from '''/usr/bin/speedtest -L''' command. 

Upload [speedtest.net CLI](https://www.speedtest.net/apps/cli) (speedtest) to /usr/bin

Set sufficient permissions for these files so that Telegraf user can use them. 

## Usage

Use the collected metrics in Grafana dashboard so you can observe your Internet connection statistics.
