# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS 
![WhatsApp Image 2025-11-25 at 13 16 28_4cad997b](https://github.com/user-attachments/assets/6189a0e3-29b7-44b9-a703-e4111f0eb033)

## HIGH-PASS
![WhatsApp Image 2025-11-25 at 13 17 01_0f692ab8](https://github.com/user-attachments/assets/8cf814c3-08a7-4e44-a236-4e1cb1ca8a87)

## BAND-PASS
![WhatsApp Image 2025-11-25 at 13 17 28_e55cc188](https://github.com/user-attachments/assets/6f20856f-0d59-46da-8b82-7d3212e1974d)


## MODEL GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-25 at 13 18 39_9212b327](https://github.com/user-attachments/assets/20b113d7-4071-4264-82d0-a5f131dbd2df)

## HIGH-PASS
![WhatsApp Image 2025-11-25 at 13 19 05_f35805d3](https://github.com/user-attachments/assets/e91622d6-dca8-4f48-bce2-6e13366eb0bc)

## BAND-PASS
![WhatsApp Image 2025-11-25 at 13 19 43_a566ca6c](https://github.com/user-attachments/assets/44843fef-675f-4fc1-bc16-67a8370febea)


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
![WhatsApp Image 2025-11-25 at 13 23 21_1f1b99b5](https://github.com/user-attachments/assets/ee56c8e4-362f-44d8-be63-9dc6f672fb68)

## HIGH-PASS
![WhatsApp Image 2025-11-25 at 13 23 53_9a17d2ed](https://github.com/user-attachments/assets/31d346a9-31b3-4123-bf03-0f9b096abf43)

## BAND-PASS
![WhatsApp Image 2025-11-25 at 13 24 33_31e17dbe](https://github.com/user-attachments/assets/0741eb00-e61d-47d1-8656-e9aedf33e8b1)


## GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-25 at 13 27 20_02538b2f](https://github.com/user-attachments/assets/63bd802b-2b93-4583-a8c4-7976315fa83c)

## HIGH-PASS
![WhatsApp Image 2025-11-25 at 13 26 37_32f0d67d](https://github.com/user-attachments/assets/9b84c609-d7f5-46fd-96f8-ac07c674c78f)


## BAND-PASS
![WhatsApp Image 2025-11-25 at 13 28 08_ed31b25d](https://github.com/user-attachments/assets/c0956189-ef2f-4c1d-8e22-800562916eb5)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

