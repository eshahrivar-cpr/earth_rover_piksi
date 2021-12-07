^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package piksi_rtk_msgs
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Forthcoming
-----------
* upgrade msgs to v1.11.0
* Contributors: Ebrahim Shahrivar

1.8.2 (2019-02-08)
------------------
* pkg version
* Driver Modified
* Contributors: Andres

1.8.1 (2018-10-29)
------------------
* Merge pull request `#62 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/62>`_ from ethz-asl/pre-master-merge
  Fix in message ASCII code
* Update release number.
* Merge pull request `#60 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/60>`_ from joshjowen/pre-master-merge
  Changed apostrophe to ASCII in device monitor description to fix unicode error
* Changed apostrophe to ASCII in device monitor description to fix unicode error in rosbags
* Contributors: Marco Tranzatto, joshjowen, marco-tranzatto

1.8.0 (2018-10-25)
------------------
* Merge pull request `#58 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/58>`_ from ethz-asl/fix/version_and_readme
  update version number and readme
* update version number and readme
* Contributors: Marco Tranzatto, marco-tranzatto

1.7.1 (2018-06-20)
------------------
* Merge pull request `#55 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/55>`_ from ethz-asl/fix/kml_set_sim_time
  [kml] set global param use_sim_time.
* [kml] set global param use_sim_time.
* Contributors: Marco Tranzatto, marco-tranzatto

1.7.0 (2018-06-19)
------------------
* Merge pull request `#54 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/54>`_ from ethz-asl/fix/version_number
  fix version number.
* fix version number.
* Merge pull request `#53 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/53>`_ from ethz-asl/feature/kml_simple_path
  Feature/kml simple path
* Update version number.
* Merge pull request `#51 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/51>`_ from ethz-asl/fix/master_in_fix_melodic
  Fix/master in fix melodic
* Merge branch 'master' into fix/master_in_fix_melodic
* Contributors: Marco Tranzatto, kh, kholtmann, marco-tranzatto

1.6.3 (2018-06-13)
------------------
* Merge pull request `#49 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/49>`_ from ethz-asl/feature/remove_anyworker_dependency
  [Gui] Replace any_worker with ros::Timer.
* Contributors: kholtmann

1.6.2 (2018-06-06)
------------------
* Merge pull request `#47 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/47>`_ from ethz-asl/fix/gui_cmakelist
  Fix/gui cmakelist
* Updated semantic version to 1.6.2
* Merge branch 'master' into fix/gui_cmakelist
* Contributors: kh, kholtmann

1.6.1 (2018-05-31)
------------------
* Merge pull request `#46 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/46>`_ from ethz-asl/fix/version_tag
  Updated version tag in all packages.
* Updated version tag in all packages.
* Contributors: kh, kholtmann

1.6.0 (2018-05-30)
------------------
* Merge pull request `#41 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/41>`_ from ethz-asl/feature/jenkins
  Feature/jenkins
* Set up install space correctly for piksi_multi_rtk_ros.
* Contributors: Marco Tranzatto, marco-tranzatto

1.5.0 (2018-05-24)
------------------
* Merge pull request `#39 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/39>`_ from ethz-asl/feature/firmware_1_5_12
  Feature/firmware 1.5.12 with lib SBP 2.3.15
* Added DeviceMonitor message.
* Added again uart_state, to be checked during next field test.
* Added support for SBAS fix.
* [Msgs] update PosLlhMulti with new flags.
* Switching to Firmware 1.5.12 and lib SBP 2.3.15
* Contributors: Marco Tranzatto, marco-tranzatto

1.4.0 (2018-05-17)
------------------
* Merge pull request `#37 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/37>`_ from ethz-asl/fix/version_number_and_indentation
  Fix version number and indentation.
* Fix version number and indentation.
* Merge pull request `#35 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/35>`_ from Wagdi-Benyaala/master
  magnetometer implementation
* magnetometer implementation
* Merge branch 'master' into feature/cleanup_gui
* Merge pull request `#27 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/27>`_ from ethz-asl/revert-24-fix/install_space
  Revert "Fix/install space"
* Revert "Fix/install space (`#24 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/24>`_)"
  This reverts commit 28ba3ad5bc3a9494911429b89bce8323c95fd0f7.
* Contributors: Marco Tranzatto, Wagdi, kh, marco-tranzatto

1.3.0 (2018-04-25)
------------------
* Fix/install space (`#24 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/24>`_)
  fix install space. RQT plugin still to be fixed.
* Contributors: Marco Tranzatto

1.2.0 (2018-03-28 17:07)
------------------------
* Merge pull request `#22 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/22>`_ from ethz-asl/feature/geodetic_survey_enu_origin
  ENU origin based on geodetic survey and specified height of the base station.
* Compute ENU origin based on geodetic survey and specified height of the base station.
* Contributors: Marco Tranzatto, marco-tranzatto

1.1.0 (2018-03-28 09:04)
------------------------
* Merge pull request `#16 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/16>`_ from ethz-asl/feature/lib_sbp_2_3_10
  LibSBP 2.3.10
* Update version number in every packages.
* Fix BasePosLlh and added BasePosEcef
* Fix import baseline_heading and add base_pos_llh message.
* Working on Observation message when in debug mode
* Contributors: Marco Tranzatto, marco-tranzatto

1.0.6 (2018-03-27)
------------------

1.0.5 (2018-03-21)
------------------

1.0.3 (2018-03-01)
------------------

1.0.2 (2017-12-21)
------------------
* Merge pull request `#4 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/4>`_ from ethz-asl/fix/after_hoengg_test
  Fixes after Hoengg test
* use message strings to set fix_mode.
* Contributors: Marco Tranzatto, marco-tranzatto

1.0.1 (2017-12-14)
------------------

1.0.0 (2017-12-01)
------------------
* Merge pull request `#1 <https://github.com/eshahrivar-cpr/earth_rover_piksi/issues/1>`_ from ethz-asl/import/piksi_drivers
  Import Piksi Drivers from mav_rtk_gps repo.
* update package.xml version
* importing piksi_rtk_msgs from mav_rtk_gps repo.
* extracting  folder piksi_rtk_msgs.
* Contributors: Marco Tranzatto, marco-tranzatto
