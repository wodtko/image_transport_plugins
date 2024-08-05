^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package compressed_image_transport
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

5.0.0 (2024-07-31)
------------------
* Added common linters to compressed_image_transport (`#167 <https://github.com/ros-perception/image_transport_plugins/issues/167>`_)
* Contributors: Alejandro Hernández Cordero

4.0.1 (2024-07-22)
------------------
* Removed warning (`#164 <https://github.com/ros-perception/image_transport_plugins/issues/164>`_)
* Contributors: Alejandro Hernández Cordero

4.0.0 (2024-04-13)
------------------

3.2.0 (2023-05-08)
------------------
* Allow parameters to be reconfigurable (`#144 <https://github.com/ros-perception/image_transport_plugins/issues/144>`_)
* Contributors: Bartosz Meglicki, Kenji Brameld

3.0.0 (2023-04-18)
------------------
* Deprecated the following parameter names in favor of transport scoped ones. The remapping is listed below:
  * `image.format` to `image.compressed.format`
  * `image.png_level` to `image.compressed.png_level`
  * `image.jpeg_quality` to `image.compressed.jpeg_quality`
  * `image.tiff.res_unit` to `image.compressed.tiff.res_unit`
  * `image.tiff.xdpi` to `image.compressed.tiff.xdpi`
  * `image.tiff.ydpi` to `image.compressed.tiff.ydpi`
  The deprecated parameters emit a warning if explicitly set, but this warning will be removed in future distros.
  (`#143 <https://github.com/ros-perception/image_transport_plugins/issues/143>`_)
* Replace deprecated cv_bridge.h with cv_bridge.hpp (`#118 <https://github.com/ros-perception/image_transport_plugins/issues/118>`_)
* Update maintainer (`#112 <https://github.com/ros-perception/image_transport_plugins/issues/112>`_)
* Compressed image transport parameters are now reconfigurable (`#108 <https://github.com/ros-perception/image_transport_plugins/issues/108>`_)
* Contributors: Bartosz Meglicki, Ivan Santiago Paunovic, Kenji Brameld

2.6.0 (2022-08-16)
------------------
* Fix advertiseImpl() in compressed_publisher and subscribeImpl() in compressed_subscriber. (`#106 <https://github.com/ros-perception/image_transport_plugins/issues/106>`_)
* Contributors: Ivan Santiago Paunovic

2.5.0 (2022-04-18)
------------------

2.3.2 (2022-02-18)
------------------
* Add tiff compression support. (`#75 <https://github.com/ros-perception/image_transport_plugins/issues/75>`_)
* Fix copyright year 20012 -> 2012 (`#79 <https://github.com/ros-perception/image_transport_plugins/issues/79>`_)
* JPEG only supports 8 bits images (`#73 <https://github.com/ros-perception/image_transport_plugins/issues/73>`_)
* Contributors: Ivan Santiago Paunovic, Michael Carroll

2.3.1 (2021-07-13)
------------------
* [ros2] Fix RCLCPP\_* logs, a string literal must be the first argument (`#72 <https://github.com/ros-perception/image_transport_plugins/issues/72>`_)
* Contributors: Ivan Santiago Paunovic, Łukasz Mitka

2.3.0 (2020-05-28)
------------------
* Use non-deprecated image_transport headers (`#59 <https://github.com/ros-perception/image_transport_plugins/issues/59>`_)
* Add parameter declarations (`#52 <https://github.com/ros-perception/image_transport_plugins/issues/52>`_)
* Contributors: Michael Carroll, Łukasz Mitka

2.2.1 (2019-10-23)
------------------

2.2.0 (2019-09-27)
------------------

2.1.0 (2019-08-23)
------------------

2.0.0 (2018-12-13)
------------------
* Pointer api updates (`#31 <https://github.com/ros-perception/image_transport_plugins/issues/31>`_)
* Update compressed_image_transport to ros2 (`#26 <https://github.com/ros-perception/image_transport_plugins/issues/26>`_)
* Contributors: Michael Carroll, Jose Luis Rivero

1.9.5 (2016-10-03)
------------------

1.9.4 (2016-10-02)
------------------
* address gcc6 build error and tune
  With gcc6, compiling fails with `stdlib.h: No such file or directory`,
  as including '-isystem /usr/include' breaks with gcc6, cf.,
  https://gcc.gnu.org/bugzilla/show_bug.cgi?id=70129.
  This commit addresses this issue for this package in the same way
  it was addressed in various other ROS packages. A list of related
  commits and pull requests is at:
  https://github.com/ros/rosdistro/issues/12783
  Signed-off-by: Lukas Bulwahn <lukas.bulwahn@oss.bmw-carit.de>
