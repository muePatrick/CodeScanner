Simple Python script to scan codes (barcodes, qr-codes, etc.) through the webcam and type it with a virtual keyboard (similar to a hardware barcode scanner).

# Installation

1. Follow https://pypi.org/project/pyzbar/

2. Run `pip install -r requirements.txt`

# Usage

Run `python main.py`.

Alternatively you can select a different webcam, append a enter behind the scanned code or suppress typing:
```
usage: main.py [-h] [--cameraId CAMERAID] [--cameraDevice CAMERADEVICE] [--printDelay PRINTDELAY] [--appendEnter | --no-appendEnter] [--type | --no-type]

options:
  -h, --help            show this help message and exit
  --cameraId CAMERAID, -i CAMERAID
                        Index of the webcam to use (overwritten by --cameraPath)
  --cameraDevice CAMERADEVICE, -d CAMERADEVICE
                        Absolute path to the webcam device (overwrites --cameraId)
  --printDelay PRINTDELAY, -t PRINTDELAY
                        Delay until code is typed again
  --appendEnter, --no-appendEnter
                        Press enter key when code is scanned (default: False)
  --type, --no-type     Type scanned code with a virtual keyboard (default: True)
```