# Task 1

Task is to install all the essential tools required for this internship such as Ubuntu on VMBox, GNU Toolchain, GTKWave, Yosys and iVerilog simulator.

---

## 1. Install Ubuntu on VirtualBox

Install Ubuntu 20.04 LTS on Oracle Virtual Machine Box.

---

## 2. Install RISC-V GNU Toolchain

What is RISC-V GNU Toolchain?

> The RISC-V GNU Compiler Toolchain is a free and open source cross-compiler for C and C++. It supports Generic ELF/Newlib and Linux-ELF/glibc build modes.

Use these commands:
```bash
sudo apt install git
git clone https://github.com/riscv/riscv-gnu-toolchain
sudo apt-get install autoconf automake autotools-dev curl python3 python3-pip libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev ninja-build git cmake libglib2.0-dev libslirp-dev
mkdir /opt/riscv
./configure --prefix=/opt/riscv --with-arch=rv64i --with-abi=lp64 --enable-multilib
sudo make

