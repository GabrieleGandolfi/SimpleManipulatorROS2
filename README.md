# SimpleManipulatorROS2

colcon build --packages-select cyclonedds
[5.442s] WARNING:colcon.colcon_core.package_selection:Some selected packages are already built in one or more underlay workspaces:
	'cyclonedds' is in: /home/unitree/cyclonedds_ws/install/cyclonedds
If a package in a merged underlay workspace is overridden and it installs headers, then all packages in the overlay must sort their include directories by workspace order. Failure to do so may result in build failures or undefined behavior at run time.
If the overridden package is used by another package in any underlay, then the overriding package in the overlay must be API and ABI compatible or undefined behavior at run time may occur.

If you understand the risks and want to override a package anyways, add the following to the command line:
	--allow-overriding cyclonedds

This may be promoted to an error in a future release of colcon-override-check.
Starting >>> cyclonedds
--- stderr: cyclonedds                             
Failed to compile '/home/unitree/unitree_ros2/cyclonedds_ws/src/cyclonedds/src/tools/ddsperf/ddsperf_types.idl'
make[2]: *** [src/tools/ddsperf/CMakeFiles/ddsperf_types_generate.dir/build.make:63: src/tools/ddsperf/ddsperf_types.c] Error 1
make[2]: *** Deleting file 'src/tools/ddsperf/ddsperf_types.c'
make[1]: *** [CMakeFiles/Makefile2:573: src/tools/ddsperf/CMakeFiles/ddsperf_types_generate.dir/all] Error 2
make: *** [Makefile:152: all] Error 2
---
Failed   <<< cyclonedds [1.18s, exited with code 2]

Summary: 0 packages finished [5.30s]
  1 package failed: cyclonedds
  1 package had stderr output: cyclonedds


