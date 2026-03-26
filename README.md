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
10 
 
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
![WhatsApp Image 2026-03-26 at 9 00 12 PM](https://github.com/user-attachments/assets/a610be14-745c-4396-9bdd-3477a4475575)

![WhatsApp Image 2026-03-26 at 9 00 34 PM](https://github.com/user-attachments/assets/b43db399-4277-4b67-9144-148b2b70a2a2)


### SAMPLE OUTPUT:
![WhatsApp Image 2026-03-26 at 9 37 50 PM](https://github.com/user-attachments/assets/e53d9d86-a308-40c3-8cfb-d8e2b529dc21)




## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

