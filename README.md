# CNN-ACCELERATOR
Hardware accelerator for convolutional neural networks implemented in Verilog HDL and the C programming language.
# DATAFLOW ARCHITECTURE

The dataflow architecture of the accelerator is an adaptation of the the BSM (broadcast, stay, migration)  dataflow introduced by Jihyuck Jo et al., which  is Energy-Efficient because it reduces the number of redundant accesses to the off-chip memory. 


![detailed_arq](https://user-images.githubusercontent.com/47645091/172915726-80be5ca7-0af3-4ce4-ba30-2a793b681a7f.png)


# AVALON SYSTEM

The convolution accelerator architecture was deployed in the FPGA DE0-Nano-Soc in conjunction with
a NIOS II processor, an On-Chip Ram, and an On-Chip Dual Port Ram connected via an Avalon
interconnect fabric. Intel Fpga Monitor Software Program was used to read the results of the convolution
performed by the accelerator on the on-chip dual port ram.

![Esquematico_sys](https://user-images.githubusercontent.com/47645091/172916317-0a5fd750-984f-44cd-a74a-4ec11ee7fed0.png)
