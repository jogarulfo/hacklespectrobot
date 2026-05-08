# SHakeItUp
A robot that shake things and guess the content of a container.

Built during the 2026 robotic hackathon of Unaite x GoSIM.

## Installation

1. Clone the repository:

```bash
git clone --recursive https://github.com/jogarulfo/ShakeItUp.git
```

2. Install dependencies:

```bash
uv pip install -e .
cd lespectrobot
uv pip install -e .[feetech] 
```

Use "feetech" for the SO101 and "damiao" for the OpenARM.

## Usage :

The install.md file is a step by step of all the main command used during the hackaton to teleoperate, record and train the OpenArm with a OpenArm_mini as the leader.

The goal is to have a sensor on the jaw that cna get vibration data and use it to guess the content of the container. The experience have been made with a dragonfly sensor, and all the acquisition with a DAQ Dewesoft. It use the openDAQ library so you are free to modify the acqusition code to match your own setup.

The goal is to have a sensor on the jaw that can get vibration data and use them to guess the content of the container. The experience have been made with a dragonfly sensor, and all the acquisition with a DAQ Dewesoft. It use the openDAQ library so you are free to modify the acqusition code to match your own setup.

The main code of the acquisition is in the submodule lespectrobot/src/lerobot/robots   and the code is ready to use for the robot SO101 and OpenARM ( for the BiopenArm, just replace whatever of the two OpenArm by a OpenFollowerDragonTacile Arm in the file bi_openarm_follower.py ).