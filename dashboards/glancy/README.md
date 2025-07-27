# Glancy Dashboard

<div align="center">

**Grafana dashboard for aggregating content from multiple sources including Reddit, Twitch, YouTube, and GitHub.**

</div>


#### Dashboard
![Dashboard-Glancy](/screenshots/glancy-dashboard.jpeg)
#### Config
![Dashboard-Glancy](/screenshots/glancy-config.jpeg)

## ✨ Dashboard Features

This Dashboard provides a centralized view of content from various sources:

- **Reddit Posts** from specified Subreddits
- **Twitch Channels** incl. Thumbnail Preview and **Top Games**
- **YouTube Feeds** from selected Channels
- **GitHub Release** from chosen Repositories
- Custom **Bookmarks** with Icons
- **Calendar**
- Custom **Search Engine**

<br>

## 📋 Prerequisites

- Grafana (v12.1.0 or higher)
- Reddit API (Infinity Data Source)
- Plugins:
  - Infinity Data Source
  - Business Calendar Panel
  - Business Text Panel
  - Business Forms Panel

### Reddit API Instruction
1. Go to your **[Reddit Apps](https://www.reddit.com/prefs/apps/)**
2. **Create** an App and name it as you like
3. Choose "**Script**"
4. Set the "**redirect uri**" to your Grafana Url
5. Create the App
6. Store the Value under your App Name and the Secret

### Infinity Datasource Instruction
1. Login to your **Grafana WebUI**
2. Go to "**Data Sources**" on the left Menu
3. **Add Datasource** and find "**Infinity**"
4. Go to "**Authentication**" and use "**Basic Authentication**"
5. Copy the "**value**" under the Reddit Apps name into User Name
6. Copy the "**secret**" value from your Reddit App into Password
7. Go to "**URL,Headers & Params**" and set your "**Base URL**" to **```https://reddit.com/r```**
8. Go to "**Security**" and set the "**Allowed Hosts**" to **```https://reddit.com```** and **```https://www.reddit.com```**

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
