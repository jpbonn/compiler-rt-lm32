LM32 Compiler-RT
================================
This can be built out-of-tree using make.  cmake apparently will not work out-of-tree.

LM32 clang should be the default on PATH.  The following LM32 utilities are needed from the GNU binutil package:
AS=lm32-elf-as
LD=lm32-elf-ld
OBJCOPY=lm32-elf-objcopy
AR=lm32-elf-ar
RANLIB=lm32-elf-ranlib

On OSX the system clang is always used.  The hack is to delete: make/platform/clang_*.mk

git clone git://github.com/milkymist/compiler-rt-lm32.git
cd compiler-rt-lm32
make lm32

Note this is untested.
