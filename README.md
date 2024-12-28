# T-FLIPFLOP-POSEDGE

**AIM:**

To implement  T flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**T Flip-Flop**

T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/458a68fe-2d08-4a9d-ac4f-7ae0480ce0bd)

 
This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/cdd7fb32-539f-4b66-bb8d-f305a153c886)

 
From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

**Procedure**

1. Start a New Project in Quartus:

  • Open Quartus Prime and create a new project.
  
  • Define the project name and directory location.
  
2. Write the Verilog Code for the T Flip-Flop:

  • Implement the T flip-flop behavior using the XOR logic based on the characteristic equation.

3. Compile and Simulate:

  • Compile the design and run the simulation in Quartus.
  
  • Observe the output waveform to verify the functionality of the T flip-flop.
  
4. Analyze the Results:

  • Ensure that the output Q toggles on each clock pulse when T = 1, and holds its state when T = 0.

**PROGRAM**

![t_flipflop_code](https://github.com/user-attachments/assets/774fbe8e-8f1f-460e-83a8-e84dad6f5424)


**RTL LOGIC FOR FLIPFLOPS**

![t_flipflop_rtl](https://github.com/user-attachments/assets/50d6cfa0-5e37-4722-b9fc-0a27f34501c1)


**TIMING DIGRAMS FOR FLIP FLOPS**

![t_flipflop_waveform](https://github.com/user-attachments/assets/f64d18b4-e160-4967-b6cf-32cff0c420fa)


**RESULTS**

• The Verilog code for the T flip-flop works correctly according to the truth table.

• The simulation results match the expected behavior of the T flip-flop.

• The output waveform from the simulation shows that Q toggles on each positive clock edge when T = 1, and holds the value when T = 0.

• The functionality of the T flip-flop is validated using the simulation and timing diagram.
