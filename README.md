# Arm Debugger

## Overview

The complete [documentation](https://developer.arm.com/documentation/108029/latest/Extension-pack-and-extensions) for Arm® Debugger and the other Keil® Studio extensions is available on Arm Developer.

The Arm Debugger extension provides access to the Arm Debugger engine for Visual Studio Code by implementing the [Microsoft Debug Adapter Protocol (DAP)](https://microsoft.github.io/debug-adapter-protocol//). The Arm Debugger engine supports connections to physical and virtual targets:

- Physical targets. Either through external debug probes such as the Arm's ULINK™ family of debug probes, or through on-board low-cost debugging such as ST-Link or CMSIS-DAP based debug probes.
- Virtual targets. Using Fixed Virtual Platform models (FVPs).

We recommend installing the [Keil Studio Pack](https://marketplace.visualstudio.com/items?itemName=Arm.keil-studio-pack) for Visual Studio Code Desktop to quickly set up your environment. You can then [import a csolution example from keil.arm.com](https://developer.arm.com/documentation/108029/latest/Get-started-with-an-example-project/Import-a-csolution-example), [download and convert a μVision project from keil.arm.com](https://developer.arm.com/documentation/108029/latest/Get-started-with-an-example-project/Download-and-convert-a-Keil--Vision-example), [create a csolution project from scratch](https://developer.arm.com/documentation/108029/latest/Arm-CMSIS-csolution-extension/Create-a-csolution-project), or [convert an existing μVision project](https://developer.arm.com/documentation/108029/latest/Arm-CMSIS-csolution-extension/Convert-a-Keil--Vision-project-to-a-csolution-project).

The Arm Debugger extension works with the Arm CMSIS csolution (Identifier: `arm.cmsis-csolution`), the Arm Device Manager (Identifier: `arm.device-manager`), and the Arm Virtual Hardware (Identifier: `arm.virtual-hardware`) extensions.

## Supported features

The Arm Debugger extension allows you to:

- Load images (for example, .elf, .axf, or .bin files) and debug information as per the DWARF Debugging Information Format Standard, up to and including version 5
- Run images
- Set breakpoints
- Do source and instruction stepping
- Access variables and registers
- View the content of memory
- Debug FVPs
- Access the [CLI](https://developer.arm.com/documentation/101471/2023-0/Arm-Debugger-commands) using the Debug Console

## Debug configuration support

The Arm Debugger engine supports debug connections based on:

- The [debug setup with CMSIS-Pack](https://open-cmsis-pack.github.io/Open-CMSIS-Pack-Spec/main/html/coresight_setup.html)
- The integrated [configuration database (configdb)](https://developer.arm.com/documentation/101470/2023-0/DTSL/Arm-Development-Studio-configuration-database)

## Supported architectures and processors

- Armv6-M architecture

  Cortex®-M0, Cortex-M0+, Cortex-M1, Arm SecurCore® SC000

- Armv7-M architecture

  Cortex-M3, Cortex-M4, Cortex-M7, Arm SecurCore SC300

- Armv8-M architecture

  Cortex-M23, Cortex-M33, Cortex-M35P

- Armv8.1-M architecture

  Cortex-M55, Cortex-M85

## Supported debug probes

- [Arm ULINK family](https://www.arm.com/products/development-tools/debug-probes/ulink)
- ST-LINK from STMicroelectronics
- Probes based on the [CMSIS-DAP](https://arm-software.github.io/CMSIS_5/latest/DAP/html/index.html) debug adapter protocol v1.x and v2.x

## Limitations

Some capabilities of the Arm Debugger engine that are not yet exposed in Visual Studio Code include:

- CoreSight™ trace
- Symmetric and asymmetric multicore debug
- RTOS awareness

## Use the Arm Debugger extension

See the [documentation](https://developer.arm.com/documentation/108029/latest/Arm-Debugger-extension) for the Arm Debugger extension to run a project on your hardware and start a debug session.

## Submit feedback

To submit feedback on the Arm Debugger extension preview version, please [open a bug report or a feature request](https://github.com/Arm-Software/vscode-arm-debugger/issues/new/choose).
