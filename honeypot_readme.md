# Honeypot Assignment

**Time spent:** **10** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment 

**Summary:** 

To deploy the Honeypot I used Google Cloud Platform (GCP) a "cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products"(Wikipedia).

<img src="mhn-admin.gif">

### Dionaea Honeypot Deployment 

**Summary:** 

A dionaea creates an environment that acts as a trap to capture malware information. After capturing the information, dionaea creates a log, you can also see where the attack are coming from. 

<img src="dionaea-honeypot.gif">

### Database Backup (Required) 

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?

MHN-Admin uses MySQL. In the exported JSON file record I found information on timestamp, date, source_ip, source_port, destination_port, identifier, and lastly protocol. 

*Upload session.json directly to this GitHub repo/branch.*


## Notes

Describe any challenges encountered while doing the assignment.

The only challenges I encountered way having to set up the Google cloud platform and deploy both on Bluetooth and a honey pot. At the end I was able to figure it out. 