* Contributors: Lukas Bulwahn

1.9.3 (2016-01-17)
------------------
* remove useless tf dependencies
* Using cfg-defined constants
* Changed flag name, and corrected typo in flag use.
* using IMREAD flags.
* Updated for indigo-devel
* Contributors: Cedric Pradalier, Vincent Rabaud

1.9.2 (2015-04-25)
------------------
* get code to compile with OpenCV3
* avoid yet another image copy
* avoid copying data if it can be shared
* Contributors: Vincent Rabaud

1.9.1 (2014-07-18)
------------------

1.9.0 (2014-05-16)
------------------

1.8.21 (2013-06-27)
-------------------
* maintainer: david gossow
* Contributors: David Gossow

1.8.20 (2013-03-18)
-------------------
* 1.8.19 -> 1.8.20
* Contributors: Julius Kammerl

1.8.19 (2013-02-24)
-------------------
* 1.8.18 -> 1.8.19
* Contributors: Julius Kammerl

1.8.18 (2013-02-07 17:59)
-------------------------
* 1.8.17 -> 1.8.18
* fixing input format checks (enabling rgba, bgra) + minor fixes
* Contributors: Julius Kammerl

1.8.17 (2013-01-18)
-------------------
* 1.8.16 -> 1.8.17
* Contributors: Julius Kammerl

1.8.16 (2013-01-17)
-------------------
* 1.8.15 -> 1.8.16
* use the pluginlib script to remove some runtime warnings
* Contributors: Julius Kammerl, Vincent Rabaud

1.8.15 (2012-12-28 20:11)
-------------------------
* fix typo
* Contributors: Vincent Rabaud

1.8.14 (2012-12-28 20:02)
-------------------------
* fix the bad xml naming
* Contributors: Vincent Rabaud

1.8.13 (2012-12-28 19:06)
-------------------------
* fix the bad exports
* make sure the plugins are visible by image_transport
* added license headers to various cpp and h files
* Contributors: Aaron Blasdel, Vincent Rabaud

1.8.12 (2012-12-19 19:30)
-------------------------
* fix downstream stuff in cmake
* Contributors: Dirk Thomas

1.8.11 (2012-12-19 17:17)
-------------------------
* fix cmake order
* Contributors: Dirk Thomas

1.8.10 (2012-12-19 17:03)
-------------------------
* fix dyn reconf
* Contributors: Dirk Thomas

1.8.9 (2012-12-19 00:26)
------------------------
* switching to verion 1.8.9
* fixing dynamic_reconfigure related catkin errors
* Contributors: Julius Kammerl

1.8.8 (2012-12-17)
------------------
* adding build_deb on message_generation & mrun_deb on message_runtime
* Updated package.xml for new buildtool_depend tag for catkin requirement
* Contributors: Julius Kammerl, mirzashah

1.8.7 (2012-12-10 15:29)
------------------------
* adding missing tf build dependency
* Contributors: Julius Kammerl

1.8.6 (2012-12-10 15:08)
------------------------
* switching to version 1.8.6
* Contributors: Julius Kammerl

1.8.5 (2012-12-09)
------------------
* adding missing build debs
* added class_loader_hide_library_symbols macros to CMakeList
* switching to 1.8.5
* fixing compressed color format to comply with opencv api
* Contributors: Julius Kammerl

1.8.4 (2012-11-30)
------------------
* switching to version 1.8.4
* adding plugin.xml exports for pluginlib
* catkinizing theora_image_transport
* github migration from code.ros.org (r40053)
* image_transport_plugins: Updated manifests to have better summaries, correct URLs.
* compressed_image_transport: Some todos.
* compressed_image_transport: Copy connection header to output Image, `#4250 <https://github.com/ros-perception/image_transport_plugins/issues/4250>`_.
* Added Ubuntu platform tags to manifest
* compressed_image_transport: Fixed swapping of R & B channels in data field.
* compressed_image_transport: Fixed bug in lookup of format parameter.
* getParam -> getParamCached
* Switch to opencv2
* compressed_image_transport: Renamed parameters, which are now searched up the parameter tree.
* compressed_image_transport: Updated for compatibility with post-0.1 image_transport.
* image_transport_plugins: Initial stack check-in. Includes theora_image_transport, compressed_image_transport and libtheora. Currently depends on opencv, but may excise this in the future.
* Contributors: Julius Kammerl, gerkey, jamesb, mihelich, pmihelich
