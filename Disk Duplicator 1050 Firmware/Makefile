all: duplicator-3.00.rom duplicator-3.10.rom

ATASM=atasm
ASMFLAGS=

duplicator-3.10.rom: DD15M0.ASM DD15M1.ASM DD15M2.ASM DD15M3.ASM DD15M4.ASM DD15M5.ASM DD15M6.ASM
	$(ATASM) $(ASMFLAGS) -r -f0 -o$@ $<

duplicator-3.00.rom: DD15M0.ASM DD15M1.ASM DD15M2.ASM DD15M3.ASM DD15M4.ASM DD15M5.ASM DD15M6.ASM
	$(ATASM) $(ASMFLAGS) -r -f0 -dREV300=1 -o$@ $<

.PHONY: clean
clean:
	rm -f duplicator-3.00.rom duplicator-3.10.rom
