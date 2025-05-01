# infrastructure modernization plan

## Overview
This repository contains a comprehensive migration plan for transitioning an aging, on-premises IT infrastructure to a modern, cloud-native architecture on AWS. The plan outlines solutions for Active Directory, DNS, DHCP, databases, email systems, application servers, web hosting, and storage—tailored for enterprise scalability, availability, and long-term operational efficiency.

## Purpose
As part of a collaborative project, our team was tasked with creating a cloud migration strategy for a simulated enterprise environment with legacy systems across multiple remote offices. The goal was to design a modern infrastructure that supports:

- Scalable and hybrid-ready identity and access management
- Reliable and centralized DNS resolution
- Streamlined email and ERP systems
- Cloud-first application hosting and storage
- Secure, compliant, and resilient networking

## My Contributions

### Active Directory & DNS Migration

I led the research and planning for migrating Active Directory (AD) and DNS infrastructure to AWS, focusing on scalability, hybrid integration, and fault tolerance. My recommendations included:

- Migrating on-premises AD to **AWS Managed Microsoft AD**, enabling forest trusts and hybrid compatibility for secure, seamless authentication across environments.
- Replacing legacy DNS servers with **Amazon Route 53 Private Hosted Zones**, using conditional forwarders to preserve on-prem resolution during hybrid operations.
- Transitioning DHCP functions using **VPC DHCP Option Sets** to maintain consistent IP allocation in AWS while retaining legacy services temporarily during cutover.

This approach reduces hardware dependency, increases directory availability, and enables centralized identity management across cloud services.

### Research Focus 
To inform our recommendations, I evaluated:

- Performance specs and constraints of the existing AD/DNS infrastructure
- AWS Directory Service capabilities and forest trust configurations
- DNS failover and name resolution strategies in hybrid environments
- Best practices for DHCP migration and phased transitions

  ## Team
This project was developed as part of CS 4843 – Cloud Computing  
University of Texas at San Antonio – Spring 2025  
Instructor: Professor Juan M. Valadez

- Damien Beltran – Active Directory & DNS Servers
- Alex Estevez – Networking & Client Needs
- Nico Cruz – ERP, Databases, Email
- Adrian Arizpe – Application & Web Servers
- Patricia Harrison – Storage & Compliance
