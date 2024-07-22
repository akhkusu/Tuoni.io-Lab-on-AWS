<h1>Kali Linux C2 with Tuoni on AWS</h1>
<h2>Description</h2>
In this lab, I set up a command and control (C2) environment using Kali Linux and Windows Server 2022 on AWS. I installed <b><a href="https://www.tuoni.io" target="_blank">Tuoni.io</a></b> on the Kali Linux instance to remotely control the Windows Server. This setup demonstrates the basics of C2 operations, allowing for remote execution of commands on the Windows server using the Tuoni platform.
<br />
<h2>Utilities and Environment Used</h2>

    Kali Linux
    Windows Server 2022
    Tuoni.io
    AWS Cloud
    AWS EC2


<h2>Program Walk-Through:</h2>
<p >
<strong>1. Setting up the Environment:</strong><br/>
Initially, I created two virtual machines on AWS: one running Kali Linux and the other running Windows Server 2022. The AWS EC2 instances were configured with appropriate security groups to allow for necessary network traffic between the machines.
<br />
<img src="img/aws_setup.png" height="80%" width="80%" alt="AWS EC2 Setup"/>
<br />
<br />
<br />

<strong>2. Installing Tuoni.io on Kali Linux:</strong><br/>
I installed the Tuoni.io command and control server on the Kali Linux instance. Tuoni is a powerful open-source tool that allows for easy management and interaction with compromised systems.
<br />
<img src="img/tuoni_installation.png" height="80%" width="80%" alt="Tuoni Installation"/>
<br />
<br />
<br />

<strong>3. Deploying and Executing the C2 Agent on Windows Server:</strong><br/>
Once Tuoni was set up, I deployed the Tuoni C2 agent on the Windows Server 2022 instance. The agent allowed me to establish a remote connection back to the Tuoni server on Kali Linux. Through this connection, I was able to execute commands on the Windows Server using the Tuoni terminal.
<br />
<img src="img/agent_execution.png" height="80%" width="80%" alt="Agent Execution"/>
<br />
<br />
<br />

<strong>4. Remote Command Execution:</strong><br/>
With the agent running, I demonstrated remote control capabilities by executing various commands on the Windows Server through the Tuoni C2 server. This included basic tasks such as file manipulation and system information gathering.
<br />
<img src="img/remote_execution.png" height="80%" width="80%" alt="Remote Command Execution"/>
<br />
<br />
<br />

<strong>5. Monitoring and Analysis:</strong><br/>
Throughout the process, I monitored the network traffic and system logs to analyze the behavior of the C2 operations. This included observing the command execution flow from the Tuoni server to the Windows agent.
<br />
<img src="img/monitoring_analysis.png" height="80%" width="80%" alt="Monitoring and Analysis"/>
<br />
</p>
<h2>Conclusion:</h2>
This lab provided valuable insights into the workings of a command and control (C2) environment using Tuoni.io. It demonstrated the ability to set up and manage a C2 server, deploy agents, and perform remote operations. Such setups are crucial for understanding the mechanisms behind cyber operations and enhancing security posture against potential threats.
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

---
