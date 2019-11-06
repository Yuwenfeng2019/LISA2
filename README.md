# LISA2
Extending project LISA(Linux Integrated System Analysis) with new designs.

Project LISA(https://github.com/ARM-software/lisa) is interesting, but have some limitations from my point of view:
1) Bias towards automated testing, which has overlap in functionality with LAVA(https://www.lavasoftware.org/) 
   from Linaro in some extent;
2) Android-oriented, while it is required to adapt to a much more generalized Linux system;
3) Lack of plug-in mechanism to integrated existed Kernel analysis and test projects.
...

In LISA2, we are trying to extend LISA in the following ways which is divided into two stages in the plan:
Stage I
1)In addition to Ftrace, combining with eBPF support, especially integrate project BCC
  (https://github.com/iovisor/bcc)
2)Architecture redesign (for better support existing Kernel analysis and test utilities) 
  e.g. flexible plug-in mechanism and well-designed interfaces for system extension;
3)Integrate the emerging Linux Kernel test platform KernelCI(https://kernelci.org/)
4)Better support hardware debug interface like JTAG(https://en.wikipedia.org/wiki/JTAG) 
  and SWD(https://www.arm.com/files/pdf/Serial_Wire_Debug.pdf);
5)Integrate good on-chip debugger like OpenOCD(openocd.org);
...

Stage II
1) More CoreSight
   (https://developer.arm.com/architectures/cpu-architecture/debug-visibility-and-trace/coresight-architecture) 
   support is preferred;
...
