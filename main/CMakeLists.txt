cmake_minimum_required(VERSION 3.13)

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)
add_executable(main 
    main.c 
)

target_link_libraries( main 
                       quadrature_encoders 
                       pwm_control 
                       pid_digital
                       pico_stdlib
                       pico_multicore
                       i2c_slave
                       limit_switch)

pico_enable_stdio_usb(main 1) 
#pico_enable_stdio_uart(main 0) 
# pull in common dependencies
pico_add_extra_outputs(main)