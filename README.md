# ✈️ GeoFS Extra Vehicles and Planes

**More aircraft. More vehicles. More ways to fly.**

Welcome to **GeoFS Extra Vehicles and Planes**, a community add-on project designed to expand the standard GeoFS experience with additional aircraft, helicopters, ground vehicles and other extra vehicles.

This project uses a `.jxt` script to introduce additional vehicle options into GeoFS, giving pilots more things to explore beyond the default aircraft selection.

Whether you're testing aircraft, exploring the simulator, or just looking for something different to fly, this add-on is built to make GeoFS a little more interesting.

---

## 🌟 Features

- **✈️ Extra Aircraft:** Expand your aircraft selection with additional vehicle models.
- **🚁 Helicopters:** Additional rotorcraft options where supported by the script.
- **🚗 Ground Vehicles:** Explore additional ground vehicle options.
- **🛩️ Expanded Selection:** Access additional vehicles through the simulator's selection interface when successfully loaded.
- **⚙️ Lightweight Design:** Designed to add functionality without unnecessarily complicating the simulator.
- **🔧 Easy Installation:** Follow the installation instructions to get started.
- **🌐 GeoFS Integration:** Designed specifically for use with the GeoFS flight simulator.

## 📦 Project Contents

| File | Description |
|---|---|
| `extra-vehicles.jxt` | Main extra vehicles script |
| `README.md` | Project documentation and installation guide |

*Additional files and vehicle models may be included as the project develops.*

---

## 🛠️ Requirements

Before installing, make sure you have:

- A working installation of [GeoFS](https://www.geo-fs.com/).
- A modern browser such as Microsoft Edge, Google Chrome or Firefox.
- The project script downloaded from this repository.
- A compatible script loader if your particular script format requires one.

**Recommended:** Desktop browsers provide the most flexibility for script installation and troubleshooting.

---

## 📥 Installation Guide

There are different ways to load the add-on, depending on the format of the script.

### Method 1 — Tampermonkey (If compatible)

1. Install the Tampermonkey browser extension.
2. Open the Tampermonkey dashboard.
3. Select **Create a new script**.
4. Open `extra-vehicles.jxt` from this repository.
5. Copy its JavaScript contents.
6. Paste the code into the Tampermonkey editor.
7. Make sure the code has the required userscript metadata if Tampermonkey needs it.
8. Save the script.
9. Open GeoFS and check whether the extra vehicles load.

**Important:** A `.jxt` extension does not automatically mean a file is a valid Tampermonkey userscript. The contents must be compatible JavaScript, with suitable userscript metadata when required.

### Method 2 — Browser Developer Console

If the script is compatible with direct execution:

1. Open GeoFS.
2. Wait for the simulator to finish loading.
3. Open your browser's Developer Tools.
4. Select the Console tab.
5. Paste the script's JavaScript contents.
6. Press Enter.
7. Check the aircraft or vehicle selection menu.

**Note:** Console-loaded scripts are temporary. You may need to run them again after refreshing GeoFS.

---

## 🎮 Using the Add-On

Once the script has loaded successfully:

1. Enter the GeoFS simulator.
2. Open the aircraft selection menu.
3. Look for the additional vehicles.
4. Select an available vehicle.
5. Enjoy exploring the expanded simulator experience!

Vehicle availability depends on the script version and the models it supports.

---

## 🔧 Troubleshooting

Having trouble? Here are a few things worth checking.

| Problem | Possible Solution |
|---|---|
| Vehicles aren't appearing | Check that the script loaded successfully. |
| Script isn't running | Check browser permissions and script compatibility. |
| Tampermonkey doesn't recognise the file | Check whether the `.jxt` contents are valid userscript-compatible JavaScript. |
| GeoFS isn't loading properly | Temporarily disable other GeoFS add-ons and test again. |
| Vehicles disappear after refreshing | Reload the script if using the temporary console method. |
| An update breaks compatibility | Check the repository for the latest version. |

### ⚠️ Compatibility Notice

GeoFS is an independently developed simulator and its internal systems can change.

Changes to the simulator may affect how additional vehicles are loaded, displayed or selected.

Compatibility is not guaranteed across every GeoFS version, browser or device.

---

## 🧑‍💻 Development & Contributions

This project is intended to grow alongside the GeoFS community.

Ideas, suggestions, bug reports and improvements are welcome.

You can contribute by:

- Reporting bugs through GitHub Issues.
- Suggesting additional aircraft or vehicles.
- Improving documentation.
- Submitting compatible improvements through pull requests.
- Helping test new releases.

Please include useful information when reporting an issue, such as your browser, GeoFS version and the problem you encountered.

---

## 📋 Project Information

| Category | Information |
|---|---|
| Project | GeoFS Extra Vehicles and Planes |
| Platform | GeoFS Flight Simulator |
| Main File | `extra-vehicles.jxt` |
| Script Format | JXT / JavaScript, depending on file contents |
| Repository | GitHub |
| Developer | CaptainCedricHockeyandMTB0291 |
| Project Type | Community Add-On |
| License | See repository license |

---

## ⚠️ Disclaimer

This is an independent community project and is not an official GeoFS product.

It is not affiliated with, endorsed by or maintained by the official GeoFS development team.

Use the add-on at your own discretion. Always keep a backup of your original files and scripts before making modifications.

---

## ✈️ Final Words

GeoFS is already a great flight simulator, but there's always room for a few more aircraft, vehicles and experiments.

This project is about expanding what's available, trying new things and making the simulator more enjoyable.

**Thanks for checking out the project.**

Happy flying, and enjoy the extra vehicles! 🛫

**— CaptainCedricHockeyandMTB0291**
