# RPMHalverDuo

**RPMHalverDuo** is designed to control and reduce the RPM of Antminer fans. The device takes a single 4-pin fan connector as input and splits it into two 4-pin connectors, effectively halving the RPM of each output fan. This is particularly useful for applications that require lower noise levels without compromising on airflow.

In typical high-speed fans operating at around 5000-6000 RPM, the noise levels can be quite high. RPMHalverDuo employs this principle by taking a single high-speed fan and splitting its output into two fans operating at lower speeds (e.g., 3000 RPM). This ensures that the air volume is maintained while significantly reducing the noise levels.

## Features
- **RPM Halving**
- **Noise Reduction**
- **PWM Control**
- **Plug and Play**
- **Microcontroller-based**

## How It Works
The device reads the PWM signal from the input fan and generates two new PWM signals at half the duty cycle for the two output fans. This is achieved through a microcontroller, which is programmed to read and manipulate the PWM signals.

## Pin Configuration
A standard 4-pin fan connector has the following pins:
- Ground (GND)
- +12V Power (VCC)
- Tachometer (TACH)
- Pulse Width Modulation (PWM)

## Installation
1. Connect RPMHalverDuo to your high-speed fan's 4-pin connector.
2. Connect the two output 4-pin connectors to your lower-speed fans.
3. Power up and enjoy quieter, yet effective, cooling!

## Roadmap
### Phase 1: Design and Prototyping
- **Design Concept**: Utilize a microcontroller like the ATTiny85 to read and manipulate PWM signals.
- **KiCad Schematic**: Create the schematic in KiCad's Eeschema.
- **KiCad PCB Layout**: Design the PCB layout in KiCad's Pcbnew.
- **Gerber Files**: Generate Gerber files for PCB manufacturing.

### Phase 2: Firmware Development
- **Firmware Design**: Write the firmware to control PWM signals.
- **Testing**: Test the firmware with an oscilloscope and actual fans.
- **Optimization**: Optimize the code for better performance and lower resource usage.

### Phase 3: Testing and Validation
- **Prototype Testing**: Test the manufactured PCB with actual fans.
- **Validation**: Validate that the device effectively halves the RPM and reduces noise.

## Contributing
Feel free to fork this project, open issues, and submit pull requests. Your contributions are welcome!
