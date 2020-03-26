# Linear Characteristics of ADC using Raspberry Pi

## Abstract 

Our intention is to measure the linear characteristics of an ADC using a Raspberry Pi. The sampling of analog data and subsequent conversion or quantization is performed by the ADC. Quantization is a process where the analog values belonging to a larger set are rounded and mapped to a smaller set ofcountable values. By sampling and quantizing analog voltage data, we can verify if the characteristics between the analog and digital data is indeed linear.

## Introduction
The  aim  in  this  lab  is  to  use  a  Raspberry  Pi  with  ADC to  verify  the  linear  characteristics  of  an  ADC  (MCP3008). The  code  is  written  in  ’Python’  language.  A  potentiometer is  connected  to  vary  voltage  values  between  0  and  3.3V.  A 10-bit ADC is used to sample this analog data. This ADC is SPI-based. Our  board  is  powered  by  a  (5V,  2.5A)  power  supply.  We connect  to  the  Pi  using  an  ethernet  cable.  We  log  into  the Pi using ssh. The compilation and execution of code is done using the serial terminal. In this paper, we will be explaining the design methodology that was taken, the design implementation, and how the testing and verification was done

## TESTING AND VERIFICATION
This  section  deals  with  the  hardware  and  software  testing and verification:

### A.  Hardware Testing
Testing  of  the  hardware  components  and  connections  are done  using  a  multimeter.  When  the  Raspberry  Pi  is  powered correctly the red and green LEDs will turn on.

### B.  Software Testing 
By writing simple GPIO testing programs, we perform input and output testing of GPIO.

### C.  Verification
1)  When the ADC code is run, it displays the voltage values (0 to 3.3V) along with its 10-bit range value (0 to 1023)
2)  The  difference  between  the  actual  and  expected  valuegives us the error
