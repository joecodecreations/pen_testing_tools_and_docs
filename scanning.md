# Scanning

## Acquire Target List

Use **fping** to get a list of ip addresses that are responding on the network.

`fping -a -g 192.168.0.1 192.168.0.254 > hosts.txt`

This will sweep the range of ip addresses looking for an active computer.

The `-a` will only report back the active computers.

This writes the file to a new file called hosts.txt.

Once you have the list of targets, move onto port scanning.

## Port scanning

There are a total of 65,536 ports on every computer.

They will either be:
* Transmission control protocol (TCP)

or
* datagram protocol (UDP).

Use Nmap to find open ports:

`nmap -sT -Pn 192.168.0.115` This will search the 1000 common ports.

A more extensive search can be performed using `nmap -sT -p- 192.168.0.115`.

Additionally, you can scan ranges by appending a range value `nmap -sT 192.168.0.1-254`

throw all results into a file by appending `> ./portscan.txt`

The above `-sT` was targeting TCP connections. We can also target specific SYN scan (syn/ack).

To test the entire network with this we can run something like:

`nmap -sS -Pn 192.168.0.1-254 > ./SYNportscan.txt`

Which will do the range 1-254 using only those smaller SNY packets.

##### Input From File

Instead of using an ip range you can use the previously found hosts in `hosts.txt` by appending `iL hosts.txt` to your command.

Check other by typing `nmap`. Other features include:

* OS detection
* Firewalls/iDS evasion and spoofing
* 
