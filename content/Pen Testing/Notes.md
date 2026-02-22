* Port 3389 is the default port for Remote Desktop Services and is an excellent indication that the target is a Windows machine.
* `nmap` can run scripts during its scan that identify specific vulnerabilities (such as the script found [here](https://raw.githubusercontent.com/cyberstruggle/DeltaGroup/master/CVE-2019-19781/CVE-2019-19781.nse)) with `nmap --script <script name> -p<port> <host>`

![[Pen Testing/Images/shell-types.png]]

![[Pen Testing/Images/nmap-script-categories.png]]