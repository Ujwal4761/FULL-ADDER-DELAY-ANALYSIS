PART I: (55 Points) STANDARD CELL BASED FULL ADDER DESIGN
1. (5 Points) Restore the given FA_p1 schematic by designing a full adder (FA) using standard cells from GSCLIB045.
 <img width="1008" height="538" alt="image" src="https://github.com/user-attachments/assets/0470672a-db15-4580-ab38-b87a82b45744" />

2. (5 Points) Create a maestro cell view for the testbench provided. (In this part only cover the (A1, B1, Ci1) signal set. Verify the logical correctness of your FA through functional simulation
Testbench
<img width="1003" height="487" alt="image" src="https://github.com/user-attachments/assets/ce6bfa16-5ddf-4151-9c4b-c6013dee703f" />

the waveform shows the correct functionality
<img width="970" height="577" alt="image" src="https://github.com/user-attachments/assets/daeb889b-51c7-413e-98c6-b516e728b9ef" />

it has been verified with the truth table of Full adder
  
it gives the output exactly as the truth table 
<img width="898" height="855" alt="image" src="https://github.com/user-attachments/assets/aa0f8d70-5309-4142-a9da-13980386bca9" />
<img width="1030" height="534" alt="image" src="https://github.com/user-attachments/assets/55b63cf3-9892-4c29-9eef-c87ec7ef01b5" />


4. Question: What is the minimum steps that you need to cover all 32 vectors? Do your simulation with minimum steps. (Bonus: +5 points)

step1: we need to set trans analysis to 33ns
step2: VDD and VSS values need to be fed from stimuli
step3:select the output pins from design
step4:upload the desired vector file
step 5:run the simulation and view the result in waveform

Area calculation and pin placement estimation
<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/1b40cb35-3056-4209-95f9-758b2ad571da" />
  
layout  
<img width="1031" height="435" alt="image" src="https://github.com/user-attachments/assets/6da9b2b1-99d6-47a8-aaa4-db1340dfa0e7" />

No DRC errors reported
 <img width="1002" height="741" alt="image" src="https://github.com/user-attachments/assets/f48e98f4-c915-4fc8-9178-f0c1447efd75" />

LVS is also clean
 <img width="1013" height="572" alt="image" src="https://github.com/user-attachments/assets/77fc84c5-298f-4715-b9d4-a865af214444" />


PART II: (55 Points) TRANSISTOR-LEVEL MIRRORED STRUCTURE
1. (5 Points) Restore the given FA_p2 cell by designing a full adder (FA) using mirrored design from Figure 1. Please follow the sizing values in the figure by referencing the standard library inverter (with [1, 1.5] sizing).
<img width="940" height="480" alt="image" src="https://github.com/user-attachments/assets/24c47407-e9d2-424e-8960-6bfc5e07e491" />
 
Note: - PMOS is 390nm,NMOS is 260nm, but the one at the extreme left are 
PMOS= 390nm x 6, NMOS = 260nm x 4

functionality and the symbol has been created successfully 
<img width="979" height="503" alt="image" src="https://github.com/user-attachments/assets/a1d676fc-1627-479f-8a3c-8716df94fd40" />

also the testbench has been created for both the parts
<img width="1020" height="556" alt="image" src="https://github.com/user-attachments/assets/3ae75f51-2059-4500-a5d5-eeb44f433e3f" />
 

Layout for part 2 has been created
due to the huge size screenshot cannot be taken

PART III: (30 Points) MULTI-BIT ADDER CONSTRUCTION

Two RCA have been made
One is made by the Fa_p1

 <img width="940" height="478" alt="image" src="https://github.com/user-attachments/assets/aa0ca936-6902-4468-979f-f8a1cdefca22" />

another by the Fa_p2
 <img width="940" height="485" alt="image" src="https://github.com/user-attachments/assets/b0fb339d-a733-45b6-8b11-b22a43542b3b" />


both the layouts have been created without any DRC or LVS errors
 RCA_p1  
<img width="1044" height="616" alt="image" src="https://github.com/user-attachments/assets/2c17dbaa-9df6-433d-9860-4395e8573c75" />

RCA_p2
 <img width="1027" height="608" alt="image" src="https://github.com/user-attachments/assets/3edfce06-dcd9-4622-986e-c6952d08b6ac" />

clearly RCA_p1 has less area and was more abutable compared to RCA_p2
