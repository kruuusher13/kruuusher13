# Romir Malik

I build machine learning systems in which computational cost is a design constraint. The work runs
from HPC down to silicon: pricing a GPT-NL data curation run on the Dutch national supercomputer
before it is launched, perception for a vehicle with no GPS, and inference on the programmable logic
of a satellite die.

MSc Applied Data Science, Utrecht University. Founding engineer at Torxflow, data scientist at
ConcertLab, and Head of External Relations at the Utrecht Data Science Community. Based in Utrecht.

**[The full record, with interactive figures and the working behind each result](https://kruuusher13.github.io/Portfolio/)**

## Selected work

**[gptnl-energy-estimation-ekf](https://github.com/kruuusher13/gptnl-energy-estimation-ekf)**
Predicts the energy, cost and CO2 of a GPT-NL data curation run on Snellius before it is launched.
A per stage law `E = c0 + c1*n` fitted from short calibration trials, an extended Kalman filter with
an innovation gate correcting the prior against live EAR telemetry, and transfer across four corpora
differing 100 fold in mean document length. Predicts a held out 400k document run to 2.8% error;
gating one contaminated reading moved final error from +93% to +8%. MSc thesis at TNO, shipped as a
command line tool with `forecast`, `monitor` and `calibrate`.

**[Chess-Bot-20M](https://github.com/kruuusher13/Chess-Bot-20M)**
Move selection as classification over the 1,968 legal UCI moves rather than as text generation, with
legality applied as a mask before the argmax so illegal moves are arithmetically unreachable. 38.9M
parameters, 12 layers, trained on 20M positions: 50% top-1 accuracy, zero illegal moves, 50 ms per
move on CPU.

**[UnitreeL1-pointLIO2](https://github.com/kruuusher13/UnitreeL1-pointLIO2)**
Containerised Point-LIO state estimation for a Unitree Go2 carrying an L1 lidar, in one Docker
environment that behaves identically on ARM64 and AMD64. Ablations locate the failure modes:
coarsening the voxel filter drifts earlier, and disabling online extrinsic estimation tilts the map
immediately.

**[APF](https://github.com/kruuusher13/APF)** and
**[BlueRov-Object-Avoidance](https://github.com/kruuusher13/BlueRov-Object-Avoidance)**
Monocular perception and artificial potential field avoidance for an unmanned underwater vehicle
with no GPS, built at CSIR National Institute of Oceanography. Monocular depth over a stereo rig
because a second pressure housing adds a failure mode and its calibration drifts with depth.
Validated in a BlueROV2 Gazebo environment, with vehicle dynamics modelled for the
[Maya AUV](https://github.com/kruuusher13/Maya_AUV).

**[Rope-augmented path following and control of a remotely operated underwater vehicle](https://ieeexplore.ieee.org/document/10465897)**
IEEE APSCON 2024. Holding an ROV steady in the turbulent water below a dam, so vision based erosion
inspection can run without sending divers down.

## Working on

**[Torxflow](https://torxflow.nl)**, as founding engineer: a garage management platform for Dutch
workshops built around three intelligence modules, smart scheduling, vehicle intelligence and AI
diagnosis, running over the systems a workshop already uses. Graduated from the UtrechtInc
validation programme.

**[ConcertLab](https://concertlab.com)**, as data scientist: the measurement layer for a filming
studio that had no instrumentation, and the strategy model behind it.

## Elsewhere

- Portfolio and CV: [kruuusher13.github.io/Portfolio](https://kruuusher13.github.io/Portfolio/)
- LinkedIn: [linkedin.com/in/romirmalik](https://www.linkedin.com/in/romirmalik/)
- Email: romir.ds10@gmail.com
