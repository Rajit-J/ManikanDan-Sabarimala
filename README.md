# Manikandan Sabarimala Smart Flow

A Flask prototype exploring crowd-density and facility-queue information along the Pampa-to-Sannidhanam pilgrimage route. It is designed to demonstrate local/offline-oriented interfaces and advice using sample data.

## What it demonstrates

- Crowd and facility status views for illustrative route zones.
- Route and timing advice from local sample data.
- Offline-oriented app shell and local caching behavior.
- Manual fallback workflows and simulated connectivity conditions.

All supplied capacities, distances, elevations, timings, and crowd values are illustrative. This is not an operational crowd-monitoring or emergency service. Local-language text and emergency contact details require verification by qualified local authorities and native speakers before any real-world use.

## Technology

- Python and Flask
- HTML, CSS, and JavaScript
- Service worker and browser storage

## Run locally on Windows

Python 3.10 or later is required. In PowerShell, from the repository root:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m flask --app app run --host 127.0.0.1 --port 5104
```

Open [http://127.0.0.1:5104](http://127.0.0.1:5104). Stop with **Ctrl+C** and exit the virtual environment with `deactivate`.

## Tests

The README-provided checks are:

```powershell
python tests\smoke_test.py
node tests\engine_test.js
```

The JavaScript engine test may require the local app/server to be running as described by the project documentation.

## Before publishing

Exclude virtual environments and Python caches. Confirm team ownership and permission for photos, route information, and any other bundled data/assets. No license is included.
