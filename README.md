# ✈️ GeoFS Extra Vehicles & Planes

### A large collection of additional aircraft, ground vehicles, marine vessels, and experimental vehicles for GeoFS.

Welcome to **GeoFS Extra Vehicles & Planes** — a collection of extra vehicles designed to expand the selection of aircraft and other vehicles available in GeoFS.

This project brings together a wide variety of additional vehicles, from commercial airliners and military aircraft to helicopters, cars, buses, ships, and experimental creations.

The project includes a vehicle selection interface, an external vehicle database, compatibility indicators, and a bookmarklet option for loading the add-on.

Whether you're interested in flying something different, exploring unusual aircraft, or simply adding more variety to your GeoFS experience, this collection gives you plenty to experiment with.

> **Important:** This repository is a presentation and distribution page for the project. Original development, vehicle models, scripts, and credits belong to their respective creators.

---

## 📌 Table of Contents

1. [Project Overview](#-project-overview)
2. [Main Features](#-main-features)
3. [Vehicle Categories](#-vehicle-categories)
4. [How the Add-on Works](#-how-the-add-on-works)
5. [Installation Guide](#-installation-guide)
6. [Using the Vehicle Selector](#-using-the-vehicle-selector)
7. [Compatibility Information](#-compatibility-information)
8. [Multiplayer Information](#-multiplayer-information)
9. [Vehicle Database](#-vehicle-database)
10. [Project Files](#-project-files)
11. [Troubleshooting](#-troubleshooting)
12. [Known Limitations](#-known-limitations)
13. [Credits and Acknowledgements](#-credits-and-acknowledgements)
14. [License](#-license)
15. [Final Notes](#-final-notes)

---

## 🛩️ Project Overview

GeoFS Extra Vehicles is an add-on that expands the available vehicle selection in GeoFS.

Instead of being limited to the standard aircraft selection, users can access an additional collection of vehicles through a dedicated interface.

The collection contains several different types of vehicles:

- Commercial passenger aircraft
- Cargo aircraft
- General aviation aircraft
- Military aircraft
- Helicopters
- Experimental aircraft
- Ground vehicles
- Marine vessels
- Miscellaneous and unusual vehicles

The add-on uses JavaScript to create its interface and communicate with the GeoFS environment. Its vehicle information is stored separately in a JSON database.

This makes it possible to maintain a large collection of vehicles without placing every vehicle entry directly inside the main script.

The project also includes compatibility information to help users understand which vehicles may work with additional systems.

---

## ⭐ Main Features

### ✈️ Expanded Vehicle Selection

Access a collection of additional vehicles that goes beyond the standard GeoFS aircraft selection.

The collection includes aircraft from different manufacturers, aircraft categories, and aviation eras.

### 🚗 Multiple Vehicle Categories

The collection isn't limited to aircraft.

It also includes ground vehicles, marine vessels, and miscellaneous creations.

### 🔎 Vehicle Selection Interface

The add-on provides an additional interface for browsing and selecting vehicles.

The interface uses the vehicle database to populate its available selections.

### 🔤 Alphabetical Vehicle Organisation

Vehicle entries can be organised alphabetically, making it easier to locate a particular aircraft or vehicle.

### 🌐 External Vehicle Database

Vehicle information is stored in `vehicles.json`, separately from the main JavaScript file.

This helps keep the main script organised and allows the vehicle collection to be maintained independently.

### 🎮 Multiplayer Compatibility Information

The project includes compatibility indicators for supported multiplayer functionality.

These indicators help distinguish between vehicles with different levels of multiplayer support.

### 🎨 LiverySelector Compatibility Information

The project also provides compatibility information for LiverySelector.

This can help users identify vehicles that are supported by the additional livery-selection system.

### 🔄 Vehicle State Handling

The main script contains logic for handling aircraft and flight-state information during vehicle loading.

This is intended to help manage the transition when changing vehicles.

### 📦 Bookmarklet Support

A bookmarklet is included as an alternative way to load the add-on.

It loads the main JavaScript file from the hosted project rather than containing the entire add-on inside the bookmark itself.

---

## 🚘 Vehicle Categories

The vehicle database is organised into several categories.

The available selection depends on the entries currently included in `vehicles.json`.

### 1. Aircraft

<details>
<summary>View aircraft examples</summary>

- McDonnell Douglas MD-11
- Cessna 550 Citation II
- Eurocopter AS365 Dauphin
- Embraer E190
- Bombardier CRJ900
- Paramotor
- Starship SN5
- Ilyushin Il-76TD
- ATR 42-600
- Boeing 747-8F
- Piper PA-18 Super Cub
- Boeing 777-9X
- Tupolev Tu-144D
- Sikorsky UH-60 Black Hawk
- Airbus A350-1000
- Airbus A400M
- Antonov An-124
- Boeing 720
- Challenger 650
- DHC-6 Twin Otter Floatplane

</details>

The aircraft collection includes a mixture of commercial, military, general aviation, experimental, and unusual aircraft.

### 2. Ground Vehicles

<details>
<summary>View ground vehicle examples</summary>

- Food Service Truck
- XTerra SUV
- Sagittarius Hypercar
- Budd Metroliner
- GE P42DC Genesis
- Mazda MX-5 Miata
- Nova Bus LFS
- Ashok Leyland Tarmac Bus

</details>

Ground vehicles add another dimension to the collection beyond traditional flight simulation.

### 3. Marine Vessels

<details>
<summary>View marine vessel examples</summary>

- CMV Probability Megayacht
- Type 055 Destroyer
- Permit-Class Submarine
- Zumwalt-Class Destroyer
- Project 15A Kolkata-Class Destroyer
- Type 052D Missile Destroyer
- USS John C. Stennis Aircraft Carrier

</details>

The marine category contains a variety of vessels, including military ships, submarines, and larger civilian vessels.

### 4. Miscellaneous

<details>
<summary>View miscellaneous vehicle examples</summary>

- Northtech RADIO
- UTOPIA
- ARCHANGEL
- Proximus Hovercraft
- Northrop Grumman TR-6A Telos
- Boeing 747x
- Concorde Duplex
- Airbus A370-800
- Jetpack Wingsuit
- Weather Balloon
- A340 neo variants

</details>

This category contains unusual, experimental, and other vehicles that don't fit neatly into the previous categories.

### 5. Archived Vehicles

The database also contains an archived category for older or retired entries.

Examples include:

- Piper Cub
- Alpha Jet
- DC-3
- A380
- Concorde
- Su-35

Archived entries are kept separate from the main active vehicle categories.

---

## ⚙️ How the Add-on Works

The project uses multiple files that work together.

Understanding what each file does makes it easier to troubleshoot the add-on and understand its structure.

### 1. Main JavaScript File — `main.js`

This is the primary script.

It is responsible for creating and managing the additional vehicle interface and connecting it with the GeoFS environment.

Its responsibilities include:

- Creating the Extra Vehicles interface
- Loading vehicle information
- Organising vehicle selections
- Handling vehicle selection
- Managing vehicle-loading logic
- Displaying compatibility information
- Supporting multiplayer-related vehicle information
- Handling fallback vehicle information if the external database cannot be loaded

The main script is the central component of the add-on.

### 2. Vehicle Database — `vehicles.json`

This file contains the vehicle information used by the main script.

It stores information such as:

- Vehicle names
- Vehicle authors
- Vehicle URLs
- Vehicle identifiers
- Multiplayer-related information
- LiverySelector-related information
- Category organisation

Keeping the database separate from the main script makes the project easier to organise and maintain.

### 3. Bookmarklet — `bookmarklet.js`

The bookmarklet is a small JavaScript loader.

Rather than containing the entire add-on, it creates a script element and loads `main.js` from the hosted project.

This means the bookmarklet depends on the external script being available.

If the hosted script changes, the bookmarklet can load the updated version without requiring the user to replace the entire bookmarklet.

### 4. Archived Script — `archive.js`

This file contains an earlier version of the project.

It is retained as an archive and historical reference rather than being the primary script used by the current installation.

---

## 📥 Installation Guide

There are different ways to load the add-on, depending on your browser and preferred setup.

### Method 1 — Bookmarklet

The bookmarklet provides a quick way to load the add-on.

1. Open your browser's bookmarks manager.
2. Create a new bookmark.
3. Give it a name, such as `GeoFS Extra Vehicles`.
4. Copy the contents of `bookmarklet.js`.
5. Paste the JavaScript into the bookmark's URL or address field.
6. Save the bookmark.
7. Open GeoFS.
8. Select the bookmark to load the add-on.

**Important:** The bookmarklet currently loads the main script from the original AF267-hosted project. If you are using a separate copy or fork, make sure its loader points to the intended hosted `main.js` file.

### Method 2 — Userscript Manager

If the project provides a compatible userscript version, it can be installed through a userscript manager such as Tampermonkey.

General installation process:

1. Install a userscript manager supported by your browser.
2. Open the userscript file.
3. Create a new script in the manager.
4. Add the script's contents.
5. Save the script.
6. Open or refresh GeoFS.
7. Check whether the Extra Vehicles interface appears.

The bookmarklet and userscript approaches are different installation methods. They should not be treated as identical files.

### Method 3 — Developer Console

For users who are comfortable with browser developer tools, the main script can also be loaded manually.

The script must be hosted at an accessible URL and loaded into the GeoFS page.

This method is primarily intended for testing and development.

---

## 🎮 Using the Vehicle Selector

Once the add-on has loaded successfully, look for the Extra Vehicles interface.

The general workflow is:

1. Open GeoFS.
2. Load the add-on.
3. Open the Extra Vehicles interface.
4. Browse the available vehicle entries.
5. Find the vehicle you want.
6. Select the vehicle through the interface.
7. Allow the script to handle the vehicle-loading process.

The available vehicles are determined by the vehicle database.

If a vehicle does not appear, check whether the database loaded successfully and whether that vehicle is included in the relevant category.

---

## 🌐 Compatibility Information

The project includes compatibility indicators for certain additional systems.

These indicators are useful because not every vehicle necessarily supports every additional feature.

### Multiplayer Compatibility

The interface includes multiplayer compatibility information.

A compatibility indicator should be treated as guidance rather than a guarantee that every vehicle will behave identically in every multiplayer session.

### LiverySelector Compatibility

The project also includes LiverySelector compatibility information.

This helps identify vehicles associated with the additional livery-selection system.

### Important Compatibility Note

Compatibility can depend on the individual vehicle entry, the external system being used, and changes to GeoFS itself.

A vehicle appearing in the selection interface does not automatically mean that every feature is supported.

---

## 👥 Multiplayer Information

Some vehicle entries include additional multiplayer-related information.

The project contains logic for broadcasting supported vehicle information and displaying multiplayer compatibility indicators.

However, multiplayer support is not necessarily universal across the entire vehicle collection.

A vehicle may appear in the local selection interface without having the same multiplayer functionality as another vehicle.

For that reason, users should check the compatibility information instead of assuming every vehicle has identical multiplayer support.

---

## 📚 Vehicle Database

The vehicle database is an important part of the project.

Instead of putting every vehicle entry directly into the main JavaScript file, the project stores vehicle information in a separate JSON file.

This has several advantages:

- Easier organisation
- Easier vehicle-list maintenance
- Clear category separation
- Less clutter inside the main script
- A more manageable project structure

The database also contains information used by the main script to identify individual vehicles and their associated compatibility details.

If the external database cannot be loaded, the main script includes fallback vehicle information.

This helps the interface handle a database-loading failure, although it does not guarantee that every vehicle will be available.

---

## 🗂️ Project Files

| File | Purpose |
|---|---|
| `main.js` | Main add-on script and vehicle interface |
| `vehicles.json` | External vehicle database |
| `bookmarklet.js` | Bookmarklet loader |
| `archive.js` | Earlier archived script |
| `README.md` | Project documentation |
| `LICENSE` | Licensing information |

Each file has a different responsibility.

The main script handles the interface and loading logic, while the JSON database provides the vehicle information.

The bookmarklet provides a convenient loading method, and the archived script preserves an older version for reference.

---

## 🛠️ Troubleshooting

### The Extra Vehicles interface does not appear

Possible causes:

- The bookmarklet was not saved correctly.
- The script did not load.
- GeoFS was not fully loaded when the bookmarklet was activated.
- The browser blocked the external script.
- The hosted script was temporarily unavailable.

**What to check:**

1. Refresh GeoFS.
2. Wait for the simulator to finish loading.
3. Activate the bookmarklet again.
4. Check the browser console for script-loading errors.
5. Confirm that the hosted `main.js` file is accessible.

### The vehicle list is empty

The external vehicle database may not have loaded.

Check that `vehicles.json` is accessible and that the browser has not blocked the request.

The main script contains fallback information, but the fallback list may not contain every vehicle.

### A vehicle does not load

Not every vehicle necessarily behaves the same way.

Check the vehicle entry and its associated information.

Also check whether GeoFS has changed its internal aircraft-loading behaviour.

### Multiplayer compatibility is unclear

Check the compatibility indicator for the selected vehicle.

Remember that compatibility indicators provide guidance, not a guarantee of perfect operation.

### The bookmarklet stops working

The bookmarklet relies on an externally hosted JavaScript file.

If the file location changes or the hosting service becomes unavailable, the bookmarklet may stop loading the add-on.

Check the script URL before assuming that the bookmarklet itself is broken.

---

## ⚠️ Known Limitations

There are a few important things to understand before using the project.

- Not every vehicle has identical functionality.
- Multiplayer compatibility can vary between vehicles.
- LiverySelector support is not universal.
- The bookmarklet depends on an externally hosted script.
- The external vehicle database must be accessible for the full vehicle list.
- GeoFS updates may affect compatibility.
- Archived vehicles are not necessarily part of the active vehicle collection.
- The appearance and behaviour of individual vehicles depend on their underlying models and definitions.

This is an additional vehicle collection, not an official GeoFS feature.

---

## 🙌 Credits and Acknowledgements

This project builds on the work of its original developers and the wider community of vehicle creators.

**Original project attribution:**

- AF267
- JAaMDG
- JXT Group

The vehicle collection also contains work and contributions associated with numerous vehicle creators and model sources.

These include names credited in the original vehicle database, such as:

- FlightGear
- SeaBus
- AriakimTaiyo
- Spice9
- MirageModels
- Ryan Xu
- Aero281
- Luca
- Nightheart
- Johani

The list above is not intended to replace the individual credits attached to vehicle entries.

Please refer to the original project and `vehicles.json` for the full vehicle-specific attribution.

**A big thank-you to everyone who contributed models, scripts, vehicle information, and development work to make this collection possible.**

---

## 📜 License

The original project includes an MIT License.

Please read the included `LICENSE` file for the applicable licensing terms.

The MIT License generally permits reuse, modification, distribution, and sublicensing, subject to its conditions, including retaining the relevant copyright and permission notices.

**Important:** Retain the original copyright and attribution notices when redistributing the original project or its code.

---

## 🔗 Project Links

- **This repository:** [GeoFS Extra Vehicles & Planes](https://github.com/CaptainCedricHockeyandMTB0291/GeoFS-Extra-Vehicles-and-Planes)
- **Original project:** [AF267 — GeoFS Extra Vehicles](https://github.com/af267/GeoFS-Extra-Vehicles)
- **Original vehicle database:** `vehicles.json`
- **Original main script:** `main.js`

---

## 📝 Final Notes

GeoFS Extra Vehicles is a useful example of how JavaScript, external data files, and browser-based add-ons can work together to expand a flight simulator.

The project combines a vehicle database, a selection interface, compatibility information, and a convenient bookmarklet loader into one additional vehicle collection.

There is plenty to explore, from familiar commercial aircraft to unusual experimental vehicles and even ships and ground vehicles.

**Have fun exploring the collection, and always remember to check compatibility before assuming a vehicle supports every feature.**

---

*Documentation prepared for the CaptainCedricHockeyandMTB0291 repository. Original project development and vehicle credits remain with their respective creators.*
