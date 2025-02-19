# dma_controller_drivers

## Description
A simple kernel module with a user-space application.

## Project Structure
```
dma_controller_drivers/
├── kernel_module/
│   ├── src/
│   │   └── dma_controller_drivers.c
│   ├── include/
│   │   └── dma_controller_drivers.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd dma_controller_drivers/kernel_module
make
```

### Application
```bash
cd dma_controller_drivers/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod dma_controller_drivers/kernel_module/dma_controller_drivers.ko
# Do something with the module
sudo rmmod dma_controller_drivers
```

### Application
```bash
cd dma_controller_drivers/application
./test_app
```

## License
GPL
