# Glancy Navigation Bar Panel

<div align="center">

**Grafana panel for creating a custom navigation bar that dynamically links to all dashboards tagged with "glancy".**

</div>

### Screenshot
![Glancy-Navbar](/screenshots/glancy-navbar.png)
### Demo
![Glancy-Navbar](/screenshots/glancy-navbar-demo.gif)
## ✨ Dashboard Features

This panel provides a custom navigation bar for Grafana dashboards tagged with "glancy" with the following features:

- **Dynamic Dashboard Links**: Automatically fetches and displays links to all dashboards tagged with "glancy"
- **Active Link Detection**: Highlights the currently active dashboard
- **Animated Navigation**: Smooth hover effects and transition animations
- **Responsive Design**: Adapts to different screen sizes
- **Sticky Positioning**: Remains visible while scrolling through dashboard content
- **Custom Styling**: Semi-transparent gradient background with modern UI elements
- **Library Panel Support**: Best used as a Library Panel for consistent navigation across your tagged dashboards

<br>

## 📋 Prerequisites

- Grafana (v12.0.0 or higher)
- Plugins:
  - Dynamic Text Panel (marcusolsson-dynamictext-panel)

<br>

## ⚙️ Installation

### 🔽 Import via Grafana UI

1. Clone this repository:

```bash
git clone https://github.com/IT-BAER/grafana.git
```

2. In Grafana, navigate to **Dashboards** → **+ Import**
3. Click on **Upload JSON file** and select the `panel.json` file from this directory
4. Before finalizing the import, ensure the panel is using the correct data source

### 📚 Using as a Library Panel (Recommended)

For the best experience with consistent navigation across all your "glancy" tagged dashboards:

1. After importing the panel, convert it to a Library Panel:
   - Click on the panel title
   - Select "More" (three dots) → "Make library panel"
   - Give it a name like "Glancy Navigation Bar"
   - Save the library panel

2. Add the Library Panel to your dashboards:
   - In any dashboard, click "Add" → "Visualization"
   - Search for your library panel name
   - Select it and add it to your dashboard

3. Tag your dashboards:
   - For each dashboard you want to appear in the navigation, add the tag "glancy"
   - Go to dashboard settings → "Tags" → Add "glancy"

🎉 **You're all Set Up!**

<br>

## 🚨 Troubleshooting

If the navigation links are not populating:

1. Verify that you have other dashboards tagged with "glancy"
2. Check that the Grafana API is accessible from the panel
3. Ensure you're using a compatible version of Grafana

If styling appears incorrect:

1. Check that no other CSS is conflicting with the panel styles
2. Verify that the panel is positioned correctly in your dashboard layout

If the panel doesn't stay sticky while scrolling:

1. Ensure no other CSS is overriding the sticky positioning
2. Check that your dashboard layout allows for sticky positioning

<br>

## 💜 Support Development

If you find any of these Dashboards useful, consider supporting this and future creations, which heavily relies on Coffee:

<div align="center">
<a href="https://www.buymeacoffee.com/itbaer" target="_blank"><img src="https://github.com/user-attachments/assets/64107f03-ba5b-473e-b8ad-f3696fe06002" alt="Buy Me A Coffee" style="height: 60px !important;max-width: 217px !important;" ></a>
</div>
