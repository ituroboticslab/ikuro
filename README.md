# ikuro
itu kutuphane projesi navigasyon ve haritalama çalışmaları
itu library project navigation and mapping applications

#How to clone repository into your desktop
mkdir -p ~/husky_desktop_ws/src
cd ~/husky_desktop_ws/src
catkin_init_workspace
cd ~/husky_desktop_ws/
catkin_make
source ~/husky_desktop_ws/devel/setup.bash
echo $ROS_PACKAGE_PATH #to check if the path is included

#clone git repository

cd ~/husky_desktop_ws/src
git init
git remote add origin https://github.com/ituroboticslab/ikuro.git
git fetch
rm -rf CMakeLists.txt #possible duplicate
git checkout -t origin/master
