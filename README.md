# Analog VLSI Project: Analog-to-Digital Converter (ADC) and Digital Components

This project focuses on the design and simulation of an **Analog-to-Digital Converter (ADC)** in VLSI using CMOS technology, alongside digital components such as priority encoders, frequency dividers, and D-Flip-Flops. The project was built and tested through a series of simulations to ensure accurate digital conversion and timing.

## Project Overview

The main goal of this project is to design an ADC that converts analog signals to digital form for processing, and to integrate this with digital circuits for encoding and signal management. The components were designed using standard CMOS technology and were simulated using industry-standard tools.

### Key Components:

1. **Analog-to-Digital Converter (ADC)**: Converts analog input signals into digital output. It uses a chain of comparator amplifiers and resistors to sample the input signal and output a digital value based on the signal's magnitude.
2. **Priority Encoder**: Selects the most significant active bit from the ADC output and encodes it into a smaller binary number.
3. **Clock Generator**: Provides clock signals to synchronize the operations of the digital components.
4. **Frequency Divider**: Reduces the frequency of the clock signal, creating multiple lower frequency signals for different components.
5. **D-Flip-Flop**: Stores data and ensures that outputs remain stable during clock transitions.
6. **Inverter**: Performs logic inversion on signals.
7. **Decoder**: Converts binary values into corresponding signals to activate different parts of the system.


### Components Details

#### 1. Analog-to-Digital Converter (ADC)

The ADC converts the input analog signal into a digital output. It is built with a chain of resistors and comparators to compare the input voltage with reference voltages and output a corresponding binary value. The output is determined by the most significant bit (MSB) that is active, ensuring accurate digital representation.

- **Input Voltage (Vin)**: Analog signal.
- **Output**: Binary representation of the input voltage.

#### 2. Priority Encoder

The priority encoder compresses the large number of input bits from the ADC into a smaller binary number. It ensures that only the most significant bit is active when multiple inputs are high.

#### 3. Clock Generator

The clock generator is built from a series of inverters and produces a stable oscillating clock signal. The clock signal is essential for synchronizing the digital components of the system.

#### 4. Frequency Divider

The frequency divider reduces the frequency of the clock signal, providing a slower clock for components that require lower frequencies to function properly.

- **Input Frequency**: High-frequency clock signal.
- **Output Frequency**: Divided clock signal, typically a factor of 2.

#### 5. D-Flip-Flop

The D-Flip-Flop is a memory element used to store one bit of data. It captures the input at the rising edge of the clock signal and holds it until the next rising edge. This ensures stable data flow within the system.

#### 6. Inverter

The inverter is a simple CMOS logic gate that outputs the opposite logic level of its input.

#### 7. Decoder

The decoder is responsible for activating specific parts of the system based on a binary input. It takes a binary value and converts it into one-hot output signals.

### Simulations and Results

All components were tested using simulation tools. Below are some highlights of the results:

- **ADC Simulation**: The ADC successfully converted the input analog signals into digital binary outputs. The output graph showed the expected binary progression as the input voltage increased.
- **Priority Encoder**: Simulated to ensure that the encoder outputs the correct binary value based on the highest-priority input.
- **Clock and Frequency Divider**: Simulations showed that the clock generator and frequency divider produced stable clock signals with the desired frequencies.
- **D-Flip-Flop**: The D-Flip-Flop was tested to ensure it holds data correctly and responds to clock edges.

### File Descriptions

- `docs/Analog_VLSI_ADC_Project_Summary.pdf`: Detailed documentation of the project, including schematics, layout designs, and simulation results.
  
### How to Run the Project

1. **Setup**: Ensure the design files are opened in the appropriate VLSI design tools (e.g., Cadence).
2. **Simulate**: Run simulations for each component to observe their behavior under different input conditions.
3. **Analyze**: Compare the simulation outputs to the expected results described in the project summary.

## Conclusion

The Analog-to-Digital Converter (ADC) and supporting digital components were successfully designed and simulated in this project. The ADC accurately converts analog inputs to digital signals, and the system demonstrates proper signal management using priority encoding, clock generation, and frequency division. This project illustrates the effective integration of analog and digital VLSI design principles.

---

© 2023 Daniel Ram. Licensed under the MIT License.
