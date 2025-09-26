                                        Firewall Configuration on Windows
The objective of this task was to configure and test basic firewall rules on Windows using 

Windows Defender Firewall to block and test traffic on port 23 (Telnet).   

Implementation Steps


Firewall Status Check: Windows Defender Firewall was opened and verified to be enabled for private, public, and domain profiles. The default settings showed that    

inbound connections were blocked unless a rule allowed them, and outbound connections were allowed unless a rule blocked them.   



Rule Creation: A new inbound rule was created using the 'New Rule Wizard' in 'Advanced Settings':   



Rule Type: Port.   



Protocol: TCP.   



Port: 23 (Telnet).   



Action: Block the connection.   



Testing the Block: The blocking rule was tested using the Telnet client.Running the command    

telnet localhost 23 in the Command Prompt resulted in the message: "Could not open connection to the host, on port 23: Connect failed".This confirmed the firewall rule was effective.   


Rule Removal: The inbound rule named "Port 23" was deleted to restore the system to its original state.   

Conclusion
The task successfully demonstrated fundamental firewall management skills—creating, verifying, and deleting rules—by effectively blocking inbound traffic on Telnet port 23. A firewall works by filtering network packets according to defined rules, where traffic matching a block rule (like TCP on port 23) is rejected
