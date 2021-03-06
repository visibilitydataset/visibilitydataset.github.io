---
sort: 3
---

# Calibration

## Sensor Coordinates

For verification, we show the sensor coordinates plots with the actual sensors installed, for each systems.

- Driving
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/drive_system.png" width="85%" height="auto" />
</div>

- Handheld
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/hand_system.png" width="65%" height="auto" />
</div>

## Calibration Procedure

The calibration was mostly done by generating observable images from alternative vision sensors, and running [Kalibr](https://github.com/ethz-asl/kalibr) on it.

<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/calib_targets.png" width="100%" height="auto" />
</div>

We used a special type of calibration pattern, which is checkerboard pattern printed on PCB. The heated PCB checkerboard shows different heat dissipation rate on aluminum and plastic parts, thus it is both observable in the RGB camera(a) and thermal(b). For the event camera, we use [E2VID](https://github.com/uzh-rpg/rpg_e2vid) to reconstruct an apriltag(c).

## Calibration Results

 - RGB to LiDAR
<table>
<tr>
  <td align = "right">
    <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align1.png" width="100%" height="auto" />
  </td>
  <td align = "left">
    <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align2.png" width="100%" height="auto" />
  </td>
</tr>
</table>

 - Thermal to LiDAR
<table>
<tr>
<td align = "right">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align1t.png" width="100%" height="auto" />
</td>
<td align = "left">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align2t.png" width="100%" height="auto" />
</td>
</tr>
</table>

 - Event(reconstructed) to LiDAR
<table>
<tr>
<td align = "right">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align1e.png" width="100%" height="auto" />
</td>
<td align = "left">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/example_align2e.png" width="100%" height="auto" />
</td>
</tr>
</table>

 - Event to RGB-D (handheld)
<div class="t3iYD" style="text-align: center;">
 <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/hand_dvs_align.png" width="40%" height="auto" />
</div>

   - Thermal to RGB-D (handheld)
<div class="t3iYD" style="text-align: center;">
 <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/hand_ther_align.png" width="40%" height="auto" />
</div>

   - LiDAR to RGB-D (handheld)
<div class="t3iYD" style="text-align: center;">
 <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/hand_vlp_align.png" width="40%" height="auto" />
</div>

## Sample Algorithms

- ORB-SLAM reconstruction (campus)
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/campus_orb2.png" width="100%" height="auto" />
</div>

- Visual Place Recognition (campus)
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/vpr.png" width="100%" height="auto" />
</div>

- LOAM reconstruction (campus)
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/campus_sample.png" width="100%" height="auto" />
</div>

## Discussions on thermal vision

- ORB-SLAM benchmarks
<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/orb_result_table.png" width="60%" height="auto" />
</div>

<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/orb_table_explain.png" width="80%" height="auto" />
</div>

<div class="t3iYD" style="text-align: center;">
<img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/orb_explain.png" width="80%" height="auto" />
</div>
