# TITTLE

      Design and simulate 1:8 De- MUX using Verilog.
# THEORY
      De-multiplexer is also a device with one input and multiple output lines. It is used to send a
signal to one of the many devices. The main difference between a multiplexer and a de-
multiplexer is that a multiplexer takes two or more signals and encodes them on a wire,
whereas a de-multiplexer does reverse to what the multiplexer does.
     In 1 to 8 De-multiplexer, there are total of eight outputs, i.e., Y0, Y1, Y2, Y3, Y4, Y5, Y6, and Y7, 3 selection lines, i.e., S0, S1and S2 and single input, i.e., A. On the basis of the combination of inputs which are present at the selection lines S0, S1 and S2, the input will be connected to one of these outputs. The block diagram and the truth table of the 1×8 de-multiplexer are given below.

### BLOCK DIAGRAM


![block assin 1](https://github.com/pavithra2200891/Design-and-simulate-1-8-De--MUX-using-Verilog./assets/128951583/007c4219-de55-4cf6-9dfa-40c8f8168388)


# LOGIC DIAGRAM

![logic assin 1](https://github.com/pavithra2200891/Design-and-simulate-1-8-De--MUX-using-Verilog./assets/128951583/4651397e-9518-4ee1-8696-8e269d8945c1)



# NETLIST DIAGRAM

![rtl assin 1](https://github.com/pavithra2200891/Design-and-simulate-1-8-De--MUX-using-Verilog./assets/128951583/519ba081-8f0c-4606-b278-a6fe67ccc38e)



# TIMING DIAGRAM

![timming assin 1](https://github.com/pavithra2200891/Design-and-simulate-1-8-De--MUX-using-Verilog./assets/128951583/0afc31e1-b2e9-405e-9259-868a8e64a13e)



# PROGRAM


module demux_1_8(y,s,a);
output reg [7:0]y;
input [2:0]s;
input a;

always @(*)
begin 
y=0;
case(s)
3'd0: y[0]=a;
3'd1: y[1]=a;
3'd2: y[2]=a;
3'd3: y[3]=a;
3'd4: y[4]=a;
3'd5: y[5]=a;
3'd6: y[6]=a;
3'd7: y[7]=a;
endcase
end
endmodule


# REFERENCE

Thus Designed and simulated 1:8 De- MUX using Verilog programming.


