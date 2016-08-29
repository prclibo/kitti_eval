# kitti_eval

`evaluate_object_3d_offline.cpp`evaluates your KITTI detection locally on your own computer using your validation data selected from KITTI training dataset, with the following metrics:

- overlap on image
- overlap on ground-plane
- overlap in 3D
- oriented overlap on image
- oriented overlap on ground-plane
- oriented overlap in 3D

Compile `evaluate_object_3d_offline.cpp` with dependency of Boost and Linux `dirent.h` (You should already have it under most Linux).

Run the evalutaion by:

    ./evaluate_object_3d_offline groundtruth_dir result_dir
    
Note that you don't have to detect over all KITTI training data. The evaluator only evaluates samples whose result files exist.
