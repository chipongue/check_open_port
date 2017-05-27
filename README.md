# check_open_port
Monitoring of ports of communication.

Port of communication is a number identifying the application to which the data of communication is destined. In this way, the data is sent directly to the corresponding application, identified by the port. For this reason, it becomes important to control the open ports, for being input and output ports in the system. Uncontrolled open ports can represent a window so that malicious users can access the system and extract what they are interested in.

This Nagios plugin monitors ports, and alerts about opening new port of communication. As arguments are passed the list of authorized ports, and the IP address of the machine to be monitored (local), returning the critical state if one or more open ports are found.

Mandatory arguments: The following arguments must be specified when the module is executed:

-H or --hostaddress used to specify the IP address to be scanned.

-p or --port used to specify ports authorized to be open.

Optional arguments: The following arguments are optionally invoked, as user needs:

-V or --version used to query the module version.

-A or --author used to query the author's data.

Command-Line Execution Example:

./check_open_port.py -H 192.168.2.35 -p 21,25,80

