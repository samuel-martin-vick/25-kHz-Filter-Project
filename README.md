# 25-kHz-Filter-Project

This circuit receives an external signal that is a any possible combination of 10 kHz, 17 kHz, and 25 kHz. The circuit is designed to detect if the 25 kHz component is present, regardless of whether the other 2 signals are on. If the 25 kHz signal is detected, an LED turns on.

Top View Labeled
![top view with LED on Labeled](https://github.com/user-attachments/assets/356cb7ed-0e37-4d70-a8c7-954709c27c79)


Circuit Diagram
![circuit diagram](https://github.com/user-attachments/assets/b2db1983-35d9-4e49-a37e-026057ff586f)


Frequency Response Analysis
![FRA](https://github.com/user-attachments/assets/df71b86d-91ec-4273-8d8d-4d9226b9c63f)


Setup
<img width="418" alt="setup" src="https://github.com/user-attachments/assets/19e32272-8819-410a-b2c0-19ac09b52fd2" />


Passing a 26 kHz signal
![passing 26 kHz](https://github.com/user-attachments/assets/cf2ac536-5ddf-4122-810b-8196d4f0da8e)


Blocking a 33 kHz signal
![blocking 33 kHz](https://github.com/user-attachments/assets/d8215180-25e9-4721-accc-3f5a045b7bf0)


Blocking a 19 kHz signal
![blocking 19 kHz](https://github.com/user-attachments/assets/5f49e06f-a45e-4bc6-99c8-8be648b468c3)


Block Diagram
(to be added)


Details:

The Infrared System was provided by SPU's Engineering Department. It plugs into wall outlet power. It has 3 infrared emitters that each send a 10 kHz, 17 kHz, or 25 kHz respectively. On the other side, their are 3 IR detectors which receive the signals. The signals are then combined into one output wire. Each signal was about 3 V peak to peak, so if all 3 switches were turned on, then the total signal would be about 9 V peak to peak.

First the circuit uses a bandpass filter centered on 25 kHz to block out the 17 kHz and 10 kHz signals. Then it has a peak detector which converts the AC signal to DC. Then a comparator detects if the output voltage of the peak detector is above a certain threshold (~0.8 V), it will output +5V. Which will then turn on the LED.

