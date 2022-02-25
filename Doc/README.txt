

Start The QUEMU by running:

"C:\Program Files\qemu\qemu-system-arm.exe" -machine xilinx-zynq-a9 -gdb tcp::1234  -S


00010000 <c_entry-0x20>:
   10000:	e59fd004 	ldr	sp, [pc, #4]	; 1000c <start+0xc>
   10004:	eb000005 	bl	10020 <c_entry>
   10008:	eafffffe 	b	10008 <start+0x8>
   1000c:	00030078 	andeq	r0, r3, r8, ror r0
   10010:	e59fd004 	ldr	sp, [pc, #4]	; 1001c <start+0x1c>
   10014:	eb000001 	bl	10020 <c_entry>
   10018:	eafffffe 	b	10018 <start+0x18>
   1001c:	00030078 	andeq	r0, r3, r8, ror r0
00010020 <c_entry>:
   10020:	e52db004 	push	{fp}		; (str fp, [sp, #-4]!)
   10024:	e28db000 	add	fp, sp, #0
   10028:	e24dd014 	sub	sp, sp, #20
   1002c:	e59f301c 	ldr	r3, [pc, #28]	; 10050 <c_entry+0x30>
   10030:	e5933000 	ldr	r3, [r3]
   10034:	e50b3008 	str	r3, [fp, #-8]
   10038:	e59f3014 	ldr	r3, [pc, #20]	; 10054 <c_entry+0x34>
   1003c:	e5933000 	ldr	r3, [r3]
   10040:	e50b300c 	str	r3, [fp, #-12]
   10044:	e59f300c 	ldr	r3, [pc, #12]	; 10058 <c_entry+0x38>
   10048:	e50b3010 	str	r3, [fp, #-16]
   1004c:	eafffffe 	b	1004c <c_entry+0x2c>
   10050:	00010070 	andeq	r0, r1, r0, ror r0
   10054:	0001006c 	andeq	r0, r1, ip, rrx
   10058:	0001005c 	andeq	r0, r1, ip, asr r0


0001005c <outPutString>: - "\r\nHello world!" -Litle Endrian
   1005c:	6548 0a0d       e  H \n\r
   10060:	206f 6c6c 	   sp  o  l l
   10064:	6c72 6f77 	    l  r  o w
   10068:	0000 2164 	          ! d
Disassembly of section .rw:
0001006c <pi>:
   1006c:	4048f5c3
00010070 <tre>:
   10070:	00000003
