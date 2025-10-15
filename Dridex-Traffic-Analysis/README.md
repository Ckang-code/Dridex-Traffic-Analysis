# Dridex Traffic Analysis (Work in Progress)
This repository contains an ongoing project analyzing Dridex malware traffic.  
The workflow begins with packet inspection in Wireshark, moves into documenting findings,  
and culminates in the development of Suricata IDS rules tested against real-world PCAPs.

## About This Project
This work references and builds upon Unit42’s published Dridex analysis and tutorial material.  
While Unit42 provides an excellent foundation for exploring Dridex traffic, this project takes the  
exercise deeper by developing custom Wireshark profiles, documenting detailed observations,  
and extending the analysis into Intrusion Detection through custom Suricata rules.  
The end goal is to move beyond traffic review and demonstrate how findings can be codified  
into actionable detections and repeatable workflows.

## Contents
- **wireshark-profile/** – Custom Wireshark configuration and filters for TLS, beaconing, and anomaly detection.
- **pcaps/** – Reference Dridex PCAPs from Unit42 (linked externally for licensing reasons).
- **analysis/** – Draft write-up of traffic analysis (Word document, later exported to Markdown/PDF).
- **suricata-rules/** – Custom Suricata signatures (to be developed and tested).
- **results/** – Screenshots, packet statistics, and I/O graphs from Wireshark and Suricata.

## Goals
1. Analyze the Dridex infection chain from initial loader traffic through stage loading to command-and-control communications.  
2. Examine TLS handshakes, certificate anomalies, and beaconing behavior.  
3. Document indicators of compromise (IOCs) across multiple stages of the infection lifecycle.  
4. Develop Suricata detection rules based on observed behaviors at each stage.  
5. Test rules against PCAPs to validate detection accuracy.  
6. Provide a repeatable workflow for translating malware traffic analysis into IDS detections.  

## Status
- Initial Wireshark profile created for enhanced view of web traffic, but I a customizing further for granular view of TLS metadata (i.e. certificate data)
- PCAPs collected (Unit42 samples)  
- Analysis draft in progress  
- Suricata rule development and testing planned 

## References
- [Unit42 Wireshark Tutorial – Dridex Infection Traffic](https://unit42.paloaltonetworks.com/wireshark-tutorial-dridex-infection-traffic/)  
- [Unit42 Dridex PCAP Collection](https://github.com/pan-unit42/wireshark-tutorial-Dridex-traffic/)  
- [Suricata Documentation](https://suricata.readthedocs.io/en/latest/)
