# Continous rotation servo PCB.

Based on the final project from ENPH259. I've extended the project by creating a PCB and mechanical mount for the project.

By using slots in a disk attached to the motor shaft, I can monitor the rotational speed of the motor. This can then be fed into a counter that resets periodically, and is latched right before every reset. This digital number is then put through an R2R DAC, which is then compared with a reference voltage and fed into a PI controller, that runs a MOSFET driving the motor.

The project requires an external 5V, GND, -5V, and 5 Hz clock signal.
