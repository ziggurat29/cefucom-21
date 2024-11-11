The source ROM dumps.

MCU2 ROMs.  The first three are the patched Sanyo PCH-25 ROMs:
01.BIN - MCU2, 0000h-1fffh
02.BIN - MCU2, 2000h-3fffh
03.BIN - MCU2, 4000h-5fffh
The 4th maps into the cartridge address space:
04.BIN - MCU2, 7800h-7fffh

PCU ROMs.  These cover the lower 32 KiB:
5-1.BIN - PCU, 0000h-1fffh
6-0.BIN - PCU, 2000h-3fffh
7-0.BIN - PCU, 4000h-5fffh
8-2.BIN - PCU, 6000h-7fffh

This is not the actual chargen ROM, but it comes from a similar machine and is suspected to have the same bit pattern:
map_chargen.bin

I made a tool to dump it to a text representation for reference:
map_chargen.txt

