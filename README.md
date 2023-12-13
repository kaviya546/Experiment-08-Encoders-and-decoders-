# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.

Developed by: KAVIYA SNEKA M

RegisterNumber:  23003642

Code:

Decoder:

![DECODER CODE](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/31d30a22-1773-416c-b451-b6e62b3e1dac)

Encoder:

![ENCODER CODE](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/b476b390-3815-4378-b83c-92671c91191c)

RTL Diagram:

Decoder:

![DECODER LOGIC](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/3105358d-55db-47c2-b4e6-acc5b961dcb0)

Encoder:

![ENCODER LOGIC](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/ff26958d-19ac-499d-b0d6-00f9ab977708)

Truth table:

Decoder:

![DECODER T](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/7b366f26-e197-494e-8151-f14e31fa8e52)

Encoder:

![ENCODER TT](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/02d646db-8796-4316-b410-0fb64b73d4b4)


Output:

Decoder:

![DECODER TIME](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/1291ea27-eaa7-4130-9754-d83e9b154f65)

Encoder:

![ENCODER TIME](https://github.com/kaviya546/Experiment-08-Encoders-and-decoders-/assets/150368823/9cf0cc69-10df-4cb8-a13f-048c57d50b8b)



### RESULTS 

Thus the program to desing encoder and decoder is done
