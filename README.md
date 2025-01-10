# Mass Search Card

The **Mass Search Card** is an advanced search card for Home Assistant, designed to simplify interaction with Music Assistant. This card allows you to effortlessly search for artists, tracks, albums, playlists, and radio stations and play them on your selected media players.

## Features

- Supports searching for artists, tracks, albums, playlists, and radio stations.
- Dynamic dropdown selection for media players and media types.
- Popup display for search results with detailed information.
- Multi-language support (English and Dutch).
- Easy integration with Music Assistant.

## Screenshots

> **Include some screenshots here showcasing your card in action.**

---

## Installation

### HACS (Home Assistant Community Store)
1. Ensure HACS is installed in your Home Assistant setup.
2. Add this repository via HACS:
   - Go to **HACS > Integrations** and click on **+**.
   - Add the GitHub URL of this repository. (https://github.com/fastxl2024/mass-search-card.git)
3. Search for `Mass Search Card` and install the card.
4. Add the following line to your `Lovelace` resources:
   ```yaml
   resources:
     - url: /hacsfiles/mass-search-card/mass-search-card.js
       type: module

# Manual Installation
1. Download the mass-search-card.js file from this repository.
2. Place the file in the /www folder of your Home Assistant configuration.
3. Add the following line to your Lovelace resources:
   yaml
   resources:
     - url: /local/mass-search-card.js
       type: module

# Usage
type: custom:mass-search-card
language: en       

**Optional Configuration**
   language: Set the language of the card. Supported languages: en, nl.
   Default: en

**Feel free to add some languages!**

**Known bugs:** 
- scaling of card
- no "icon" when item is in library
