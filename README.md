# Home Dashboard Documentation

**Source**: [Reddit Post by homeassistantme](https://old.reddit.com/r/homeassistant/comments/1ggg31g/yaml_and_blanks_are_ready/)

---

### Overview

This is my complete personal Home Assistant dashboard. It includes YAML configurations and supporting graphics (both blank and native) for various elements, such as media player, location tracking, sensor management, and other custom integrations.

---

## Features

This dashboard covers a wide range of functionalities:

- **Media Player**
- **Location Map**
- **Motion Sensor Management**: Enable/disable motion sensors.
- **Medication Tracking**
- **Pet Management**: Food and water level tracking with low-level warnings connected to a flashing beacon.
- **Air Quality Monitoring**: Warning beacon attached for low quality.
- **Laundry Monitoring**: Connected to flashing beacon.
- **Vacuum Control and Mapping**
- **Room Control Pages**: Control over individual rooms and entities like blinds, curtains, lights, etc., via "hold" actions over a 3D floorplan.
- **Flight Schedule Tracking**
- **Weather Radar**
- **Reminders**: Feed fish, change cat litter, walk dog.
- **Low Battery Tracking**
- **Chore Chart**: Lists outstanding tasks on the main dashboard.
- **To-Do List**: On a dedicated page with outstanding items also listed on the main dashboard.
- **News Ticker**: Pulls from multiple feeds and displays at the screen's bottom.
- **Health Dashboard**: Includes exercise, calorie tracking, weight, and heart health.
- **Teleporter** (after some more tweaks with the Hadron Collider 😄)

---

### Compatibility Notes

- Designed for **Home Assistant Operating System**. Functionality on Docker-based setups may vary.

---

### Helpful Folder Structure

- **/local/**: Equivalent to the `/www` folder.
- **/local/lovelace/**: Stores graphics for this dashboard. You may want additional subfolders for fonts, icons, and background graphics.

---

## Required Components

### HACS Integrations

Install the following through HACS:

1. Mushroom Card Package (including `climate-card`, `vacuum-card`, `light-card`, `cover-card`)
2. Tabbed-card
3. Maxi-media-player
4. Xiaomi Vacuum Map Card
5. Auto-entities Card
6. Clock-weather-card
7. Battery-state-card
8. HTML-card
9. Digital-clock Card
10. Card-mod
11. Browser-mod
12. Button-card
13. Bubble-card
14. Passive BLE Monitor Integration
15. Mini Media Player
16. Alexa Media Player
17. Vertical Stack In Card
18. Multiple Entity Row
19. Spotify Lovelace Card
20. Auto Backup
21. Paper Buttons Row
22. Stack In Card
23. Simple Vacuum Card
24. Light Entity Card
25. Lovelace_gen
26. Office 365
27. Flight Radar24
28. Feedparser
29. Places
30. Hui-element
31. Lovelace HTML Card (for News Ticker)
32. Datetime Card
33. O365 Card

### Home Assistant Internal Integrations

Ensure the following are set up:

1. Accuweather
2. Alexa Media Player
3. Bluetooth
4. Feed Parser
5. FlightRadar24
6. Google Nest
7. HACS
8. Local Tuya
9. MQTT
10. Music Assistant
11. Office 365
12. OwnTracks
13. RESTful
14. Shopping List
15. Spotcast
16. Spotify
17. Time & Date
18. Tuya
19. Uptime
20. Vacuum Integration (like Xiaomi)
21. Z-Wave
22. Zigbee Home Automation

### Add-Ons for Home Assistant

1. File Editor
2. Home Assistant Google Drive Backup
3. Log Viewer
4. MariaDB
5. Mosquitto Broker
6. MQTT IO
7. Music Assistant Server
8. Samba Share
9. Spotify Connect
10. Studio Code Server (essential if not already installed)
11. Z-wave JS
12. Terminal & SSH

### Fonts

Install the following fonts:

1. Pathway Gothic One
2. raleway-extralight.woff2
3. raleway-light.woff2
4. Tahoma

---

## Setup Requirements

1. Install HACS and all required integrations and add-ons.
2. Create a folder named `lovelace` inside the `/www` folder.
3. Add the graphics from the attached ZIP file into the `lovelace` folder (add graphics individually without folders).
4. Create a new Dashboard Page by editing the Overview tab, naming it, and selecting "Panel" as the View Type.
5. Use the Picture Elements Card for the dashboard's main graphic layout.

### Floorplan

- Create your own floorplan using a free service like [home.by.me](https://home.by.me). This may require 4-6 hours to customize based on skill level.

### Health Dashboard

- iPhone users: Use **Health Auto Export** app to integrate health metrics. You may need a paid subscription.

---

## Example Setup

1. **Create Config Templates**: Copy the code from the "Config setup" file into `config.yaml`.
2. **Scripts and Automations**: Email `byhomeyyz@gmail.com` with the specific entity or automation name to request the YAML setup if needed.
3. **News Ticker**: Ensure Feed Parser is installed in both HACS and Integrations.

### Testing and Adjustments

Once all integrations and cards are in place, add the Picture Elements card using the YAML provided. For further assistance, email `byhomeyyz@gmail.com` with your error details.

---

## Notes

- **Graphic Editing**: This dashboard requires some graphic editing skills to customize properly.
- **Developer Appreciation**: If you use portions of this dashboard, consider supporting developers by donating on platforms like GitHub.
- **Disclaimer**: This dashboard is a personal project, shared for others who might find it useful.

---

## Helpful Resources

Below is a list of helpful resources and tools referenced in this project:

- [Card Mod Styling](https://community.home-assistant.io/t/card-mod-add-css-styles-to-any-lovelace-card/120744/1396)
- [Chore Cart Explanation and Instructions](https://theawesomegarage.com/blog/repeating-household-chores-with-scoring-system-and-awards)
- [Convert Add Fonts for Home Assistant](https://community.home-assistant.io/t/use-ttf-in-lovelace/143495/33)
- [Health Auto Export App](https://www.healthyapps.dev/)
- [Home.By.Me Free 3D Floorplan Creator](https://home.by.me/)
- [Maxi Media Player](https://community.home-assistant.io/t/maxi-media-player/705007)
- [Mushroom Card Styling Guide](https://community.home-assistant.io/t/mushroom-cards-card-mod-styling-config-guide/600472)
- [Smart Home Junkie Tutorial Videos](https://www.youtube.com/@SmartHomeJunkie)

Enjoy!
