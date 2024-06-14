<h1>SOC-Automation-Project</h1>

<h2>Description</h2>
In this cybersecurity project, I created a comprehensive diagram of data traversing through a network. More specifically, I visualized how data traverses through different tools such as TheHive and Wazuh Managers to enhance incident response, accelerate threat detection, and streamline SOC workflows.
<br />
<h2>Project walk-through:</h2>
<img width="650" alt="Screenshot 2024-06-13 at 7 23 23 PM" src="https://github.com/bpark1223/SOC-Automation-Project/assets/77799235/ef5549f0-3dee-412f-8544-07bb13fa4f68">
<br />
<h2>Step-by-Step Walkthrough</h2>
1. Data originates at the Windows 10 Client, which has the Wazuh Agent installed. 
<br />
2. The Wazuh agent collects logs and security events and sends them through the router and Internet to the Wazuh Manager.
<br />
3. The Wazuh manager then collects and analyzes data from the deployed Wazuh agents. It triggers alerts to Shuffle when threats or anomalies are detected 
<br />
4. Shuffle then performs open-source intelligence (OSINT) gathering to enrich the indicators of compromise (IOC). It will then send an alert to TheHive, as well as an email to the SOC analyst 
<br />
5. The SOC analyst then receives this email which contains details about the alert, and asks if the analyst would like to perform a certain action. 
<br />
6. Depending on the response, the action will then be sent over to Shuffle, then to Wazuh, and finally back to the Client which will perform the action.
