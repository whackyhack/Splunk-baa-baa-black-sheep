# Splunk-baa-baa-black-sheep
In this demo dashboard, linguistic and semantic constructs in Baa, baa, black sheep are used to illustrate how "hidden" fields can be used to enhance visualization, especially (but not limited to) text visualization.  It also demonstrates some advanced text visualization techniques.

This dashboard is for Dashboard Studio, and requires Splunk 9.4.0 and higher to display multiple tabs.

# Rack view
This demo dashboard demonstrates a practical application of the "tower" view exemplified in Baa, baa, black sheep.

When the dashboard loads, only server names are displayed.  You can add model, temperature, etc., into the view.  You can also select racks or other attributes of interest, all on a 42-unit vertical ladder.

This dashboard is tested in Splunk 9.4.0 Dashboard Studio but should be compatible with any versions of Dashboard Studio (starting Splunk 8.0).

# Vulnerability report
This demo dashboard demonstrates a practical application of the breakdown view exemplified in Baa, baa, black sheep.  Requires vulnerabilities.csv as lookup.

The column order is time line from right to left; i.e., left-most entries are the most recent.  Base breakdown is severity rating (based on CVSS score), vulnerability group (with the most severe vulnerability in the group displayed as group lead), and the exposure duration of the oldest vulnerability in the breakdown.  Servers are organized by silos.  At this time, the only additional breakdown is silo.

Data cells display exposures in the breakdown, number of servers exposed to that breakdown.  By default, if there are more than one vulnerabilities in that breakdown, additional vulnerability counts (VIDs) are also displayed in the cell.  You can change that to display list of additional vulnerabilities.

Using the top of dashboard selectors, you can also select a single vulnerability breakdown, or a single silo for analysis.  Additionally, you can view more details about vulnerabilities in a particular breakdown, for example, which servers are exposed, suggested solution, compliance status, etc., by clicking on it.  Minimal functionality is implemented in the detailed view for now.

This dashboard is tested in Splunk 9.4.0 Dashboard Studio but should be compatible with any versions of Dashboard Studio (starting Splunk 8.0).
