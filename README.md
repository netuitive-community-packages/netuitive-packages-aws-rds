# netuitive.packages.aws.rds

For detailed information on this package, please refer to the [online documentation](https://help.netuitive.com/Content/Integrations/aws.htm).

## Release History

### Version 1.6.0

* Updated element details dashboard layout

### Version 1.5.2

* Removed overall utilization computed metric and associated widgets
* Replaced overall utilization dashboard and element detail widgets with individual component utilizations

### Version 1.5.1

* Fixed the IOPS utilization calculation to take into account storage size

### Version 1.5.0

* Updated dashboard layouts for gridstack.

### Version 1.4.3

* Updated the CPU Utilization policy to not alarm when CPU is under 20%.

### Version 1.4.2

* Updated package compatibilities.

### Version 1.4.1

* Bug fix for the multi-metric widgets on the element detail page.

### Version 1.4.0

* Renamed the "Connection Utilization Percent" metric to "Connection Throughput Utilization" to make it clearer that this metric is measuring how utilized the capacity of the connections is, not what percentage of the total available connections are in use.
* Removed correlation flag from the "Overall Utilization" metric, since this metric is a linear combination of the other utilization metrics.
* Baseline and correlate "Read IOPS" and "Write IOPS" rather than "Total IOPS". This allows us to more reliably catch an incident where, for example, read is excessively high and write is excessively low, or vice versa.
* Added three new policies:
 * AWS RDS - Elevated Connections
 * AWS RDS - Elevated Read IOPS
 * AWS RDS - Elevated Write IOPS
* Fixed a bug where some widgets were not displaying correctly on the element detail page.

### Version 1.3.2

* Fixed bug with the Events widget on the Element Detail Page.

### Version 1.3.1

* Minor cleanup to the RDS Summary dashboard.

### Version 1.3.0

* Added RDS-specific element detail page.
* Changed "sum" to "avg" on summary dashboard widgets.

### Version 1.2.0

* Defined units for the metrics.

### Version 1.1.1

* Removed reference to obsolete metric.

### Version 1.1.0

* Added summary dashboard.

### Version 1.0.0

* Initial production release of the package for monitoring AWS Relational Database Service (RDS) resources.
