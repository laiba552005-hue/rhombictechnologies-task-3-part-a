# 📍 IP Geolocation Map Viewer

## Description

This Python project retrieves the user's approximate location using their public IP address and displays it on an interactive map.

The program:

* Detects your current location using an IP geolocation API.
* Extracts the city, country, latitude, and longitude.
* Prints the location details in the terminal.
* Creates an interactive HTML map using Folium.
* Places a marker on your detected location.
* Automatically opens the generated map in your default web browser.

---

# Features

* 🌍 Detects approximate location from IP address
* 📌 Displays latitude and longitude
* 🏙️ Shows city and country information
* 🗺️ Generates an interactive map
* 🌐 Opens the map automatically in the browser

---

# Technologies Used

* Python 3
* requests
* folium
* webbrowser

---

# Requirements

Install the required libraries:

```bash
pip install requests folium
```

---

# Project Structure

```
project/
│
├── location.py
├── location_map.html   (generated automatically)
└── README.md
```

---

# How to Run

1. Install Python 3.
2. Install the required packages:

```bash
pip install requests folium
```

3. Save the code in a file named:

```text
location.py
```

4. Run the program:

```bash
python location.py
```

---

# Sample Output

```
City: Lahore
Country: Pakistan
Latitude: 31.5497
Longitude: 74.3436

Map created successfully!
```

The program will generate:

```
location_map.html
```

and automatically open it in your default web browser.

---

# How It Works

1. Sends a request to the IP geolocation API.
2. Receives location data in JSON format.
3. Extracts:

   * City
   * Country
   * Latitude
   * Longitude
4. Creates an interactive Folium map.
5. Adds a marker at the detected location.
6. Saves the map as `location_map.html`.
7. Opens the map in the browser.

---

# Note

* The detected location is based on your **public IP address**.
* The result is an **approximate location** and may not represent your exact GPS position.
* Accuracy depends on your Internet Service Provider (ISP), VPN usage, and the geolocation database.

---

# Future Improvements

* Add live GPS support
* Show ISP information
* Display region and postal code
* Reverse geocoding to show full address
* Track multiple locations with markers
* Export location data to CSV or JSON

---

# License

This project is free to use for educational and learning purposes.
