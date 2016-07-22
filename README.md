#netuitive.packages.aws.rds 1.4.1

For detailed information on this package, please refer to the [online documentation](https://help.app.netuitive.com/Content/Misc/Datasources/AWS/new_aws_datasource.htm).

##Release History

###Version 1.4.1

* Bug fix for the multi-metric widgets on the element detail page.

###Version 1.4.0

* Renamed the "Connection Utilization Percent" metric to "Connection Throughput Utilization" to make it clearer that this metric is measuring how utilized the capacity of the connections is, not what percentage of the total available connections are in use.
* Removed correlation flag from the "Overall Utilization" metric, since this metric is a linear combination of the other utilization metrics.
* Baseline and correlate "Read IOPS" and "Write IOPS" rather than "Total IOPS". This allows us to more reliably catch an incident where, for example, read is excessively high and write is excessively low, or vice versa.
* Added three new policies:
 * AWS RDS - Elevated Connections
 * AWS RDS - Elevated Read IOPS
 * AWS RDS - Elevated Write IOPS
* Fixed a bug where some widgets were not displaying correctly on the element detail page.

###Version 1.3.2

* Fixed bug with the Events widget on the Element Detail Page.

###Version 1.3.1

* Minor cleanup to the RDS Summary dashboard.

###Version 1.3.0

* Added RDS-specific element detail page.
* Changed "sum" to "avg" on summary dashboard widgets.

###Version 1.2.0

* Defined units for the metrics.

###Version 1.1.1

* Removed reference to obsolete metric.

###Version 1.1.0

* Added summary dashboard.

###Version 1.0.0

* Initial production release of the package for monitoring AWS Relational Database Service (RDS) resources.
