# Threat Actor Detection Lab

## Objective

The objective of this lab was to establish a controlled environment for simulating and detecting cyber attacks. Two virtual machines were set up, designated as host and target machines respectively. Subsequently, activities within this environment were monitored and logged to emulate real-world cyberattack scenarios. These logs were then ingested and analyzed utilizing a Security Information and Event Management (SIEM) tool, offering comprehensive telemetry for detection and analysis. Through this hands-on experience, I gained valuable insights into attack patterns, defensive strategies, and network security principles.

## Skills Learned

- Proficiency in utilizing Security Information and Event Management (SIEM) tools, including practical application within controlled environments.
- Competency in analyzing and interpreting network logs to identify anomalous behavior and potential cyber threats.
- Skill in generating and recognizing attack signatures and patterns, essential for proactive threat detection and response.
- Understanding of various network protocols and associated security vulnerabilities, enabling effective defense and mitigation strategies.
- Development of critical thinking and problem-solving abilities specific to cybersecurity, honed through hands-on experience with simulated cyberattack scenarios.

## Tools Used

- 𝗦𝗽𝗹𝘂𝗻𝗸 - Security Information and Event Management (SIEM) system for log ingestion and analysis.
- 𝗦𝘆𝘀𝗺𝗼𝗻 - Monitor and log system activity to the Windows event log.
- 𝗡𝗺𝗮𝗽 - Network scanning tool used for network exploration and host discovery.
- 𝗠𝗲𝘁𝗮𝘀𝗽𝗹𝗼𝗶𝘁 - Platform that allows to create exploits.
<br/>

 [//]: # (Math Sans Bold used for the bold heading) 

## Demonstration Video

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/RWE0wywoazo?modestbranding=1&showinfo=0&fs=0&rel=0;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe>
<br/>

## Steps 

- Opening 2 instances of virtual machines, one with Kali Linux and the other with Windows 10, and taking note of the IP address
  
<img src="https://i.imgur.com/HyJTOrt.png" width="50%" height="50%">

- Initiating Nmap and scanning the target machine ports
  
<img src="https://i.imgur.com/U1epTKg.png" width="50%" height="50%">

- Building a malware using msfvenom
  
<img src="https://i.imgur.com/EaZY7Fy.png" width="50%" height="50%">

- Using msfconsole to configure a handler that can listen to the assigned port 
  
<img src="https://i.imgur.com/hinFQUE.png" width="50%" height="50%">

- Setting up an HTTP server using Python to download the malware
  
<img src="https://i.imgur.com/3YDSTlt.png" width="50%" height="50%">

- Executing the malware and checking if the connection is established
  
<img src="https://i.imgur.com/Ii1wVO1.png" width="50%" height="50%">

- Establishing a shell and running some commands in the target machine
  Also checking to see if Splunk is configured to ingest Sysmon logs
  
<img src="https://i.imgur.com/GvnoJKo.png" width="50%" height="50%">

- Querying the malware events in Splunk from the newly created 'endpoint' index
  
<img src="https://i.imgur.com/3S6Z1m6.png" width="50%" height="50%">

- Using the process_guid to display the command prompt actions done by the attacker and create a table
  
<img src="https://i.imgur.com/iuFsEqI.png" width="50%" height="50%">









[Return To Homepage](https://edwinmathew0012.github.io/Portfolio/)

