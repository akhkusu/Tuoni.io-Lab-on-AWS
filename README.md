<h1>Kali Linux C2 with Tuoni on AWS</h1>

<h2>Description</h2>
<p>In this lab, I set up a command and control (C2) environment using Kali Linux and Windows Server 2022 on AWS. I installed <b><a href="https://www.tuoni.io" target="_blank">Tuoni.io</a></b> on the Kali Linux instance to remotely control the Windows Server. This setup demonstrates the basics of C2 operations, allowing for remote execution of commands on the Windows server using the Tuoni platform.</p>

<h2>Environments Used</h2>
<ul>
    <li><b>Cloud Platform</b>: AWS</li>
    <li><b>Virtual Machines</b>:
        <ul>
            <li>Kali Linux</li>
            <li>Windows Server 2022</li>
        </ul>
    </li>
</ul>

<h2>Lab Walk-through</h2>

<h3>Setting Up the Environment</h3>
<ol>
    <li><b>Creating AWS EC2 Instances</b>: I set up two EC2 instances on AWS, one with Kali Linux and the other with Windows Server 2022.</li>
</ol>

<p align="center">
    <img src="img/Screenshot 2024-07-18 163857.png" height="80%" width="80%" alt="AWS EC2 Setup"/>
</p>
<p align="center">
    <img src="img/Screenshot 2024-07-18 181341.png" height="80%" width="80%" alt="AWS EC2 Setup"/>
</p>


<h3>Installing Tuoni.io on Kali Linux</h3>
<ol>
    <li><b>Download and Install Tuoni.io</b>: On the Kali Linux instance, I downloaded and installed the <a href="https://www.tuoni.io" target="_blank">Tuoni.io</a></li>
</ol>


<h3>Deploying the C2 Agent on Windows Server</h3>
<ol>
    <li><b>Generating and Running the Agent</b>: Generated the Tuoni C2 agent on the Kali Linux server and executed it on the Windows Server 2022 instance.</li>
</ol>

<p align="center">
    <img src="img/Screenshot 2024-07-18 235545.png" height="80%" width="80%" alt="Agent Execution"/>
</p>

<h3>Remote Command Execution</h3>
<p>With the C2 agent running on the Windows Server, I used the Tuoni.io command and control server to execute remote commands. This included file system exploration and system information retrieval.</p>


<p align="center">
    <img src="img/Screenshot 2024-07-18 231038.png" height="80%" width="80%" alt="Remote Command Execution"/>
</p>
<p align="center">
    <img src="img/Screenshot 2024-07-18 185700.png" height="80%" width="80%" alt="Remote Command Execution"/>
</p>


<ol>
    <li><b>Downloading an Image from Windows to Kali Linux</b>: As part of the C2 operations, I demonstrated how to download a file from the Windows Server to the Kali Linux machine using Tuoni.io. Specifically, I downloaded an image of a cat from the Windows machine.</li>
</ol>


<p align="center">
    <img src="img/Screenshot 2024-07-18 234804.png" height="80%" width="80%" alt="Cat Image on Windows"/>
</p>

<p align="center">
    <img src="img/Screenshot 2024-07-18 234942.png" height="80%" width="80%" alt="Cat Image on Kali Linux"/>
</p>



<h2>Conclusion</h2>
<p>This lab provided valuable insights into the workings of a command and control (C2) environment using <a href="https://www.tuoni.io" target="_blank">Tuoni.io</a>. 
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
