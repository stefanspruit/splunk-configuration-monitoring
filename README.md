# splunk-configuration-monitoring
Contains monitoring dashboards to track changes for .conf and .xml files

Requires a new index 'splunk'

Install inputs-nix-configs on splunk components that are running on Linux. 
If Splunk is running on Windows you should install inputs-win-configs.

For each Splunk component where you install the inputs app it does a tail on splunk .conf and .xml files and forwards the config lines data to index=splunk.

conf-monitoring should be installed on the search heads. This app contains the dashboards to monitor which splunk configs/dashboards are changed.
