# Raspberry Pi Pico C-SDK Template

## Install Pico C-SDK

- First install dependencies


```bash
sudo apt install cmake g++ gcc-arm-none-eabi doxygen libnewlib-arm-none-eabi git python3
```

- Clone the C-SDK

```bash
git clone --recurse-submodules https://github.com/raspberrypi/pico-sdk.git $HOME/pico-sdk
```

- Configure environment

```bash
echo "export PICO_SDK_PATH=$HOME/pico-sdk" >> ~/.bashrc
source ~/.bashrc
```

## Build

- You need to create a new ``build`` directory in the root folder to build the ``.uf2`` file 

```bash
mkdir build 
cd build 
cmake ..
make
```

- Copy the .uf2 file from the ``build`` directory

```bash
# Ubuntu
cp {project_name}.uf2 /media/$USER/RPI-RP2/
```
