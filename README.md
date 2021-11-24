# A project page for ViVID++

This paper is a proceeding work of the unpublished paper "ViViD : Vision for Visibility Dataset", best poster presentation of ICRA 2019 Workshop/Tutorial - Dataset Generation and Benchmarking of SLAM Algorithms for Robotics and VR/AR. After prior submission, the scale of experiment has been expanded to include driving sequences, with more details on dataset statistics and characteristics. Also, the models of event camera and LiDAR was changed to provide higher resolution.

# Keywords

Data Sets for SLAM; Data Sets for Robotic Vision; Data Sets for Robot Learning

# Overview

<div class="t3iYD" style="text-align: center;">
  <img class="CENy8b" role="img" src="https://urserver.kaist.ac.kr/publicdata/ViViD++/figures/visibility.png" width="90%" height="auto" />
</div>

 An overview of the sensor system and the dataset. We set up different sensor configurations for handheld (upper left) and driving (upper right). Sensor systems include RGB, thermal, events, depth, and interial measurements. Each sensor is indicated with the letter box. Each sensor's visibility differences are displayed in the lower row. Relative to RGB, thermal and event show less variance to the illumination condition.

 <video width="640" height="360" controls>
   <source src="https://urserver.kaist.ac.kr/publicdata/ViViD++/RAL2021-video-main.mp4" type="video/mp4">
 </video>

# Related Links
There's a lot of excellent work that was introduced for SLAM Developments. For example, [Awesome SLAM Datasets](https://sites.google.com/view/awesome-slam-datasets/) lists up State-Of-The-Art SLAM datasets. And you may also want to check [Complex Urban Dataset](https://irap.kaist.ac.kr/dataset/) containing large scale and long term changes.

# The Dataset

{% include list.liquid all=true %}

# Special thanks to
[Sungho Yoon](https://scholar.google.com/citations?user=PUvBz80AAAAJ&hl=ko&oi=ao/) and Joowan Kim for contributions on the dataset configuration.

# Website License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
