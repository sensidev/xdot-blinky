cmake_minimum_required(VERSION 3.6)
project(xdot_blinky)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
    main.cpp)

include_directories(
        ISL29011
        mbed-os
        mbed-os/cmsis
        mbed-os/cmsis/TOOLCHAIN_GCC
        mbed-os/docs
        mbed-os/drivers
        mbed-os/events
        mbed-os/events/equeue
        mbed-os/features
        mbed-os/features/frameworks
        mbed-os/features/frameworks/greentea-client
        mbed-os/features/frameworks/greentea-client/greentea-client
        mbed-os/features/frameworks/greentea-client/source
        mbed-os/features/frameworks/unity
        mbed-os/features/frameworks/unity/source
        mbed-os/features/frameworks/unity/unity
        mbed-os/features/frameworks/utest
        mbed-os/features/frameworks/utest/source
        mbed-os/features/frameworks/utest/utest
        mbed-os/features/mbedtls
        mbed-os/features/mbedtls/importer
        mbed-os/features/mbedtls/inc
        mbed-os/features/mbedtls/inc/mbedtls
        mbed-os/features/mbedtls/platform
        mbed-os/features/mbedtls/platform/inc
        mbed-os/features/mbedtls/platform/src
        mbed-os/features/mbedtls/src
        mbed-os/features/nanostack
        mbed-os/features/netsocket
        mbed-os/features/storage
        mbed-os/hal
        mbed-os/hal/hal
        mbed-os/hal/storage_abstraction
        mbed-os/platform
        mbed-os/rtos
        mbed-os/rtos/rtx
        mbed-os/rtos/rtx/TARGET_CORTEX_M
        mbed-os/rtos/rtx/TARGET_CORTEX_M/TARGET_M3
        mbed-os/rtos/rtx/TARGET_CORTEX_M/TARGET_M3/TOOLCHAIN_GCC
        mbed-os/targets
        mbed-os/targets/TARGET_STM
        mbed-os/targets/TARGET_STM/TARGET_STM32L1
        mbed-os/targets/TARGET_STM/TARGET_STM32L1/TARGET_XDOT_L151CC
        mbed-os/targets/TARGET_STM/TARGET_STM32L1/TARGET_XDOT_L151CC/device
        mbed-os/targets/TARGET_STM/TARGET_STM32L1/TARGET_XDOT_L151CC/device/TOOLCHAIN_GCC_ARM
        mbed-os/targets/TARGET_STM/TARGET_STM32L1/device
)

add_executable(xdot_blinky ${SOURCE_FILES})