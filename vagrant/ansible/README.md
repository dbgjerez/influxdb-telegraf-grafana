# Ansible configuration

This example install Apache, Tomcat, Influxdb and Grafana.

Functionally, Telegraf pulls stats from Apache and Tomcat. This information is saved in InfluxDB. Grafana has been configured with InfluxDB as datasource.

The information is showing in different dashboards.

# Apache
Apache's role install apache with mod_status enabled. This is installed as a system service.

# Grafana
Grafana is installed as a system service.

When Grafana has been installed, another role configure it, dashboards and datasources are configured. 

# Telegraf
Telegraf is installed as a system service. 

# InfluxDB 
InfluxDB is installed as a system service. The information can be sended at 8086 port.
