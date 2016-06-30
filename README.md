# Python Port Checker

A basic port checker written in python. 

Can check either a single port or a range of ports, with a set timeout. Works by trying to open a socket on the desired port, if this fails the port is closed / is open with no application using it. Perhaps not the most elegant solution but it works.

# Usage 

To use run `python3 portmap.py` with the desired arguments. With no arguements will print help text.

# List of possible parameters

|Short |    Long    |  Arguments | Explanation
|:------:|:-----------:|:-----------:|-------------
|  -h  |   --help   |   none   | Display this help text
|  -u  |   --host   | hostname | Supply a hostname to probe
|  -p  |   --port   |   port   | Specify a single port to test
|  -s  |--rangestart|start port| Specify the start of a port range
|  -e  | --rangeend | end port | Specify the end of a port range
|  -t  | --timeout  | timeout  | Specify a timeout in seconds per test
