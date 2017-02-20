# Penetration Testing Documents and Tools

## Methodology

Reconnaissance --> scanning --> Exploitation --> Post Exploitation ( maintaining Access / Cleaning Tracks (BH Only) )


## Websites

* [exploit-db](http://www.exploit-db.com) 
* [netcraft](http://netcraft.com)
* [https://www.robtex.com/](https://www.robtex.com/) "swiss army knife internet tool" a one-stop shop for information gathering

## Google Dorking

**site:domain.com** search google on a specific domain

**allintitle:index of** keywords that are all in the title

**inurl:admin** words in the url

**cache:domain.com** search cache pages only for data

**filetype:pdf** limit search to filetype only.

## Attack Operating Systems

* blackbuntu
* Kali
* NodeZero
* Pentoo
* SamuraiWTF
* Backtrack

## Victim Operating Systems
* [Metasploitable](https://sourceforge.net/projects/metasploitable/files/Metasploitable2/) A linux distro  
* Windows XP - Because LOL


# Tools

## DNS
* `nslookup` --> `server <ip address>` --> `type all`
* `dig@<ipaddress> -t AXFR`
* `fierce -dns codecreations.net`


## Data Extraction
### metagoofil
run `metagoofil -d codecreations.net -t pdf,doc,xls,pptx -l 75 -n 100 -o results -f results.html`

This will put the results in the folder results.



### theHarvester
Finds emails and servers

run

 `theharvester -d codecreations.net -l 10 -b google`

 or  `theharvester -d codecreations.net -l 10 -b google` for more all areas to search like linkedin, PGP, bing etc.


### mitmproxy
Man in the middle software
[https://mitmproxy.org/](https://mitmproxy.org/)


## Documents
