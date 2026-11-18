+++
title      = "assembly language"
date       = 2026-11-14T15:42:58-04:00
tags       = ["asm"]
identifier = "20261114T154258"
+++

the cpu has memmory called registers

`mov rax, 3` : move to register rax 3
`mov rbx, 4` : move to register rbx 4
`add rax, rbc` : add to register rax rbx

hex is 4 bits

`rip` : instruction pointer register
`rsp` : stack pointer register
`rbp` : base pointer resister

`mov rax, 1`
`add rax, 3`
`add rax, rbx`
`sub rax, 2`
`inc rax`: increment rax

```asm
.global _start
.text

_start:
mov rax, [req16]  /* move data from address reg16 */
lea rax, [reg16]  /* load effective address */
mov al, [reg16] /* move to lowest byte al */
add rax, 8 /* move to the next 8 bytes address */
lea rax, [mem] /* load address to rax */
mov [mem], rax  /* move to memory */

.data
reg16: .quad 0x1234567890abcdef
reg17: .quad 0xaaaaaaaaaaaaaaaa 
mem: .byte 0x1, 0x2, 0x3, 0x4  /* write bytes */
     .word 0xabcd /* write words */
	 .skip 1024, 0xff  /* fill a kilobyte with ff */
```
a WORD is 16bits or 2 bytes 0xaa
a DOUBLE is 32bits or 4 bytes or 2 WORDS 0xaaaa
a QUAD is 64bits or 8 bytes of 4 WORDS 0xaaaaaaaa
