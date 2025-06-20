# Continous rotation servo PCB.

Based on the final project from ENPH259. I've extended the project by creating a PCB and mechanical mount for the project.

I've also included an optional 'speed readout' on the board itself. This displays the current revolutions per cycle of the servo in binary.

By using slots in a disk attached to the motor shaft, I can monitor the rotational speed of the motor. This can then be fed into a counter that resets periodically, and is latched right before every reset. This digital number is then put through an R2R DAC, which is then compared with a reference voltage and fed into a PI controller, that runs a MOSFET driving the motor.

The project requires an external 5V, GND, -5V, and 5 Hz clock signal.

![final-product](https://github.com/user-attachments/assets/f0ccd1d3-18b3-4a7a-b99a-84ee22a1c312)
![enph259-servo](https://github.com/user-attachments/assets/533800ff-53f0-4b58-b47d-1a5afa88ceae)
![enph259-servo-board-only](https://github.com/user-attachments/assets/5b297364-0aed-488e-a999-2987d55b918e)
