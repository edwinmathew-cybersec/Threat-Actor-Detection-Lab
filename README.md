# Threat Actor Detection Lab

## Objective

The objective of this lab was to create a controlled environment where I could simulate and detect cyber attacks. For this, two virtual machines were created and used as host and target machines. The logs generated were ingested and analyzed using an SIEM (Security Information and Event Management) tool, providing telemetry that simulated real-world cyberattack scenarios. This hands-on lab gave me a deep understanding of attack patterns, defensive methods, and network security.

## Skills Learned

- Understanding of SIEM and its practical application.
- Analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

## Tools Used

- 𝗦𝗽𝗹𝘂𝗻𝗸 - Security Information and Event Management (SIEM) system for log ingestion and analysis.
- 𝗦𝘆𝘀𝗺𝗼𝗻 - Monitor and log system activity to the Windows event log.
- 𝗡𝗺𝗮𝗽 - Network scanning tool used for network exploration and host discovery.
- 𝗠𝗲𝘁𝗮𝘀𝗽𝗹𝗼𝗶𝘁 - Platform that allows to create exploits.
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

- Setting up a HTTP server using Python to download the malware
  
<img src="https://i.imgur.com/3YDSTlt.png" width="50%" height="50%">

- Executing the malware and checking if the connection is established
  
<img src="https://i.imgur.com/Ii1wVO1.png" width="50%" height="50%">

- Establishing a shell and running some commands in the target machine
  Also checking to see if Splunk is configured to ingest Sysmon logs
  
<img src="https://i.imgur.com/GvnoJKo.png" width="50%" height="50%">

- Querying the malware events in Splunk from the newly created 'endpoint' index
  
<img src="https://i.imgur.com/3S6Z1m6.png" width="50%" height="50%">

- Using the process_guid to display the command promt actions done by the attacker and create a table
  
<img src="https://i.imgur.com/iuFsEqI.png" width="50%" height="50%">


