# Developer Notes

## 2020-01-01:
* Added visualization support (tello_viz.launch).
* Changed IMU and odometry axes mapping to follow North-West-Up (right hand axes).
* Added timestamp to camera messages.
* Removed orientation from IMU messages (as the message values should be in IMU frame itself).
* IMU messages get published at 15Hz which is slower than the camera messages (30Hz). This causes issues in IMU pre-integration in VINS-Fusion.