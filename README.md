# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;
clear all; % clear screen
close all; % close all figure windows

% INPUT SEQUENCE
a = input('Enter the starting x(n): ');
x = input('Enter the x(n) sequence: ');
n = a:1:length(x) + a - 1;

figure(1);
stem(n, x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

% IMPULSE SEQUENCE
b = input('Enter the starting h(n): ');
y = input('Enter the h(n) sequence: ');
m = b:1:length(y) + b - 1;

figure(2);
stem(m, y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

% LINEAR CONVOLUTION
z = conv(x, y);
n1 = a + b : 1 : length(z) + a + b - 1;

figure(3);
stem(n1, z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```


## OUTPUT:
## linear convolution:
<img width="675" height="521" alt="image" src="https://github.com/user-attachments/assets/2fcc0426-1caa-4c60-850f-fc0135e7cd42" />

## impulse response:
<img width="657" height="520" alt="image" src="https://github.com/user-attachments/assets/88b80b5c-bf0f-47df-88bd-91249e3e1be7" />



## RESULT:
<img width="1919" height="639" alt="image" src="https://github.com/user-attachments/assets/3922e066-d755-4905-b232-59c22f1874e9" />

