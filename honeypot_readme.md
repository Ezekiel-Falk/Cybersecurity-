# Honeypot Assignment

**Time spent:** **10** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment 

**Summary:** 

To deploy the Honeypot I used Google Cloud Platform (GCP) a "cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products"(Wikipedia).
![Screen Shot 2022-11-08 at 2 15 50 PM](https://user-images.githubusercontent.com/88115439/201148981-498c635a-6fe4-420b-aa9d-8d8fdd9c5705.png)
![Screen Shot 2022-11-08 at 2 58 59 PM](https://user-images.githubusercontent.com/88115439/201149004-78c164a0-d908-4eb8-bba2-d00b4cf71359.png)

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
