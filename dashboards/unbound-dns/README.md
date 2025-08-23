# Unbound DNS Dashboard
<div align="center">

**Grafana dashboard for Monitoring Unbound DNS servers via OPNsense API, including all necessary Assets.**

</div>

![Dashboard-Unbound-DNS](/screenshots/unbound-dns.jpeg)


## ✨ Dashboard Features

This Dashboard provides an Alternative to the OPNsense Unbound DNS Monitoring with the following features:

- Overall query statistics (total, resolved, blocked)
- Real-time query visualization
- Client activity tracking
- Detailed query logs with filtering capabilities
- Top passed and blocked domains
- Blocklist size monitoring

<br>

## 📋 Prerequisites

- Grafana (v11.0.0 or higher)
- Plugins:
  - Infinity Data Source
  - Business Variable Plugin
- OPNsense API Key configured in Infinity Datasource

### OPNsense Instruction
Enable Unbound Statistics:
1. Go to your OPNsense Web UI
2. Navigate to **Reporting > Settings**
3. Enable **Statistics** under **Unbound DNS reporting**

Create User & API:
1. Go to your OPNsense Web UI
2. Navigate to **System > Access > Users**
3. Create a **new User** with any Name and PW
4. Set **Privileges** to **Services: Unbound (MVC)**
5. Save the new User
6. In the Users List, use the Command on the right Column to **Create and download API key for this user** and store the File securely

### Infinity Datasource Instruction
1. Login to your **Grafana WebUI**
2. Go to "**Data Sources**" on the left Menu
3. **Add Datasource** and find "**Infinity**"
4. Go to "**Authentication**" and use "**Basic Authentication**"
5. Copy the "**key**" value from your API File into User Name
6. Copy the "**secret**" value from your API File into Password
7. Go to "**URL,Headers & Params**" and set your "**Base URL**" to your **OPNsense API Endpoint**, f.e. ```https://fw.your-domain.net/api/unbound/overview```
8. Go to "**Security**" and set the "**Allowed Hosts**" to your FW URL, f.e. ```https://fw.your-domain.net```
9. (OPTIONAL) Go to "**Health Checks**", Enable and set the URL to your Healthcheck URL , f.e. ```https://fw.your-domain.net/api/unbound/overview/isEnabled```

🎉 **You're all Set Up!**

<br>

## ⚙️ Installation

### 🔽 Import via Grafana UI

1. Clone this repository:

```bash
git clone https://github.com/IT-BAER/grafana.git
```

2. In Grafana, navigate to **Dashboards** → **+ Import**
3. Click on **Upload JSON file** and select the `dashboard.json` file from this directory
4. Before finalizing the import, ensure the dashboard is using your working data sources
5. Copy the contents of the `assets` folder to your Grafana's public assets directory:

```bash
cp -r assets/* /usr/share/grafana/public/img/bg/
```

Note: The path may vary depending on your Grafana installation

<br>

## 🚨 Troubleshooting

If images are not displaying properly:

1. Verify that the assets were copied to the correct location
2. Check Browser Dev Tools for any path-related errors
3. Ensure the image paths in the dashboard JSON match where you placed the assets



<br>

## 💜 Support Development

If you find any of these Dashboards useful, consider supporting this and future creations, which heavily relies on Coffee:

<div align="center">
<a href="https://www.buymeacoffee.com/itbaer" target="_blank"><img src="https://github.com/user-attachments/assets/64107f03-ba5b-473e-b8ad-f3696fe06002" alt="Buy Me A Coffee" style="height: 60px !important;max-width: 217px !important;" ></a>
</div>
