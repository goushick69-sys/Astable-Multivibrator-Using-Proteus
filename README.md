## Experiment No: 5
ASTABLE MULTIVIBRATOR USING 555 TIMER Using Proteus
## Aim
To design and simulate an Astable Multivibrator using NE555 in Proteus Design Suite and observe the continuous square wave output.
## Apparatus Required
<img width="463" height="214" alt="image" src="https://github.com/user-attachments/assets/ace629d7-ba57-4e27-b821-02a87554de13" />

## Circuit Diagram
Pin Configuration of 555 Timer:
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/3b165290-27bb-41ee-a27a-2f638f87e297" />

•	Pin 1 → Ground
•	Pin 2 → Trigger
•	Pin 3 → Output
•	Pin 4 → Reset (Connected to Vcc)
•	Pin 5 → Control Voltage (Bypass with 0.01 µF capacitor optional)
•	Pin 6 → Threshold
•	Pin 7 → Discharge
•	Pin 8 → Vcc
## Connections:
•	R1 → Between Vcc and Pin 7
•	R2 → Between Pin 7 and Pins 2 & 6
•	C → Between Pins 2 & 6 and Ground
•	Output → Pin 3
## Theory
•	The NE555 timer is a widely used integrated circuit for generating precise time delays and oscillations. When operated in astable mode, it functions as a free-running oscillator that continuously produces a square wave without any external triggering signal. In this mode, a capacitor connected to the circuit charges through resistors R1 and R2 and discharges through R2 repeatedly. The internal voltage divider of the 555 timer creates two reference levels at 1/3 Vcc and 2/3 Vcc. 
•	When the capacitor voltage reaches 2/3 Vcc, the upper comparator resets the flip-flop and turns ON the discharge transistor, causing the capacitor to discharge. When the voltage falls to 1/3 Vcc, the lower comparator sets the flip-flop, turning OFF the discharge transistor and allowing the capacitor to charge again. This continuous charging and discharging process generates a square wave at the output (Pin 3) and an exponential waveform across the capacitor. The time period of oscillation is given by T=0.693(R1+2R2)CT = 0.693 (R1 + 2R2) CT=0.693(R1+2R2)C, and the frequency depends on the values of R1, R2, and C. Thus, the 555 timer in astable mode acts as a simple and reliable square wave generator used in clock circuits, LED flashers, and pulse generation applications.
## Procedure
1.	Open Proteus software.
2.	Select NE555 IC, resistors, capacitor, and CRO.
3.	Connect circuit in astable configuration.
4.	Apply 5V supply.
5.	Run simulation.
6.	Observe square wave output at Pin 3.
7.	Measure time period and frequency.
## Tabulation
<img width="675" height="60" alt="image" src="https://github.com/user-attachments/assets/9f78a57e-c36a-4bf7-a9f6-379e1323130e" />

## Waveforms
<img width="1380" height="881" alt="image" src="https://github.com/user-attachments/assets/fdae6332-21c3-4378-9ed2-607c447dfab1" />

•	Output (Pin 3) → Square wave
•	Capacitor voltage → Exponential charging & discharging waveform
## Result
The Astable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.
A continuous square wave output was obtained.
The practical frequency closely matches the theoretical frequency.
## Conclusion
•	The 555 timer works as a free-running oscillator in astable mode.

•	Frequency depends on R1, R2, and C values.

•	Increasing R or C decreases frequency.

•	Used in clock generation, LED flashing, and tone generation.

## Viva Questions
1. What are the operating modes of 555 timer?

The 555 timer operates in three modes: monostable, astable, and bistable mode. These modes are used for one-shot pulse, continuous oscillation, and flip-flop operation.

2. What are the threshold levels in astable mode?

In astable mode, the capacitor voltage varies between 1/3 Vcc and 2/3 Vcc. These levels control the charging and discharging of the capacitor.

3. Write the frequency formula.

The frequency of astable multivibrator is given by f = 1.44 / ((R1 + 2R2)C). It depends on resistor and capacitor values.

4. What is duty cycle?

Duty cycle is the percentage of time the output remains HIGH in one cycle. It indicates the ratio of ON time to total time.

5. What happens if R2 increases?

If R2 increases, the charging and discharging time increases. So the frequency decreases and time period increases.
