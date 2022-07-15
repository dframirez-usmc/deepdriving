# deepdriving
AI and ML techniques applied to the KITTI automotive dataset!
This is mostly demonstrations of different computer vision and deep learning techniques for Visual-SLAM, 3D Reconstruction, and Pointclouds.

![alt text](https://github.com/dframirez-usmc/deepdriving/blob/main/projection.gif?raw=true)

[As described in the MonoReq repo...](https://github.com/Brummi/MonoRec#kitti-odometry)

Run the code below to move `data_depth_annotated.zip` files into the sequence directories:

    python preprocess_kitti_extract_annotated_depth.py \
    --output ~/KITTI/dataset/ \
    --input ~/KITTI/data_depth_annotated.zip \
    --depth_folder image_depth_annotated


KITTI Odometry Dataset is expected in the user home of your filesystem:

    ~/KITTI/dataset/poses/
                   /sequences/00/image_0/
                                /image_1/
                                /image_2/
                                /image_3/
                                /image_depth_annotated/
                                /velodyne/
                             /01/
                             /02/
                             /...
                             /21/
