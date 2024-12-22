# Network-traffic-analysis-using-tcpdump-Analysis-with-wireshark

Intro: Tcpdump is a command-line packet sniffer that can directly capture and interpret data frames from a file or network interface. It was built for use on any Unix-like operating system and had a Windows twin called WinDump. It is a potent and straightforward tool used on most Unix-based systems. It does not require a GUI and can be used through any terminal or remote connection, such as SSH.

TCPDump is available for most Unix systems and Unix derivatives, such as AIX, BSD, Linux, Solaris, and is supplied by many manufacturers already in the system. Due to the direct access to the hardware, we need the root or the administrator's privileges to run this tool. For us that means we will have to utilize sudo to execute TCPDump as seen in the examples below. TCPDump often comes preinstalled on the majority of Linux operating systems.

# Validating if the package exists.
-	Which tcpdump, command use to validate on hour. Often it can be found in /usr/sbin/tcpdump. 
![image](https://github.com/user-attachments/assets/fc9bf2c7-67f8-4974-b533-60ea7c58527f)
-	However, if the package does not exist, we can install it with:

-	Sudo apt install tcpdump

We can run the tcpdump package with the --version switch to check our install and current package version to validate our install.
-	Sudo tcpdump –version 
![image](https://github.com/user-attachments/assets/25907153-6f6f-44be-bccf-84e7a3e4fb9d)

Traffic Captures with Tcpdump
Because of the many different functions and filters, we should first familiarize ourselves with the tool's essential features. Let us discuss some basic TCPDump options, demo some commands, and show how to save traffic to PCAP files and read from these.
Basic Capture Options
Below is a table of basic Tcpdump switches we can use to modify how our captures run. These switches can be chained together to craft how the tool output is shown to us in STDOUT and what is saved to the capture file. This is not an exhaustive list, and there are many more we can use, but these are the most common and valuable.
Switch Command	Result
D	Will display any interfaces available to capture from.
i	Selects an interface to capture from. ex. -i eth0
n	Do not resolve hostnames.
nn	Do not resolve hostnames or well-known ports.
e	Will grab the ethernet header along with upper-layer data.
X	Show Contents of packets in hex and ASCII.
XX	Same as X, but will also specify ethernet headers. (like using Xe)
v, vv, vvv	Increase the verbosity of output shown and saved.
c	Grab a specific number of packets, then quit the program.
s	Defines how much of a packet to grab.
S	change relative sequence numbers in the capture display to absolute sequence numbers. (13248765839 instead of 101)
q	Print less protocol information.
r file.pcap	Read from a file.
w file.pcap	Write into a file
Man Page Utilization
To see the complete list of switches, we can utilize the man 
![image](https://github.com/user-attachments/assets/15a8222b-795d-4e6f-a4f3-0c63dcbd72d6)
![image](https://github.com/user-attachments/assets/8aa2a931-4721-42a4-8ebc-57cb7ee68129)
Here are some examples of basic Tcpdump switch usage along with descriptions of what is happening:
Listing Available interfaces:
For more info please visit word document. Thanks!




