# RC2014-FORTH

I know NOTHING about FORTH but I just want something simple to mess around with.

I found a simple FORTH buried in a ZIP file on the Z80 info site at ...

http://www.z80.info/zip/z80asm.zip

I have no idea of it's origin but from snooping around it seems to be fig-forth-79 or based on that.

https://archive.org/details/FigFORTHGlossary

I combined it with Grant Searles initialisation and referenced the routines for the TXA and RXA where necessary.

Built with  ... TASM -80 -b -c -dROM FORTH.Z80 FORTHROM.bin FORTHROM.lst ... For ROM binary

or 

Built with ... TASM -80 -g0 FORTH.Z80 FORTHRAM.hex FORTHRAM.lst ... For RAM Hex file to run from Monitor

After some messing around and realising that I need to AND 7F to knock off the top bit of the characters
as it uses this as an end of word marker.


