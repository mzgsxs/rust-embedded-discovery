# rust-embedded-discovery
code resulted from following rust embedded discovery tutorial
https://docs.rust-embedded.org/discovery/microbit/index.html

## Basic Concepts
Cross compiling - compile in dev machine (x86 etc), generate binary machine code for target machine (arm etc)
JTAG - Joint Test Action Group: for testing, debugging, and programming, operates through a Test Access Port (TAP)

PAC - Peripheral Access Crate: provide direct interface to the peripherals of the chip
HAL - Hardware Abstraction Layer: high-level interface to interact with the hardware SoC
BSC - Board Support Crate: abstract a whole board, provide abstractions to use both the microcontroller as well as the sensors, LEDs etc.

embedded-hal: provide a set of traits that describe behaviour which is usually shared, enables generic/platform agnostic driver (for LEDs, sensors etc)

RTT Real-Time Transfer - debugging protocol, communication between a microcontroller and a host computer over a JTAG or SWD interface. small memory buffer, minimizes CPU overhead.

Serial communication - asynchronous protocol, neither of the shared lines carries a clock signal. allows duplex communication
