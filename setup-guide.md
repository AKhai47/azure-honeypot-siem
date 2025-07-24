# ⚙️ Setup Guide

## ☁️ 1. Azure Resource Deployment
- Create a subscription and resource group
- Set up a Virtual Network and Subnet
- Deploy a Windows 10 VM

## 🔓 2. Simulate Vulnerable Host
- Open all inbound traffic on NSG
- Disable Windows firewall from within the VM
- Attempt failed logins to generate Event ID 4625

## 📊 3. Logging & Sentinel Integration
- Create Log Analytics Workspace (LAW)
- Install Azure Monitor Agent on the VM
- Connect Sentinel to LAW
- Enable "Windows Security Events via AMA"

## 🌍 4. GeoIP Watchlist & Attack Map
- Upload `geoip-summarized.csv` as a Sentinel Watchlist
- Use KQL to enrich IP data with geographic info
- Build an interactive attack map in Sentinel Workbook
