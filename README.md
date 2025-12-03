# Hello World in Binary/Machine Code

This repository contains "Hello World" represented in raw binary and machine code formats without using any programming language.

## Files

- **hello-world.txt** - Contains the binary, hexadecimal, and octal representations of "Hello World"
- **hello-world.bin** - Raw binary file containing the actual bytes

## Representations

### Binary (8-bit ASCII)
Each character is represented as 8 bits:
```
H = 01001000
e = 01100101
l = 01101100
l = 01101100
o = 01101111
(space) = 00100000
W = 01010111
o = 01101111
r = 01110010
l = 01101100
d = 01100100
```

### Hexadecimal (Machine Code)
The same message in hex format:
```
48 65 6C 6C 6F 20 57 6F 72 6C 64
```

### How to Verify

You can verify the binary file contents using:
```bash
hexdump -C hello-world.bin
```

Or view the raw bytes:
```bash
xxd hello-world.bin
```