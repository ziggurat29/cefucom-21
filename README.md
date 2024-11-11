# cefucom-21
Cefucom-21 reverse engineering work

At the moment this consists of my ROM disassembly work.  The Cefucom-21 has two Z80 subsystems on two boards:  a 'main' board, which has a silkscreen marking of "MCU2", and an 'i/o' board, which has a marking (on later units) of "PCU".  So I use that nomenclature.

The MCU is derived from a Sanyo PCH-25 design, adding a bit of hardware (a Z80-PIO), and a 2 KiB ROM in what was the cartridge address space.  The Sanyo ROM is lightly patched to thunk over to the Cefucom ROM that does the additional hardware setup and presents a menu of options.

The PCU is to wit an original design (though it shows evidence of being built from library/framework code rather than completely from scratch).  It controls the distinctive hardware of the Cefucom.  I do not have schematics, so my work infers hardware particulars from the context provided by the code.