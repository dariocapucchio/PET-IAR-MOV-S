# PET-IAR-MOV-S
---
Firmware de la placa esclavo del sistema de control de movimiento del Prototipo de Estacion Terrena (PET). Las placas esclavo controlan los motores y envían 

Sistema de posicionamiento para antena de sala de control del IAR. 

## Compilacion 
---
El proyecto utiliza gcc-arm-none-eabi con c/c++ SDK de raspberry pi pico 
Posicionarse con terminal en el directorio

Crear carpeta build
mkdir build 
cd build 
cmake .. 
make 

Crea los archivos binarios dentro de la carpeta build/main/* 
-   *uf2
-   *hex 
-   *elf -> debugger  

## Hardware
---
