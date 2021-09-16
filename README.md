# OpenTX2GPX
OpenTX2GPX converts OpenTX Log file contains GPS telemetry data to GPX file. 

OpenTX2GPX reads timestamp, GPS coordinate, speed, altitude, number of GPS satelites from OpenTX log and exports to GPX track points.

## Setup
### Python environment
If you have Python 3.x environment, just you need to do following.
- pip install gpxpy
- python3 OpenTXGPX.py
### MacOS
Download and extract OpenTX2GPXMac.zip. OpenTX2GPX is MacOS executable.
### Windows
Download and extract OpenTX2GPXMac.zip. OpenTX2GPX.exe is Windows executable. 
Some of antivirus program may show trojan alert. I hope that you can setup antivirus software to ignore/bypass OpenTX2GPX.

## Usage
![main menu](images/OpenTX2GPX.png)
1. Click "OpenTX Log" button to select OpenTX log file. Sample log file is available at https://github.com/nkozawa/OpenTX2GPX/blob/main/samples/CRSF-2021-08-29.csv.
2. Timestamp fields will be filled up if OpenTX log file contains valid GPS data. Timestamp shows first valid GPS data entry.
3. If you need to change the timestamp, please modify timestamp fields and click "Update" button. Timestamp of all log entries will be updated accordingly.
4. OpenTX log usually contains multiple sessions (flights). Select pull down to a session to make GPX file.
5. Select GPX1.0 or GPX1.1. GPX1.0 contains 'speed' tag, but GPX1.1 does not. Some applications may accept only GPX1.1.
6. Click "Export GPX" button to export GPX file.

## Additional Informatios
- OpenTX is open source firmware for RC radio trasnmitter. It has ability to logging telemtry data from RC receiver on the drone or plane. If GPS device is available on the drone or plane, we will have GPS coordinate, speed and altitude. OpenTX log is stored on the SD card of RC radio as CSV format.
- GPX (GPS Exchange Format) is supported by various softwares and web sites. This is most convinent data format to carry GPS log entries.

## Links
- Google Earth
- Garmin VIRB Edit (only accepts GPX1.1)
- Dashware (Windows only)
