# NMAP
Known as "Network Mapper" and a free, open-source tool for network security.
<br> NMAP identifies: 
<br>  - Which systems are up? <br>  - What services are running on these systems? <br/>

## Fundamental Use Cases
  1. Nmap Live Host Discovery
  2. Nmap Basic Port Scans
  3. Nmap Advanced Port Scans
  4. Nmap Post Port Scans


## To Discover Live Host, NMAP uses: 
  1. ARP scan: This scan uses ARP requests to discover live hosts
  2. ICMP scan: This scan uses ICMP requests to identify live hosts
  3. TCP/UDP ping scan: This scan sends packets to TCP ports and UDP ports to determine live hosts.

## NMAP Scan Model
![NMAP Discovery](https://user-images.githubusercontent.com/111991325/211160601-0920fbef-335c-4ab6-a8c6-21cde421f05b.jpg)

## Enumerating Targets
- Scanning Technique to specify targets:
  - List: 10.0.0.1 example.com (these are two different devices via IP or DNS)
  - Range: 10.0.0.1-10 
  - Subnet: 10.0.0.1/30
 
 - Protocols to discover the live hosts. Starting from bottom to top, we can use:
    - ARP from Link Layer
    - ICMP from Network Layer
    - TCP from Transport Layer
    - UDP from Transport Layer

## Host Discovery using ARP
