# Wireshark


## Introduction
Wireshark is a popular open-source network protocol analyzer that allows users to capture and analyze network traffic in real-time. By capturing packets as they travel across a network, Wireshark can provide valuable insights into the behavior of network applications and devices. From a cyber security perspective, Wireshark can be used to detect and investigate security incidents, identify malicious activity, and troubleshoot network performance issues. For security purposes, the I.P address of the destinations and sources in the lab have been omitted. 

For this project, the following represent the required actions needed:

- Filter by "HTTP"
- Review streamed information between the source and target.
- Filter for a specific IP address and confirm the protocol.
- Confirm the victim's AD environment and confirm the number of clients logged into the domain.
- Locate the victim's host name given an IP address.
- Identify the MAC address of the infected windows client.
- Identify the user account name of the infected Windows host.



# Basic Filters
Using Wireshark to filter for unsecured protocols is simple for users as they can easily apply filters such as "http" or "ftp" to quickly identify unencrypted traffic. This allows SOC analysts to pinpoint potential security vulnerabilities and threats within the network, enabling them to take appropriate action to mitigate risks and protect sensitive data.


![image](https://github.com/dbriones49/Wireshark/assets/143753667/110dfa3e-d584-4c50-87ee-aca5dc42da74)



# Statistics Filter
Using the Statistics menu allows you to filter from a variety of options, including endpoints and packet length. Here I used a filter for protocol.

![image](https://github.com/dbriones49/Wireshark/assets/143753667/96f19235-e0c9-4a34-ae53-72b8d9369f8a)



![image](https://github.com/dbriones49/Wireshark/assets/143753667/c984a2d6-66e6-42d3-b477-fa6f184ff012)




# Information in Data Stream
By right clicking on an event, You can choose FOLLOW< TCP/HTTP STREAM and view both the information received from the source, and the response from the target.


![image](https://github.com/dbriones49/Wireshark/assets/143753667/33dd87ac-a3be-4530-891f-12f50339aeda)


# Filter for a Specific IP
Here you can enter a query for a specific IP address. This address used the TCP.
![image](https://github.com/dbriones49/Wireshark/assets/143753667/79c3762e-c4fc-4880-b769-403d82eee922)




# Confirm domain name and number of clients
By right clicking on the pcap and then filtering for TCP stream data, I confirmed the domain name and that there were three clients logged in to the domain.
![image](https://github.com/dbriones49/Wireshark/assets/143753667/92913213-5a49-4d99-b64c-293139e889d3)


# Locating username and MAC address
I filtered by the victim's IP address and with a NameString query, and was able to obtain the noted information. 


![image](https://github.com/dbriones49/Wireshark/assets/143753667/ddff9d7c-5933-4175-b42e-cbee502f1121)

# Conclusion
Wireshark has strong filtering capabilities that enable cybersecurity professionals to extract specific information from vast amounts of data, making it an essential tool for cyber forensics investigations. By utilizing Wireshark's filtering features, organizations can enhance their cyber posture by identifying and mitigating threats more efficiently, ultimately improving their overall security posture.






