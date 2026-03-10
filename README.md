## Experiment No: 3
DIFFERENTIATOR USING OP-AMP (μA741)
## Aim
To design and simulate a Differentiator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the rate of change of input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Capacitor C = 0.01 µF
•	Resistor Rf = 10 kΩ
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram

<img width="1045" height="488" alt="DEFFFF" src="https://github.com/user-attachments/assets/ae858e11-eaa0-42a2-94a1-4a8a4cbc55ab" />

## Connection Details:
•	Input signal → Capacitor (C) → Inverting terminal (Pin 2)
•	Feedback resistor (Rf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
A Differentiator circuit produces an output voltage proportional to the rate of change of input voltage.
## Working Principle:
•	When input changes rapidly → output amplitude increases
•	When input is constant → output is zero
•	Output is inverted
## Procedure
1.	Open Proteus software.
2.	Select μA741, capacitor, resistor, signal generator, and CRO.
3.	Connect circuit in differentiator configuration.
4.	Apply ±15V power supply.
5.	Set input sine wave (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation

| Sl. No | Input Voltage (Vin) | Time Interval | Output Voltage (Vout)           |
| ------ | ------------------- | ------------- | ------------------------------- |
| 1      | +5 V                | 0 – 0.5 ms    | 0 V → –2.5 V (decreasing ramp)  |
| 2      | +5 V                | 0.5 – 1 ms    | –2.5 V → –5 V                   |
| 3      | –5 V                | 1 – 1.5 ms    | –5 V → –2.5 V (increasing ramp) |
| 4      | –5 V                | 1.5 – 2 ms    | –2.5 V → 0 V                    |
| 5      | +5 V                | Next cycle    | Pattern repeats                 |

## Waveforms
•	Sine input → Cosine output (90° phase shift)
•	Square input → Positive & negative spikes
•	Triangular input → Square wave

<img width="1372" height="875" alt="DEFF" src="https://github.com/user-attachments/assets/6dab6116-a75a-45b8-8532-cabce04b5a55" />

## Result
The Differentiator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the rate of change of input voltage.
The circuit behaves as a differentiator.
## Conclusion
•	Output depends on frequency.
•	Output leads input by 90° (for sine input).
•	Higher frequency → Higher output amplitude.
•	Used in wave shaping and signal processing applications.
## Viva Questions
1.	What is a differentiator?

Differentiator: An op-amp circuit whose output is proportional to the rate of change of the input signal.

2.	Write the output equation of differentiator.

Vout​=−RCdtdVi

3.	Why is output leading input?

Why Output Leads Input: Because differentiation produces a signal proportional to slope, causing a 90° phase lead for sinusoidal input.

4.	What happens at very high frequency?

At Very High Frequency: Gain increases excessively and the circuit becomes unstable with noise amplification.

5.	What is practical differentiator?

Practical Differentiator: A modified differentiator with added resistor and capacitor to limit high-frequency gain and improve stability.
