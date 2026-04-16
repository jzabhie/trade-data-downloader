# TRADESTAT Automated Data Downloader

Automated tool to download region-wise commodity export/import data from the Indian TRADESTAT website for January 2021 to December 2025.

## Quick Start

```bash
git clone https://github.com/jzabhie/trade-data-downloader.git
cd trade-data-downloader
pip install -r requirements.txt
python tradestat_downloader.py
```

## Features

- Downloads 1,440+ monthly trade reports automatically
- Organizes data by Region → Trade Type → Value Type
- Regions: Europe, Asia, Africa, Americas, Baltic, Unspecified
- Trade Types: Export & Import
- Value Types: USD (Million) & Quantity
- Retry logic for failed downloads
- Real-time progress tracking
- Detailed logging

## Folder Structure

```
TradeData/
├── Europe/
│   ├── Export/
│   │   ├── USD/
│   │   └── Quantity/
│   └── Import/
│       ├── USD/
│       └── Quantity/
├── Asia/
├── Africa/
├── Americas/
├── Baltic/
└── Unspecified/
```

## Requirements

- Python 3.8+
- Google Chrome browser
- Dependencies: selenium, pandas, requests, webdriver-manager

## Installation

1. Clone repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run: `python tradestat_downloader.py`

## Configuration

Edit `config.json` to customize regions, date ranges, and download settings.

## Support

Check `tradestat_download.log` for detailed download logs and troubleshooting information.