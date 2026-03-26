# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
 ```
clear; 
clc; 
close; 
xn = [1 2 3 4 4 3 2 1] 
 
n1=0:1:length(xn)-1; 
subplot(2,2,1); 
plot2d3(n1,xn); 
xlabel('Time n'); 
ylabel('Amplitude'); 
title('Input Sequence');
Xk = fft(xn); 
 
K1=0:1:length(Xk)-1; 
magnitude=abs(Xk) 
subplot(2,2,2); 
plot2d3(K1,magnitude); 
xlabel('frequency(Hz)'); 
ylabel('magnitude(gain)'); 
title('magnitude spectrum'); 
angle = atan(imag(Xk),real(Xk)) 
subplot(2,2,3); 
plot2d3(K1,angle); 
xlabel('frequency(Hz)'); 
ylabel('Phase'); 
title('Phase spectrum') 
y= ifft(Xk) 
 
n2=0:1:length(y)-1; 
subplot(2,2,4) 
plot2d3(n2,y) 
xlabel('Time n'); 
ylabel('Amplitude'); 
title('Inverse FFT OF X(K)');
```
### CALCULATIONS:
![WhatsApp Image 2026-03-26 at 9 00 12 PM](https://github.com/user-attachments/assets/85303c6b-4433-41e3-b466-283b393dde83)

<img width="1080" height="1015" alt="image" src="https://github.com/user-attachments/assets/7f5cbf6e-aa57-4db9-949c-5c84ce19ada6" />




### SAMPLE OUTPUT:

<img width="1080" height="1134" alt="image" src="https://github.com/user-attachments/assets/dbb4ba4c-4951-4aef-bce0-287a3a3d461d" />




## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

