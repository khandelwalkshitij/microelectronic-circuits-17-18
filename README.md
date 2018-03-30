##### Resources:
1. [List of Teaching Assistants (Use BITS Mail Account to log in and view)](https://docs.google.com/spreadsheets/d/1mZVkgLm2miW1pYADgRn2tXi6tSlGk4C-xHr2PJEK3Ss/edit?usp=sharing)
2. [AC Analysis using LT SPICE (Write the Netlist instead of drawing the schematic) ](https://www.youtube.com/watch?v=fziUQaVQxA4)
3. [SPICE Commands](http://www.ecircuitcenter.com/SPICEsummary.htm)

##### Expectations from Students:
1. As a part of this course, students are expected to conduct all simulation by writing the SPICE Netlists themselves without the use of Schematic.
2. Students are expected to be crystal-clear with their concepts in Micro-electronic Circuits. Any doubts with the same should be clarified with the course instructor or any of the teaching assistants. It is also suggested that this exercise should be performed **much** before the test and not at the last minute.
3. Using LT Spice is a lot about practice. Do not expect to magically understand the use of the software just on the basis of the demo sessions. A hands-on experience of the software is irrefutable in order to understand it's usage.


It is also suggested that you keep checking this repository for problems, resources, etc. Notices for the same shall be put on Nalanda.

###### Explaination for Gain Margin and Phase Margin

Gain margin and phase margin are two parameters to assess the performance of a circuit. Depending on the values of both, we judge factors such as the stability of the circuit etc. 

###### Gain Margin: 
The value of the gain at the same frequency where the phase crosses -180° is called as the gain margin of the circuit. The frequency at which the phase crosses -180° is called  phase crossover frequency. Hence, the value of the gain at the phase crossover frequency is called as the gain margin. 

###### Phase Margin: 
The value of the phase relative to -180°, at the same frequency at which the gain crosses 0dB (gain crossover frequency) is called as the phase margin. 
The following figure shows the gain margin and the phase margin for a particular circuit. 

![alt text] (https://github.com/khandelwalkshitij/microelectronic-circuits-17-18/blob/master/gm_pm.png)

Usually, for any circuit, the gain crossover frequency is less than the phase crossover frequency. 
Both these parameters can be calculated in LT-SPICE also. The following figure shows a sample graph from a cascade amplifier simulation done in class. 

![alt text] (https://github.com/khandelwalkshitij/microelectronic-circuits-17-18/blob/master/gm_pm_sim.png)

The cursor can be obtained by left clicking the ‘V(3)’ written at the heading of the graph. The cursor is shifted till the magnitude field in the box shows 0 dB (or a value closest). The phase margin s calculated at this value. The value of the phase is measured and the phase relative to -180° is calculated. 

++++ e.g. In this case, the phase margin is 20.93 - (-180) = 200.93°. ++++

Similarly, the value of the gain margin can be calculated by moving the cursor to a point where value of phase is -180°.  
