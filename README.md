# 25-kHz-Filter-Project


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

Top View
![top view with LED on](https://github.com/user-attachments/assets/39bcac05-425d-424f-8038-6a3b36af3959)

Top View Labeled

Circuit Diagram

Block Diagram


Details:

The Infrared System was provided by SPU's Engineering Department. It plugs into wall outlet power. It has 3 infrared emitters that each send a 10 kHz, 17 kHz, or 25 kHz respectively. On the other side, their are 3 IR detectors which receive the signals. The signals are then combined into one output wire. Each signal was about 3 V peak to peak, so if all 3 switches were turned on, then the total signal would be about 9 V peak to peak.

My circuit's goal was to turn on an LED if the 25 kHz signal was present, regardless of whether the other 2 signals were on.

First the circuit uses a bandpass filter centered on 25 kHz to block out the 17 kHz and 10 kHz signals. Then it has a peak detector which converts the ...

