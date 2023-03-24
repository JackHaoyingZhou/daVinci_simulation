# A framework for  da Vinci simulation

# 1. How to install

## Clone the repository and submodules

Run following command directly in the terminal:

```bash
git clone --recursive https://github.com/JackHaoyingZhou/daVinci_simulation.git
```

## Compile AMBF:

```bash
cd daVinci_simulation/ambf
mkdir build
cd build
cmake ..
make
```

## Make the ROS workspace

```bash
cd ~/daVinci_simulation
catkin_make
```

## source the workspace

```bash
cd ~/daVinci_simulation
source devel/setup.bash
```

Or make the source process automatically runs when starting

```bash
echo "source ~/davinci_simulation/devel/setup.bash" >> ~/.bashrc
```

# 2. How to enable teleoperation devices

## Raze Hydra

```bash
roslaunch razer_hydra hydra.launch
```

## Geomagic Touch

```bash
roslaunch geomagic_control geomagic_headless.launch
```

# To be continued




 

# Reference

Reference of this work:

```bibtex
@article{munawar2022open,
  title={Open Simulation Environment for Learning and Practice of Robot-Assisted Surgical Suturing},
  author={Munawar, Adnan and Wu, Jie Ying and Fischer, Gregory S and Taylor, Russell H and Kazanzides, Peter},
  journal={IEEE Robotics and Automation Letters},
  volume={7},
  number={2},
  pages={3843--3850},
  year={2022},
  publisher={IEEE}
}
```
