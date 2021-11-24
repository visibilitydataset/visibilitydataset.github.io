---
sort: 1
---

## Sensor Specifications

<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/table2.png" width="100%" height="auto" />
</div>

## Sequences

We provide a dataset from two distinct sensor systems, handheld and driving.

<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/table3.png" width="100%" height="auto"/>
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/table4.png" width="100%" height="auto"/>
</div>


```
dataset
├── process_img.py
├── process_dvs.py
├── calibration
│   ├── driving_results
│   ├── handheld_files
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
