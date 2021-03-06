# Extended Kalman Filter
## Adapted and built for the Self-Driving Car Engineer Nanodegree Program

This is an implementation of an extended kalman filter for object tracking.
The extension refers to the ability to fuse radar and lidar sensory input.

Radar relays sensory input as polar coordinates as opposed to cartesian. This measurement is non-linear, and requires a linearisation step.
This presents itself as a Taylor Series approximation.

The algorithm was tested on a Unity-based 2D car simulator, and compared against the ground truth using RMSE.

![result](data/final_result.png)

The algorithm with optimised noise achieves an RMSE as shown in diagram.

---

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make` 
   * On windows, you may need to run: `cmake .. -G "Unix Makefiles" && make`
4. Run it: `./ExtendedKF path/to/input.txt path/to/output.txt`. You can find
   some sample inputs in 'data/'.
    - eg. `./ExtendedKF`
