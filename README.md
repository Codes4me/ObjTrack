# ObjTrack

A browser-based tool for tracking an object's center of mass across a photo or video and exporting its position to CSV.

## Features

- Upload a photo/video, or use your webcam to snapshot/record one
- Click to manually mark an object's center of mass
- Color-based auto-tracking follows the marked point frame-by-frame in video, with manual correction at any time
- Optional two-point scale calibration to also export real-world `x_cm`/`y_cm` alongside pixel coordinates
- Built-in calibration mode to compare auto-tracked points against your manual ones and auto-search for the tolerance/search-radius settings that minimize tracking error
- Exports all logged points to CSV

## Usage

No build step or dependencies. Serve the folder and open it in a browser:

```
python3 -m http.server 8000
```

Then open `http://localhost:8000`. Camera access requires `localhost` or HTTPS.
