Notes:

When running make -j, if the error fatal error: "Eigen/Dense: No such file or directory" occurs, run the following commands

cd /usr/local/include
sudo ln -sf eigen3/Eigen Eigen

after running make -j, the command:
sudo make install
MUST be run

Must modify path in ros_eigen_params.cfg
additionally, the following files have absolute paths that need updating:
gpd/include/gpd/net/dense_layer.h
gpd/include/gpd/util/eigen_utils.h
gpd/include/gpd/candidate/local_frame.h
gpd/include/gpd/net/conv_layer.h
gpd/include/gpd/candidate/finger_hand.h
gpd/include/gpd/util/point_list.h
gpd/include/gpd/util/cloud.h
gpd/include/gpd/net/layer.h
gpd/include/gpd/net/layer.h
gpd/include/gpd/candidate/hand.h
gpd/include/gpd/candidate/antipodal.h