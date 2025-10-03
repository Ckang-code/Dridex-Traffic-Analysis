# Wireshark Profile for Dridex Traffic Analysis

This directory contains a customized Wireshark profile for HTTP and TLS traffic analysis,  
adapted from the Unit42 Dridex tutorial and tuned for this project.

## Usage
- Import the profile into Wireshark:
  1. Go to **Edit → Configuration Profiles → Import**.
  2. Select the `HTTP_TLS_Wireshark_Profile.zip` file in this folder.
- Once imported, switch to the profile via the profile selector in Wireshark’s status bar.

## Features
- Custom columns for TLS metadata:
  - Server Name Indication (SNI)
  - JA3 fingerprint
  - TLS version
 
- Filters tuned for:
  - HTTP request traffic
  - TLS ClientHello and Certificate handshakes
  - Quick spotting of anomalous or suspicious sessions

## Files
- `HTTP_TLS_Wireshark_Profile.zip` – Import-ready Wireshark profile.
