piksi_multi_rtk
======
ROS node to read SBP messages from an attached Piksi **Multi** RTK device.

The piksi_multi_rtk package has been tested under ROS Indigo and Ubuntu 14.04, and ROS Kinetic and Ubuntu 16.04.


**WARNING:** default baud rate of the driver is set to '230400' (default baud rate of Piksi Multi is '115200').
  
## Installation and Configuration
**WARNING: install __ONLY ONE__ version of SBP library, depending of which Hardware version you are using. This page contains the driver for [Piksi Multi](https://www.swiftnav.com/piksi-multi).

The following code will automatically download the required version of libsbp and install it in the default folder `/usr/local/lib/python2.7/dist-packages/sbp-<SBP_LIB_VERSION>-py2.7.egg/sbp/`.

```
# Execute this line in the package folder 'piksi_multi_rtk'
source install/install_piksi_multi.sh
```

### Firmware and SBP Lib Version
Please check [here](https://support.swiftnav.com/customer/en/portal/articles/2492810-swift-binary-protocol) which Piksi Multi firmware version based on the current SBP Lib version.

## Advertised Topics
The most interesting advertised topics are:

 - `/piksi/navsatfix_rtk_fix` ([sensor_msgs/NavSatFix](http://docs.ros.org/api/sensor_msgs/html/msg/NavSatFix.html))
   in case of RTK fix position from Piksi then this message contains WGS 84 coordinates;
 - `/piksi/navsatfix_spp` ([sensor_msgs/NavSatFix](http://docs.ros.org/api/sensor_msgs/html/msg/NavSatFix.html))
   in case of SPP fix position from Piksi then this message contains WGS 84 coordinates;
 - `/piksi/navsatfix_best_fix` ([sensor_msgs/NavSatFix](http://docs.ros.org/api/sensor_msgs/html/msg/NavSatFix.html))
   this message contains WGS 84 coordinates with best available fix at the moment (either RTK or SPP);
 - `/piksi/enu_pose_fix` ([geometry_msgs/PointStamped](http://docs.ros.org/api/geometry_msgs/html/msg/PointStamped.html))
   this message contains ENU (East-North-Up) coordinate of the receiver in case of RTK fix. Orientation is set to identity quaternion (w=1);
 - `/piksi/enu_pose_spp` ([geometry_msgs/PointStamped](http://docs.ros.org/api/geometry_msgs/html/msg/PointStamped.html))
   this message contains ENU (East-North-Up) coordinate of the receiver in case of SPP fix. Orientation is set to identity quaternion (w=1);
 - `/piksi/enu_pose_best_fix` ([geometry_msgs/PointStamped](http://docs.ros.org/api/geometry_msgs/html/msg/PointStamped.html))
   this message contains ENU (East-North-Up) coordinate of the receiver with best available fix at the moment (either RTK or SPP). Orientation is set to identity quaternion (w=1);
   
## Rosservice
The following services are available:
 - `piksi/settings_write`: writes a specific setting to Piksi Multi;
 - `piksi/settings_read_req`: requests a parameter to Piksi Multi;
 - `piksi/settings_read_resp`: reads the latest response of a "settings_read_req" request;
 - `piksi/settings_save`: saves the current settings of Piksi Multi to its flash memory.
