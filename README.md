# Conbinis Visits Analyser

This small Python Notebook project counts the number of unique convenience stores (conbinis) you've visited using your Google Maps Location History data.

## How it works

The project analyzes your Google Maps Timeline data (previously known as Location History) to identify and count unique conbinis you've visited over a given period.

## Prerequisites
1.	You need to have had your Google Maps Location History (now called Timeline) enabled during the period you wish to analyze.
2.	Since there is no official Google Maps Location History API, you must manually export your location data.
3.	You need a Google Maps API key with access to the Places API. Store this key in a `.env` file as described below.

## How to get your Timeline data

As of 2024, Google no longer stores Location History on its servers. Instead, it's stored locally on your device and can be accessed as Timeline data.

### Steps to export your data:
1.	On your Android phone, open the Settings app.
2.	Navigate to:
Location → Location Services → Timeline → Export Timeline Data.
3.	This will generate a file called Timeline.json.
4.	Transfer the Timeline.json file to this project folder.

## Usage
1.	Create a `.env` file in the project root with the following content:
```sh
GOOGLE_MAPS_API_KEY=your_actual_api_key_here
```
2.	Open the provided Python Notebook (`main.ipynb`) in Google Colab, VS Code, or any compatible notebook environment. If executed locally, use [uv](https://docs.astral.sh/uv/getting-started/installation/) to install the dependencies.
3.	Follow the instructions inside the notebook to run the analysis and see your results.
