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
% DHRUV D MEHTA 212223050012


clc; % clear screen

clear all; % clear screen

close all; % close all figure windows


% input sequence

% X[n]={4,−3,2.5,1.5,2 ,5,2,7,−1} h[n]={4,2.5,−4,3.6,−2.5,3,4,5}


a = input("enter the starting x(n)");

x = input("enter the x(n) sequence");

n = a:1:length(x)+a-1;

figure(1);

stem(n,x);

xlabel('time');

ylabel('amplitude');

title('input sequence');


%impulse sequence


b= input('enter the starting h(n)');

y = input('enter the h(n) sequence');

m = b:1:length(y)+b-1;

figure(2);

stem(m,y);

xlabel('time');

ylabel('amplitude');

title('impulse response');


%linear convolution


z = conv(x,y);

n1 = a+b:1:length(z)+a+b-1;

figure(3);

stem(n1,z);

xlabel('time');

ylabel('amplitude');


## OUTPUT:


## RESULT:

