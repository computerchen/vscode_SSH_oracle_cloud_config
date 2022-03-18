Supposed your VPS on Oracle Cloud , and its IP Address is xx.xx.xx.xx.
As we all known, Oracle Cloud has provided SSH private key file and public key file.
How to use this private key to access Oracle Cloud VPS using vscode?
First  Step: download private key file like "ssh-key-2022-03-17.key"
Second Step: change this file privelege as 600,such as "chmod 600  ssh-key-2022-03-17.key"
Third  Step: open terminal and input "ssh-add ssh-key-2022-03-17.key"
             then test like : "ssh ubuntu@xx.xx.xx.xx". if success you connect the host.
Fourth Step: open vscode and install plugin "Remote-SSH"
Fifth  Step: open vscode "command palette",and input command "Remote-SSH:open SSH configuration file"
Sixth  Step: choice the "/Users/someone/.ssh/config",and you will see your config of SSH to xx.xx.xx.xx
SeventhStep: open vscode "command paletter", and input command "Remote-SSH:connect current window"
Eighth Step: choice the "xx.xx.xx.xx"

