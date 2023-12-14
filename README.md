UPDATED for Q4 2023  and Q1 2024

To run in Windows VScode 22 with the newest vers of build tools desktop development with c++
download miniconda 
create a new environment
Install Python version 3.11, nothing newer

update pip

pip install swig 
It is very important to install the gym environment in a set order otherwise it won't work, swig error will happen

pip install gymnasium[classic-control]
pip install gymnasium[mujoco]
pip install gymnasium[atari]
pip install gymnasium[accept-rom-license]
pip install gymnasium[box2d]

pip install tensorflow==2.12.0
pip install keras==2.12.0
pip install keras-rl2

Step 2 (for DQNAgent Model):
Since the keras rl library (keras-rl2) is outdated and not updated anymore, some changed had to be made to the existing library files. In ...site-packages\rl replace the callbacks.py and core.py file with the files in this repo. Same for dqn.py in ...site-packages\rl\agents.
