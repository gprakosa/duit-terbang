# Duit Terbang 💸

![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-iOS%20Shortcut-lightgrey.svg)
![Google Forms](https://img.shields.io/badge/Ingestion-Google%20Forms-673AB7?logo=googleforms&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Datastore-Google%20Sheets-34A853?logo=googlesheets&logoColor=white)
![Gemini](https://img.shields.io/badge/AI-Gemini-4285F4?logo=google&logoColor=white)

Ever felt like your money just... flies away?

**Duit Terbang** is a free tool to catch your flying money directly from your iPhone. From Indonesia, for anyone who needs it 🇮🇩. 

## Overview

**Duit Terbang** is used for logging daily expenses, designed for personal use with zero infrastructure overhead.

This project uses the iOS Shortcuts platform as the interface and Google services as the backend (Google Forms as the ingestion endpoint, Google Sheets as the datastore, and Gemini as the AI model for receipt parsing via a simple API call). Everything can run on free tiers.

**Duit Terbang** is the game changer. Why? 

- 📱 **Straightforward:** iOS Shortcut is fast and easy to modify.
- 🎯 **Sovereign:** Your data lives on your own Google Sheets.
- ⚡ **Secure:** Form link and API key are stored on your iCloud. 

## Prerequisites
* A __Google__ account (the free one).
* An __iPhone__ (no iPhone 17 Pro Max 2 TB required).
* Some __money__ to be spent (spending it wisely, thank me later). 

## Quick Start
Create a [Google Form](from-scratch/README.md#create-a-google-form), get a [Gemini API Key](from-scratch/README.md#create-a-gemini-api-key),  download the [iOS shortcut](https://github.com/gprakosa/duit-terbang/releases) and run it.

> You will be prompted for the pre-filled Google Form URL and Gemini API Key on the first run.

#### Google Form

|Question/Column|Type|Response validation|
|:---|:---|:---|
|*Timestamp*|*Auto*|
|`Kategori`|Short answer| |
|`Deskripsi`|Short answer| |
|`Nominal`|Short answer|Number; Is number; Custom error text|
|`Latitude`|Short answer|Number; Is number; Custom error text|
|`Longitude`|Short answer|Number; Is number; Custom error text|

## From Scratch

Want to build it from scratch instead? [This guide](from-scratch/README.md) walks you through every step (great if you're new to iOS Shortcuts).

## Roadmap

Started as a sharing session demo. Ended up as something worth releasing. 

This project focuses on shipping the shortcut for data ingestion. However, you can pivot, filter, chart, or export the data to any tool you want. 

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) for the details.