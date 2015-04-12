LM32 Compiler-RT
================================
This can be built out-of-tree using make.  cmake apparently will not work out-of-tree.

LM32 clang should be the default on PATH.  GNU LM32 binutils are used for linking and assembly. 

On OSX the system clang is always used.  The hack is to delete: make/platform/clang_*.mk

git clone git://github.com/milkymist/compiler-rt-lm32.git
cd compiler-rt-lm32
make lm32

Note this is untested.
