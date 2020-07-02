Code, files and instructions for **module 3** (same flow and instructions as in [<b>module 1</b>](../module1_baseline) to run Vitis, Vitis Analyzer)

No need to run Vitis HLS in this module as the kernel source code is same as in module 2.

The difference here is in the Vitis v++ configuration file which is now assigning local block of RAM within the Xilinx device logic array for faster access:
> By default host in Alveo cards connections are assigned to the DDRs available on the card but since the U50 does not have DDR but HBM instead, data transfers go to that memory.  It is however possible to use smaller memories that are part of the logic array (PLRAMs).