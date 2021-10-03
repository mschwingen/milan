# Milan RomPortConnector-PCB

![RoPoCop-PCB Photo](RoPoCop1.jpg?raw=true "RoPoCop PCB")

The RoPoCop PCB allows connection of classic Atari ST ROM cartridges to the
Milan. This started as a slightly modified version of the RoPoCop-PCB by MW
electronic for the Hades (V1, V2 shows the modifications done for the
Milan). The original RoPoCop has 3 romport sockets (1 external on the ISA
slot bracket, 2 internal), which are mapped to the ISA address space. By use
of the 68040 MMU, one of these can be mapped to the original Atari rom port
address space.

V3 was an attempt at a stripped-down, Milan-only version with 1
socket. Schematic and Layout were finished, but it never made it into
(prototype) production. V1 and V2 schematics were reverse-engineered from
the original RoPoCop PCBs, so there is no guarantee for correctness.

Schematic and PCB files were made using Protel 3 (these can be opened using
Altium Designer). I have also exported ASCII versions of these files, since
they may be easier to import into other EDA tools.

The GAL sources are ABEL format and used Lattice ISP Synario tools to
translate.
