# NIST-Cybersecurity-Framework-Respond
Analyze the situation using the National Institute of Standards and Technology's Cybersecurity Framework (NIST CSF) and create an incident report that you can include as part of your cybersecurity portfolio documentation. The CSF is a voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk.

### Table of contents

1. [Introduction](#introduction)
2. [Objective](#objective)
3. [Incident Report Analysis](#analysis)

## Introduction <a name="introduction">
You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 

To address this security event, the network security team implemented: 

- A new firewall rule to limit the rate of incoming ICMP packets

- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets

- Network monitoring software to detect abnormal traffic patterns

- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

## Objective <a name="objective">
As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). You will use the CSF to help you navigate through the different steps of analyzing this cybersecurity incident and integrate your analysis into a general security strategy:

- **Identify** security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 

- **Protect** internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 

- **Detect** potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 

- **Respond** to contain, neutralize, and analyze security incidents; implement improvements to the security process. 

- **Recover** affected systems to normal operation and restore systems data and/or assets that have been affected by an incident.

## Incident Report Analysis <a name="analysis">

| **Summary** |    |
| ----- | ----- |
| Identify | The organization's network services stopped responding due to an incoming flood of ICMP packets. Normal network traffic could not access any network resources. Investigation showed that the flood of ICMP packets was sent through a configured firewall. Due to this vulnerability, the malicious actor overwhelmed the company's network with a Distributed Denial of Service (DDoS) attack.|
| Protect | To protect from future DDoS attacks, the network security team  implemented new firewall rules that limit the rate of incoming ICMP packets, verification the Source IP address in the firewall to check for spoofed IP addresses on incoming ICMP packets, implemented IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics, and network monitoring software to detect abnormal traffic patterns |
| Detect | To detect similar DDoS attacks, network monitoring software to detect abnormal traffic and source IP address verification of spoofed IP addresses through the firewall. |
| Respond | The incident management team responded to the DDoS attack by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. For future security events the cybersecurity team will isolate affected systems to prevent disruption of critical systems and services. The team will analyze network logs for suspicious activity. All incidents should be reported to upper management. |
| Recover | Availability of the network services should be stored to normal. Firewall should be configured to black external ICMP flood attacks. All non-critical services should be halted  to reduce internal network traffic. Critical network Services should be restored first. Once the attack has been stopped restore all non-critical services. This incident took over two hours to recover from, and both IT and security teams worked together to bring the network back to normal business operations. Normal checks will be implemented so all systems and firewalls are configured properly. Update Incident playbook from lessons learned. |
