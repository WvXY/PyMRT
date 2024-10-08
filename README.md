# WvXY's Python Toolbox(WIP)

## Description

A tiny Python toolbox using ModernGL and PyTorch, 
designed for prototyping and testing for my research project.

It derived from my master research project.
It is currently under development and not ready for use.
I will add more functions as my project progresses.

## Structure

It is divided into several modules:

- **Geometry**: contains the game object and primitives
- **Physics**: contains the physics classes
- **Rendering**: contains the rendering classes
- **Utils**: contains the utility classes

## Installation

##### PIP: Windows

```zsh
python3 -m venv venv
./venv/Scripts/activate.bat
pip install -r requirements.txt
pip install -e .
```

##### PIP: Linux

```zsh
python3 -m venv venv
bash ./venv/bin/activate
pip install -r requirements.txt
pip install -e .
```

##### Conda environment (recommended)

Install [miniconda](https://docs.conda.io/en/latest/miniconda.html) first.

```zsh
conda create -n wtbxCenv python=3.12 numpy scipy matplotlib
conda activate wtbxCenv
pip install del-msh imgui moderngl moderngl-window pygmsh
conda install pytorch torchvision torchaudio pytorch-cuda>=12.1 -c pytorch -c nvidia
conda install conda-forge::pygalmesh 
pip install -e .
```

#### (Optional)Add and init as submodule

```zsh
git clone git@github.com:WvXY/WvXY_ToolboxPy.git
git submodule init
git submodule update
```

## Problems

- [ ] Particles are not properly rendered


## TODO

- [ ] Rename class and submodule names to be more consistent
- [ ] Use only PyTorch & reduce dependencies
- [ ] Entity Component System
- [ ] Physics Engine

## Black Formatting

I used the following options to format the code using black

```
--line-length=80 --preview
```

## References

- https://youtu.be/Y9U9IE0gVHA?si=kwfcpUtY0MACyFwI
- https://github.com/jrouwe/JoltPhysics/tree/master/Jolt
