# Verilator example sources for Verilog/SystemVerilog verification with C++

The sources in this repository contain an Arithmetic Logic Unit (ALU, *alu.sv*) writen in SystemVerilog as the Device-Under-Test (DUT), a Verilator C++ testbench (*alu_tb.cpp*), and an accompanying Makefile to build, simulate and display waveforms.

Dependencies: you need to have verilator, gtkwave, gcc, make installed on your system. 
Written and tested primarily under Arch Linux, known to be working on Ubuntu 20.04 and 18.04.

To simulate the testbench, simply run `make` in the root of the repo.
To draw waveforms, run `make waves`.

You can find beginner friendly Verilator tutorials here:

*    [Verilator Tutorial Pt.1: Introduction](https://www.itsembedded.com/dhd/verilator_1/)
*    [Verilator Tutorial Pt.2: Basics of SystemVerilog verification using C++](https://www.itsembedded.com/dhd/verilator_2/)
*    [Verilator Tutorial Pt.3: Traditional style verification example](https://www.itsembedded.com/dhd/verilator_3/)
*    [Verilator Tutorial Pt.4: Modern transactional (UVM) style C++ testbench](https://www.itsembedded.com/dhd/verilator_4/)

Please visit the links above or www.itsembedded.com for more info.


Below are the tags you can check out:
* **verilator_pt1** for a minimal testbench source that simply builds and generates a clock signal to the DUT
* **verilator_pt2** is based on verilator_pt1 testbench with a reset method and some primitive verification functionality
* **verilator_pt3** is based on verilator_pt2 testbench and has a traditional (sequential, time based) verification example.
* **verilator_pt4** is a transactional (UVM) style testbench with a transaction generator, driver, monitors and scoreboard implemented in raw C++.

```
git clone https://github.com/n-kremeris/verilator_basics
git checkout <tag_name>
```




Norbertas Kremeris 2021
