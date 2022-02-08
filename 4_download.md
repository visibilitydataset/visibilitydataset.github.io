---
sort: 4
---

# Download & Tools

## Request Downloads

The dataset is provided on-demand, by following a [request link](https://forms.gle/o1boKS4LL6jzCR137). Please fill out a simple form to us, and you will get a automated response mail containing full download links.

```note
Please note that only education domains (*.edu, *.ac.* etc.) are allowed for download.
```

The shortcut for the calibration parameters are also [here](https://urserver.kaist.ac.kr/publicdata/ViViD++/calibration/calibration_results.zip).


## Development tools

If you are not familiar with rosbag files, you could use our simple image undistort & saver [script](https://urserver.kaist.ac.kr/publicdata/ViViD++/process_img.py).
For saving non-image sensors as a csv or text file, simple imu / event image saver [script](https://urserver.kaist.ac.kr/publicdata/ViViD++/process_dvs.py) will help.

Locate the script in the same folder with the bagfile, and running the script will save your images in the folder named "rgb" or "ther". You will also find a text file containing
gps coordinate (UTM) oriented in start point of driving-campus-day1 with corresponding timestamps, in the "gpslist.txt" file.

```note
- About Timestamps

The timestamps recorded from the sensor clock are recorded in the headers of each message, and is different from the timestamp recorded in the bag message. Please ignore the message timestamps and only use the timestamps in the message header.
```

### process_img.py
process_img script searches image and gps messages from from the bagfile, and saves them as in text and png format.

### process_dvs.py
process_dvs script observes the gps and images in the folder, and generates event images by searching events from the bagfile.

### Functions
#### write_gps(message, gps_file)
write_gps function writes UTM coordinates to given GPS_file, converted from gps message.

#### write_images(message, image_folder)
write_images function undistorts and writes desired RGB or Thermal images, into the desired image_folder, with timestamp filename.

#### raw_to_kelvin(value)
raw_to_kelvin function transforms the values obtained from 14-bit thermal image to real kelvin temperature.

#### update_event_q(message, eventlist)
update_event_q function sorts and transforms the events from the message, and returns as a eventlist class object.

#### generate_event_img(event_folder, eventlist, timestamp)
generate_event_img function generates an event image into the event_folder, by collecting all events around the given timestamp, in 5ms. If there's less than 1% of events, it skips.


## Dataset structure

```
dataset
├── process_img.py
├── process_dvs.py
├── calibration
│   ├── driving_results
│   ├── handheld_results
│   └── handheld_targets
├── driving_full
│   ├── campus_day1.bag
│   ├── campus_day2.bag
│   ├── campus_evening.bag
│   ├── campus_night.bag
│   ├── city_day1.bag
│   ├── city_day2.bag
│   ├── city_evening.bag
│   └── city_night.bag
├── driving_vision
│   ├── campus_day1.bag
│   ├── campus_day2_2.bag
│   ├── campus_day2.bag
│   ├── campus_evening.bag
│   ├── campus_morning_2.bag
│   ├── campus_morning.bag
│   ├── campus_morning_manual.bag
│   ├── campus_morning_manual_small.bag
│   ├── campus_night_2.bag
│   ├── campus_night.bag
│   ├── city_day1.bag
│   ├── city_day2.bag
│   ├── city_evening.bag
│   ├── city_morning.bag
│   ├── city_morning_manual.bag
│   ├── city_night.bag
│   ├── urban_day.bag
│   ├── urban_evening.bag
│   ├── urban_evening_road.bag
│   ├── urban_morning.bag
│   ├── urban_morning_manual.bag
│   └── urban_night.bag
├── handheld_indoor
│   ├── dark_aggresive.bag
│   ├── dark_robust.bag
│   ├── dark_unstable.bag
│   ├── global_aggressive.bag
│   ├── global_robust.bag
│   ├── global_unstable.bag
│   ├── local_aggressive.bag
│   ├── local_robust.bag
│   ├── local_unstable.bag
│   └── varying_robust.bag
└── handheld_outdoor
    ├── outdoor_robust_day1.bag
    ├── outdoor_robust_day2.bag
    ├── outdoor_robust_night1.bag
    ├── outdoor_robust_night2.bag
    └── pose
        ├── map_outdoor_robust_day1.pcd
        ├── map_outdoor_robust_day2.pcd
        ├── map_outdoor_robust_night1.pcd
        ├── map_outdoor_robust_night2.pcd
        ├── path_outdoor_robust_day1.csv
        ├── path_outdoor_robust_day2.csv
        ├── path_outdoor_robust_night1.csv
        └── path_outdoor_robust_night2.csv
```

