# PINS---Ideation

This contains the code, files, presentation for Ideation 2023 by team EWhizard.
This works better in [Google Colab](https://colab.research.google.com/drive/1WMq66Qe55pfc9ScyMlnHwejvfAOlZYyh?usp=sharing "PINS-Ideation 2023").
[Click here to view the presentation](https://www.canva.com/design/DAFYGIAl9-g/FcR_1MPzJziyDlbtKEkagw/view?utm_content=DAFYGIAl9-g&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink "PINS -Canva Presentation").

---

## PSG Indoor Navigation System

an interactive mapping and navigation tool that uses Python and the Folium library to visualize and navigate through the blocks of PSG College of Technology (PSGCT), leveraging Geo Maps API and interactive widgets. 

---

## Features

1. **Interactive Map Navigation:**
   - Displays an interactive map with markers and routes.
   - Highlights pathways between selected starting and destination points.

2. **Customizable Location Resources:**
   - Dynamically loads and manages GeoJSON files to represent buildings and pathways.

3. **Dynamic Widgets for Interaction:**
   - Selectors for start and target locations allow for easy navigation through a user-friendly widget interface.

4. **Pathway Visualization:**
   - Shows animated paths using `folium.plugins.AntPath` for a clear and visually appealing route.

5. **Building Highlighting:**
   - Displays the outline of the target building to help users orient themselves better.

---

## Getting Started

### Prerequisites

- Python 3.7 or higher.
- Required Python libraries:
  - `folium`
  - `ipywidgets`
  - `pandas`
  - `json`
  - `os`

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/hajay180505/PINS---Ideation.git
   cd PINS---Ideation
   ```

2. Install the required Python libraries:
   ```bash
   pip install folium ipywidgets pandas
   ```

3. Ensure your GeoJSON files for routes and buildings are correctly organized in the project directory.

---

## Usage

1. **Run the Main Script:**
   Execute the script to launch the interactive navigation interface.
   ```bash
   python pins_start.py
   ```

2. **Select Start and Destination:**
   - Use the `Start` widget to choose your starting location.
   - Use the `Target` widget to select your destination.

3. **View Routes:**
   - The map will display a pathway from the start to the target location, along with the destination building highlighted.

4. **Customization:**
   - Modify `geoResources` to include your specific GeoJSON files for pathways and building outlines.

---

## Code Overview

### Main Classes and Functions

- **`navigator` Class:**
  - Manages the loading of GeoJSON files.
  - Handles route drawing and building highlighting on the map.
  
- **Key Methods:**
  - `changeDestination(newDestination)`: Updates the target destination.
  - `changeStartPoint(newStartPoint)`: Updates the starting point.
  - `redrawMap()`: Refreshes the map display with the selected start and target.

- **Interactive Widgets:**
  - `selectHouse_widget`: Dropdown for selecting the target.
  - `selectPosition_widget`: Dropdown for selecting the starting point.

---

*Happy navigating!* 🚀



