# Unbound DNS Grafana Dashboard

Grafana dashboard for monitoring Unbound DNS servers, complete with all necessary assets.


### Screenhot
![Dashboard-Unbound-DNS](https://github.com/user-attachments/assets/71d4c57b-0fcf-4c36-9eb8-8863c675652b)


## Installation

### Prerequisites

- Grafana (v11.0.0 or higher)
- Plugins:
  - Infinity Data Source
  - Business Variable Plugin
- OPNsense API Key configured in Infinity Datasource
- (optional) n8n for formatting OPNsense API Responses


### Import via Grafana UI

1. Clone this repository:

```bash
git clone https://github.com/IT-BAER/grafana.git
```

2. In Grafana, navigate to **Dashboards** → **+ Import**
3. Click on **Upload JSON file** and select the `dashboard.json` file from the `/grafana/dashboards/unbound-dns` directory
4. Before finalizing the import, ensure the dashboard is using your working data sources
5. Copy the contents of the `assets` folder to your Grafana's public assets directory:

```bash
cp -r grafana/dashboards/unbound-dns/assets/* /usr/share/grafana/public/img/bg/
```

Note: The path may vary depending on your Grafana installation


## Troubleshooting

If images are not displaying properly:

1. Verify that the assets were copied to the correct location
2. Check Browser Dev Tools for any path-related errors
3. Ensure the image paths in the dashboard JSON match where you placed the assets


## Support Development 💜

If you find this Dashboard useful, consider supporting this and future creations, which heavily relies on coffee:

<a href="https://www.buymeacoffee.com/itbaer" target="_blank"><img src="https://github.com/user-attachments/assets/64107f03-ba5b-473e-b8ad-f3696fe06002" alt="Buy Me A Coffee" style="height: 60px !important;max-width: 217px !important;" ></a>
