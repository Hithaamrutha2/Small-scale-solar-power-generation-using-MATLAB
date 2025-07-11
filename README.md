# Small-scale-solar-power-generation-using-MATLAB
> A MATLAB Simulink-based mini project that models and simulates a small-scale solar power generation system. This project was developed during my 2nd year of ECE to understand solar panel behavior, energy conversion, and basic renewable energy system simulation.

Charging> SOFTWARE SPECIFICATIONS:
1. Software Requirements
Platform: MATLAB Simulink
Toolboxes: Simulink
Circuit diagram ![WhatsApp Image 2025-07-11 at 23 56 56](https://github.com/user-attachments/assets/354c2d76-dedc-44ef-b8e0-138071005e80)
Proposed and existing system -![WhatsApp Image 2025-07-11 at 23 58 55](https://github.com/user-attachments/assets/9d9dce97-3179-4219-9620-bbd22e472138)
Working:
Main Components and Their Roles
1. PV Array:
Constant blocks input irradiance (1500 W/m2) and temperature (25°C). Produces DC power based on solar energy input.
2. DC-DC Converter Stage:
Composed of:IGBT/Diode pair (DC chopper),
Pulse Generator to control the switching,
Series RLC Branches acting as filters/energy transfer elements. Purpose: To boost or regulate the PV output voltage.
3. Battery and Switches:
Battery block is connected via two Ideal Switches.
It allows: from the PV (when excess power is available).
Discharging to load or inverter (when PV output is low).
Goto blocks for voltage, current, and state of charge (SOC) monitor battery output.
4. Voltage Measurements and Scopes:
Several Voltage Measurement blocks were placed at strategic locations to monitor system behavior.
PV output (Scope1) Inverter input (Scope2) Load side (final Scope)
5. Inverter (Universal Bridge):
Converts the DC power from the PV/Battery to AC.
Controlled via a PWM Generator (2-Level).
Output is fed through filter circuit components (Series RLC Branch4 and Branch5) to smooth the AC waveform.
6. Load:
Represented as a resistive load (Series R with RLC Branches). Receives AC power from the inverter.
RESULT
Scope 1 and 2-![WhatsApp Image 2025-07-12 at 00 02 55](https://github.com/user-attachments/assets/7d38614f-d5dd-407e-8d88-2936ef397181)
scope 3-![WhatsApp Image 2025-07-12 at 00 04 16](https://github.com/user-attachments/assets/9dbc6bf0-0c8b-4389-83f4-6efb207e94d6)
Report-[
](https://kaagaz.app/doc/Df7wb207398126CyjWbGm)
Conclusion
Solar power is a key component in the shift from fossil fuels to renewable energy. MATLAB and Simulink provide powerful tools for modeling and simulating solar photovoltaic (PV) systems, including MPPT algorithms, inverters, and energy storage. These tools help researchers and engineers analyze system performance under various environmental conditions.

Simulation in MATLAB/Simulink enables the design and optimization of solar systems for both small- and large-scale applications. By testing different scenarios—like grid integration, temperature, and irradiance variations—users can improve system efficiency and feasibility. As solar power expands in residential and commercial markets, MATLAB/Simulink continues to play a vital role in enhancing system performance and supporting wider adoption.


