# Recap of computer networking

## OSI 
	> For computer to communicated with each other 
		> OSI – 7 layers  
			> 7 / Application  
			> 6 / Presentation  
			> 5 / Session  
			> 4 / Transport  
			> 3 / Networking  
			> 2 / Data link  
			> 1 / Physical  

## Layer 1  
    > Analog modem  
        > Modulates signal digital-to-analog  
        > Demodulates signal analog-to-digital  
    > Hub  
        > Replicates signal to the other ports  

## Layer 2  
    > Switch  
        > ASIC chip  
            > Works with MAC address  
    > Wireless access point (WAP)  
        > Connects wireless/wired network segments  

## Layer 3  
    > Multilayer switch (MLS)  
        > Most common in layer 3 than 2  
        > ASIC chip works higher than layer 2  
    > Router  
        > Most common device to connect networks  
        > Uses software to learn about routes between networks  

## Security devices  
    > Firewall  
        > Allows or deny network traffic  
        > Can be hardware or software  
    > Intrusion detection system (IDS)  
        > Informs when malicious actions have occurred (they are passive)  
    > Intrusion prevention system (IPS)  
        > Take action against malicious activities are detected  

## Optimization and performance devices  
    > Load balancer (content switch)(content filler) (hardware or software)  
        > Balance request across multiple devices that contain the same data  
    > Proxy server  
        > Acts on behave of a client device to fulfill requests to retrieve data  
        > Also can limit what requests are fulfilled  

## Network services and application  
    > Virtual private network (VPN)  
        > Allows remote sites or users to access a private network  
        > Functions as a local segment  
        > Site to site VPN  
            > Connects two sites together  
        > Remote-access VPN (host to site VPN)  
            > Allow users to connect but requires user to have preconfigured VPN clients installed on their system  
        > Host to host VPN (SSL VPN)  
            > Allows user to connect to the private network without VPN client software  
    > IPsec  
        > Most common protocol for secure VPN connection  
        > Layer 3 and above  
        > Generic Routing Encapsulation (GRE)  
            > Tunneling protocol that encapsulate wide variety of other networks layer protocol  
            > Used with IPsec for multicast and broadcast packet transmission  
        > Point-to-Point Tunneling Protocol (PPTP)  
            > Older VPN technology that supports dial-up VPN connections  
        > TLS  
            > Cryptographic protocol that provides authentication services  
            > Used in web based transactions  
            > Replaced SSL  
        > SSL  
            > Similar to TLS but replaced by it  
        > Network access service (NIC)  
            > Operates on layer 2 and 1  
            > Determines which network protocol a device will use on the network  
            > Converts the network bits into electrical signal  
        > RADIUS  
            > AAA protocol used to authenticate end users  
            > Robust accounting features  
        > TACACS+  
            > AAA protocol used to authenticate end devices  
            > Encrypts all transmissions between devices  
        > RAS  
            > Description of software and hardware required for remote access connection  
            > Not a protocol  
        > Web services  
            > Allow disparate software or platforms to communicate.  
            > Uses XML format that most software can understand  
        > Unified voices services  
            > Description of software and hardware for voice communication into a network  

## DHCP in the network  
    > Static IP  
        > Administrator supplies specific IP  
    > Dynamic IP  
        > Uses DHCP to distribute IP  
    > DHCP  
        > How it works  
            > Sends discovery packets  
            > Offer packets to let the device know the DHCP has required information  
            > When it receives the packet, the device sends a request packet for IP  
            > DHCP gets the requested packet, it responds with an acknowledgement packet  
        > Uses UDP port 67  
        > UDP port 68 to provide the IP to PC  
        > IP address comes from scope (range) of addresses  
        > Admin reserves a pool of addresses  
            > Includes  
                > Default gateway  
                > DNS server  
                > Time servers  
                > Other options  
        > Addresses are leased and it expires, but can request the same IP  
    > DHCP relay  
        > Used when DHCP server is not on local network segments  

## DNS service  
    > DNS servers  
        > Maps human-friendly names to IP addresses  
        > Uses root, TLD and local to resolve FQDN (Fully Qualified Domain Name) to the right IP address  
        > Responses either authoritative or non-authoritative  
    > DNS records  
        > A  
            > Records map hostnames to IPV4 addresses  
        > AAAA  
            > Records map hostnames to IPV6 addresses  
        > CNAME  
            > Records map canonical names to hostnames  
        > PTR  
            > Records point to canonical names  
        > MX  
            > Records point to the email server that handles the email for a given domain  
    > DDNS  
        > Lightweight adjustments to the local DNS database  
        > Useful for networks that don't use static IP addresses  
        > DDNS updating  
            > Automatically updates DNS records without manually inputting the information  

## Network address translation (NAT)  
    > Solves the problem of how to route non-routable IP addresses  
    > Transforms private IP address into a routable public IP address  
        > (since private IP can't cross public IP network)  
        > Which allows access outside the local network  
    > SNAT (static NAT)  
        > Private IP address gets assigned a specific public IP address  
    > DNAT (Dynamic NAT)  
        > Private IP address gets assigned a dynamic public IP address from available pool of addresses  
    > PAT (Port Address Translation)  
        > Extends the capabilities of DNAT  
        > Dynamically sends IP address and port numbers to the public IP  
    > NAT terminology  
        > Inside local  
            > Private IP inside the local network  
        > Inside global  
            > Public IP inside the local network  
        > Outside local  
            > Private IP outside the local network  
        > Outside global  
            > Public IP outside the local network
