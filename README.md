# ElfParser
despite this program is called ElfParser, it can only read the dynamic symbols in shared object. i write this program so that i can read the dynamic symbols in Windows rather than use nm in linux. and the name of dynamic symbols is essential for us when we want to dlsym some symbols.
Beside, these codes can be used to do got hook, just as i use in another project named android-inject-and-hook. it can find the offset of the item for dynamic symbols in GOT.
the code can be compile to support 32-bit or 64-bit ELF, you just have to add or move the macro named __aarch64__.
