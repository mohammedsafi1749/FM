EXP NO : 4 GENERATION AND DETECTION OF FM

AIM:

To write a program for Frequency Modulation and Demodulation using SCILAB and to observe
and measure the frequency deviation and the modulation index of FM.

EQUIPMENTS REQUIRED

 Computer with i3 Processor

 SCI LAB

THEORY:

Frequency modulation is a type of modulation in which the frequency of the high frequency
(carrier) is varied in accordance with the instantaneous value of the modulating signal.
FREQUENCY DEVIATION f and MODULATION INDEX m f :
The frequency deviation f represents the maximum shift between the modulatedsignal
frequency, over and under the frequency of the carrier

We define modulation index m f the ratio between f and the modulating frequency
m= f / fm

FREQUENCY MODULATION GENERATION:

The circuits used to generate a frequency modulation must vary the frequency of a high
frequency signal (carrier) as function of the amplitude of a low frequency signal (modulating signal). In
practice there are two main methods used to generate FM.

Algorithm:

1. Define Parameters:
 Fs: Sampling frequency.
 T: Duration of the signal.
 Fc: Carrier frequency.
 Fm: Frequency of the modulating signal.
 Beta: Modulation index, which controls the extent of frequency deviation.
3. Generate Signals:
 modulating_signal: Sinusoidal signal used for modulation.
 carrier_signal: The high-frequency carrier signal.
 modulated_signal: FM modulated signal calculated by varying the carrier frequency according
to the modulating signal.
4. FM Modulation:
 Modulated_signal is obtained by modulating the carrier signal with the modulating signal.
5. FM Demodulation:
 Differentiation: Computes the derivative of the modulated signal to extract frequency
variations.
 Envelope Detection: Takes the absolute value to retrieve the envelope of the signal.
 Low-pass Filtering: Applies a Butterworth low-pass filter to smooth the envelope and recover
the original modulating signal.
6. Visualization:
 Plots the modulating signal, carrier signal, FM modulated signal, and demodulated signal for
analysis.

PROCEDURE

 Refer Algorithms and write code for the experiment.
 Open SCILAB in System
 Type your code in New Editor
 Save the file
 Execute the code
 If anyError, correct it in code and execute again

MODEL GRAPH:
<img width="1312" height="700" alt="image" src="https://github.com/user-attachments/assets/0f081bdf-408f-424f-bf45-7587e918fc64" />

Program:

Am=20.6;
fm=424;
Ac=41.2;
fc=4240;
fs=42400;
t=0:1/fs:2/fm;
m=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,m);
c=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,c);
b=5.4;
s=Ac*cos((2*3.14*fc*t)+b*sin(2*3.14*fm*t));
subplot(3,1,3);
plot(t,s);

OUTPUT WAVEFORM:

![WhatsApp Image 2025-08-28 at 09 36 30_686cdfa5](https://github.com/user-attachments/assets/1ef484ac-0aa5-4df8-ba7a-dc7286d53471)

TABULATION:

![WhatsApp Image 2025-08-28 at 09 37 52_2bc138a4](https://github.com/user-attachments/assets/b74d703d-ef5e-4671-8a04-03414c995748)

RESULT:

Thus the frequency modulation and demodulation is successfully done and the output is
experimentally verified.
