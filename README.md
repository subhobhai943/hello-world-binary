# Hello World in Binary/Machine Code

This repository contains "Hello World" represented in raw binary and machine code formats without using any high-level programming language.

## Files

- **hello-world.hex** - Pure hexadecimal representation (raw bytes)
- **hello-world-binary.txt** - Pure binary (1s and 0s)
- **x86-machine-code.txt** - Actual x86-64 machine code instructions
- **x86-hello-world.asm.txt** - Assembly code for reference (lowest level before machine code)
- **hello-world.txt** - Human-readable format breakdown

## Pure Binary Format

### Hexadecimal (Raw Bytes)
```
48 65 6C 6C 6F 20 57 6F 72 6C 64
```
This is the actual data stored in memory - each pair of hex digits represents one byte.

### Binary (Bits)
```
01001000 01100101 01101100 01101100 01101111 00100000
01010111 01101111 01110010 01101100 01100100
```
This is how the data appears at the bit level in computer memory.

## Machine Code

The `x86-machine-code.txt` file contains actual CPU instructions in hexadecimal format. These are the binary opcodes that an x86-64 processor executes directly:

- `B8 01 00 00 00` - Move value 1 into register RAX
- `0F 05` - Execute system call
- etc.

This is true machine code - the lowest level of computer instructions.

## Character Encoding Table

| Character | Binary | Hex | Decimal |
|-----------|--------|-----|----------|
| H | 01001000 | 48 | 72 |
| e | 01100101 | 65 | 101 |
| l | 01101100 | 6C | 108 |
| l | 01101100 | 6C | 108 |
| o | 01101111 | 6F | 111 |
| (space) | 00100000 | 20 | 32 |
| W | 01010111 | 57 | 87 |
| o | 01101111 | 6F | 111 |
| r | 01110010 | 72 | 114 |
| l | 01101100 | 6C | 108 |
| d | 01100100 | 64 | 100 |

## How to View Raw Bytes

To see the actual bytes in hexadecimal format:
```bash
xxd hello-world.hex
hexdump -C hello-world.hex
```