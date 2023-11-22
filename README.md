# trackpad_issue_fix
In some laptops, especially Lenovo, the trackpad doesn't work in Ubuntu, or some other Linux distros. The fix for that is provided here.

<br>

Open terminal and type <br>
`gedit /etc/default/grub`
<br>
A configuration file will be opened. Add the following line in this file <br>
`GRUB_CMDLINE_LINUX="i8042.nopnp=1 pci=nocrs"`
<br>
Save the file. After closing the file, in the terminal, enter <br>
`update-grub` <br>
Restart the system. <br>
Done <br> <br>
Created by Vishnu Hidesh, BCA 2021 - 24, KBMGCT <br>
Github: https://github.com/vishnuhidesh <br>
