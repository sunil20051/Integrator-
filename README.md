## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Resistor R = 10 kΩ
•	Capacitor Cf = 0.01 µF
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="1159" height="622" alt="image" src="https://github.com/user-attachments/assets/60958460-7aed-430e-ae5c-2baa8d8c64e2" />

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)
•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal
•	Output is inverted
•	Output depends on time
For Sine Wave Input:
•	Output lags input by 90°
•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.

## Tabulation
| S.No | Input Signal              | Frequency | Expected Output                       | Practical Observation                           |
| ---- | ------------------------- | --------- | ------------------------------------- | ----------------------------------------------- |
| 1    | Square Wave               | 100 Hz    | Positive & negative spikes (impulses) | Sharp spikes at rising & falling edges observed |
| 2    | Triangular Wave           | 100 Hz    | Square Wave                           | Square waveform obtained                        |
| 3    | Sine Wave                 | 100 Hz    | Cosine Wave (90° lead)                | Phase-shifted sine (cosine) observed            |
| 4    | Square Wave (higher freq) | 1 kHz     | Higher amplitude spikes               | Narrower and sharper spikes seen                |
| 5    | Sine Wave (higher freq)   | 1 kHz     | Higher amplitude cosine               | Output amplitude increased                      |
## Waveforms
## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.
<img width="1374" height="879" alt="image" src="https://github.com/user-attachments/assets/179512f3-7a13-4e36-879c-c3d400a7cc3d" />
<img width="1378" height="878" alt="image" src="https://github.com/user-attachments/assets/16965897-342d-49bd-8310-91b115fae6d1" />
<img width="1377" height="879" alt="image" src="https://github.com/user-attachments/assets/8281f66b-a594-46fa-bc8e-084e06fe4389" />

## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions
1.	What is an integrator circuit?
2.	Write the output equation of integrator.
3.	Why does output lag input?
4.	What happens at very low frequency?
5.	What is practical integrator?


## Answer
1. An integrator is an op-amp circuit in which the output voltage is proportional to the integral of the input voltage. It uses a resistor at the input and a capacitor in the feedback path.
2. Vout = -(1/RC)(Vin/dt)
3. For a sine wave input, integration converts sine into –cosine, which introduces a –90° phase shift. Therefore, the output lags the input by 90°.
4. At very low frequency, the gain becomes very high. This may cause output saturation and drift due to DC components and offset voltage.
5. A practical integrator is a modified integrator circuit that includes a resistor in parallel with the feedback capacitor to prevent excessive gain at low frequencies and improve stability.
