# SOC Automation

<br>

## Description
- Set up **Wazuh** (XDR and SIEM Platform) to ingest Sysmon logs and detect malicious activity.
- Malicious activity triggered a rule to push alerts from **Wazuh** to **Shuffle** via an API.

Utilized **Shuffle** (Automation Workflow Platform) to:
- Enrich IoCs and perform VirusTotal hash-check on malware via APIs.
- Generate an alert on **TheHive** (Incident Response Platform).
- Email an alert to the SOC analyst for incident response.

## Technology Used
- **Wazuh** (XDR and SIEM Platform)  
- **Shuffle** (Automation Workflow Platform)  
- **TheHive** (Incident Response Platform)  
- **ElasticSearch** (Search & Analytics Engine)  
- **Cassandra** (NoSQL database)  
- **VirusTotal** (Malware Database)  
- **API Integration**  

## Diagram
![SOC Automation Workflow](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/SOC%20Automation%20Workflow%20Diagram.jpg)

## **Demo**  

### **1. Shuffle Automation Workflow**  
This image showcases the **Shuffle automation process**, illustrating how alerts and security events flow through different components.  
![Shuffle Automation Workflow](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/Shuffle%20Automation%20Workflow.jpg)  

<br>

### **2. Mimikatz Malicious Activity Detected**  
This screenshot highlights a **malicious activity detection** involving **Mimikatz**, a well-known credential dumping tool. The detection is based on Sysmon logs analyzed by Wazuh.  
![Mimikatz Malicious Activity](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/Mimikatz%20Malicious%20Activity%20Running.jpg)  

<br>

### **3. Wazuh Detection Rules**  
Here, we see **custom Wazuh rules** in action, which are responsible for identifying suspicious activity and triggering alerts.  
![Wazuh Rules](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/Wazuh%20Rules.jpg)  

<br>

### **4. Automated Email Alert**  
Once a threat is detected, an **automated email alert** is sent to SOC analysts, ensuring they are informed in real time.  
![Automated Email Alert](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/Automated%20Email%20Alert.jpg)  

<br>

### **5. TheHive Alert Generation**  
The detected threat is **automatically pushed into TheHive**, an incident response platform, allowing analysts to investigate further.  
![TheHive Alert](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/TheHive%20Alert.jpg)  

<br>

### **6. Expanded TheHive Alert Details**  
Finally, this image shows a **detailed view of the alert within TheHive**, including enriched IoC data and contextual information for deeper analysis.  
![TheHive Alert Expanded](https://raw.githubusercontent.com/JunedConnect/SOC_Automation/main/images/TheHive%20Alert%20Expanded.jpg)  
