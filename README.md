# Web_Map

# Interactive Volcano & Population Web Map

An interactive, multi-layered web map application built with **Python** and **Folium**. 

The application parses real-world geological and demographic data to visualize global population distribution alongside the locations and elevations of active/historic volcanoes across the United States.

## 🚀 Features

- **Volcano Marker Layer:** Dynamic map markers pinning the exact coordinates of volcanoes.
- **Elevation-Based Color Coding:** Volcanic markers are dynamically styled based on height:
  - 🟢 **Green:** Elevation under 1000 meters
  - 🟠 **Orange:** Elevation between 1000 and 3000 meters
  - 🔴 **Red:** Elevation above 3000 meters
- **Interactive Pop-ups:** Clicking any volcanic marker displays its name and exact elevation.
- **Population Choropleth Layer:** A polygon-based GeoJSON layer that shades countries based on their population metrics to visualize density.
- **Layer Control Panel:** A fully interactive map toggle interface allowing users to independently turn the Volcanoes or Population layers on and off.

## 🛠️ Tech Stack & Libraries

- **Python 3.10
- **Folium:** For generating the interactive Leaflet.js web map.
- **Pandas:** For reading, cleaning, and structuring the volcano coordinate datasets (`Volcanoes.txt` / `.csv`).
- **GeoJSON:** For rendering geographic boundaries and polygon layers for global populations.

## 📁 Repository Structure

```text
├── app.py                # Main Python script containing the map logic
├── Volcanoes.txt         # Raw dataset containing volcano names, coordinates, and elevation
├── world.json            # GeoJSON file containing world country shapes and population metrics
└── README.md             # Project documentation
```

## 💻 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd YOUR_REPOSITORY_NAME
   ```

2. **Install the required dependencies:**
   Make sure you have `pip` installed, then run:
   ```bash
   pip install folium pandas
   ```

3. **Run the script:**
   Execute the main python application script to generate the map:
   ```bash
   python app.py
   ```

4. **View the Map:**
   The script will generate an HTML file named `Map1.html` (or your custom filename) in your root directory. Simply open this file in any web browser to view your interactive web map.

## 🎯 Learning Outcomes
Through this project, I practiced:
- Manipulating external files and datasets using the `pandas` library.
- Implementing loops to dynamically append features to a map object.
- Managing code structure with Folium FeatureGroups to isolate map elements.
- Working with geographical coordinates and parsing JSON/GeoJSON metadata
