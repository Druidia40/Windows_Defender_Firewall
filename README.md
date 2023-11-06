<h1>Microsoft Windows Defender Firewall</h1>

<h2>Description</h2>
Windows Defender Firewall is a host-based software firewall that is included with the Windows operating system. In this lab, I'll show you how to configure firewall rules using Windows Defender Firewall and Windows Defender Firewall with Advanced Security.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Windows Lab Workspace</b> 

<h2>Environments Used </h2>

- <b>Windows 11 Pro</b>

<h2>Program walk-through:</h2>

<p align="center">
Click the Windows Start button and select Windows Security: <br/>
<img src="https://i.imgur.com/FrfS3pE.png" height="60%" width="60%" alt="Select Windows Security from Start Menu"/>
<br />
<br />
Click Firewall & network protection:  <br/>
<img src="https://i.imgur.com/5iuZ4ez.png" height="60%" width="60%" alt="Firewall & Network Protection"/>
<br />
<br />
Review network status: <br/>
<img src="https://i.imgur.com/TERSLag.png" height="60%" width="60%" alt="Network Status"/>
<br />
<br />
Click Domain Network:  <br/>
<img src="https://i.imgur.com/8gV1sW0.png" height="60%" width="60%" alt="Domain Network"/>
<br />
<br />
Verify the Windows Defender Firewall is toggled to "ON":  <br/>
<img src="https://i.imgur.com/Cc8RinK.png" height="60%" width="60%" alt="Toggle ON"/>
<br />
<br />
Ensure that the firewall for both the Private and Public Network is ON, then click on "Allow an app through firewall":  <br/>
<img src="https://i.imgur.com/Xgmgoo8.png" height="60%" width="60%" alt="Allow app through firewall"/>
<br />
<br />
Scroll to Mozilla Firefox. The current configuration allows for Firefox to communicate on the Private network but denies it from communicating on the Public network:  <br/>
<img src="https://i.imgur.com/sOWSKOE.png" height="60%" width="60%" alt="Apps & Features Screen"/>
<br />
<br />
Click the Public box next to Firefox. A checkmark will appear. Click OK to return to the Firewall & network protection screen:  <br/>
<img src="https://i.imgur.com/pXIUPLj.png" height="60%" width="60%" alt="Checkmark Screen"/>
<br />
<br />
On the Firewall & network protection screen, select Advanced settings to edit an existing rule:  <br/>
<img src="https://i.imgur.com/Rs2kbBK.png" height="60%" width="60%" alt="Advanced Settings"/>
<br />
<br />
Here you can review Inbound and Outbound Rules, click on Inbound Rules:  <br/>
<img src="https://i.imgur.com/j2Q8TI4.png" height="60%" width="60%" alt="Inbound/Outbound Rules"/>
<br />
<br />
Scroll to Key Management Service, double click the rule:  <br/>
<img src="https://i.imgur.com/ErbUmcd.png" height="60%" width="60%" alt="Key Management Service"/>
<br />
<br />
Review the Properties then click the Advanced tab:  <br/>
<img src="https://i.imgur.com/OAvChuZ.png" height="60%" width="60%" alt="Advanced tab"/>
<br />
<br />
Here you can see which profiles the rule applies to, Domain, Private and Public are listed:  <br/>
<img src="https://i.imgur.com/yif50MH.png" height="60%" width="60%" alt="Profiles"/>
<br />
<br />
To allow communication only with the domain and private networks, uncheck the Public box, click OK then Apply:  <br/>
<img src="https://i.imgur.com/db0E7zq.png" height="60%" width="60%" alt="Uncheck Public Box"/>
<br />
<br />
Copy and Paste the rule. Ensure that Domain, Private is enabled and allowed and that Public is Disabled and Block:  <br/>
<img src="https://i.imgur.com/wbYEiML.png" height="60%" width="60%" alt="Copy and Paste the rule"/>
<br />
<br />
The Overview panel will show your changes. Right-click each Key Management Service (TCP-In) rule and click Enable rule, verify with green checkmark:  <br/>
<img src="https://i.imgur.com/p4j67Nn.png" height="60%" width="60%" alt="Overview Panel"/>
<br />
<br />

</p>
