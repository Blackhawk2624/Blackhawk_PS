# Installation Instructions

### Installing Ardupilot and MAVProxy Ubuntu 20.04

### Video Tutorial at https://youtu.be/1FpJvUVPxL0

### Clone ArduPilot

In home directory:
```
cd ~
sudo apt install git
git clone https://github.com/ArduPilot/ardupilot.git
cd ardupilot
```

### Install dependencies:
```
cd ardupilot
Tools/environment_install/install-prereqs-ubuntu.sh -y
```

reload profile
```
. ~/.profile
```

### Checkout Latest Copter Build
```
git checkout Copter-4.2
git submodule update --init --recursive
```

Run SITL (Software In The Loop) once to set params:
```
cd ~/ardupilot/ArduCopter
sim_vehicle.py -w
```
