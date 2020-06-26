# How to SIEM Your SAP Security Audit Log with Splunk?

The following repository contains a lookup CSV file to be used in the Splunk Indexer to match SAP NetWeaver Security Audit Log message IDs with event metadata. This will allow you to generally see SAP audit logs in a similar way as you will typically see those in SAP transaction SM20.

[sm20.csv - Download](https://raw.githubusercontent.com/WALLSEC/SAPtoSPLUNK/master/sm20.csv)

Below you will find the link to a tutorial on how to forward SAP NetWeaver Security Audit Logs to Splunk directly, parse those and create SIEM Splink alerts without the need for a third party adapter or intermediate SAP SIEM solution, saving money on costs and maintenance.

https://www.wallsec.de/blog/siem-your-sap-security-audit-log-with-splunk


## SIEM your SAP NetWeaver Audit Log

The SAP Security Audit Log is not in a common log format which needs to be transformed in order to make it usable for our SIEM purposes.

GET FROM THIS:

![SAP NetWeaver 100MB one liner file containging the SAP Security Audit Log](/images/SAP_Security_Audit_Log_raw.png)

TO THIS:


![Parsed and enriched SAP Audit Log in Splunk](/images/Splunk_SAP_audit_log_parse.png)


The final result is a searchable SAP audit log on top of which we can build our security monitoring use cases and improve SIEM coverage over the enterprise SAP landscape.
