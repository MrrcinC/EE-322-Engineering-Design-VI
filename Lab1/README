## Lab 1 — GHDL and GTKWave

Windows Binaries of GHDL and GTKWave were downloaded and used for this demonstration.
Please ensure that when running gtkwave to display the output from ghdl, you match the file path of the vcd files accurately.

### Half Adder
```
library ieee;
use ieee.std_logic_1164.all;
entity ha is
		port
		(
			a: in std_ulogic;
			b: in std_ulogic;
			o: out std_ulogic;
			c: out std_ulogic
		);
end ha;

architecture behave of ha is
begin
	o <= a xor b;
	c <= a and b;
end behave;
```
'''
library ieee; 
use ieee.std_logic_1164.all;

entity ha_tb is
end ha_tb;

architecture test of ha_tb is
	component ha
		port
		(
			a: in std_ulogic;
			b: in std_ulogic;
			o: out std_ulogic;
			c: out std_ulogic
		);
	end component;
	
	signal a, b, o, c : std_ulogic;
begin
	half_adder: ha port map (a => a, b => b, o => o, c => c);
	
	process begin
	
		a <= 'X';
		b <= 'X';
		wait for 1 ns;
		
		a <= '0';
		b <= '0';
		wait for 1 ns;
		
		a <= '0';
		b <= '1';
		wait for 1 ns;
		
		a <= '1';
		b <= '0';
		wait for 1 ns;
		
		a <= '1';
		b <= '1';
		wait for 1 ns;
		
		assert false report "Reached end of test";
		wait;
	
	end process;
	
end test;
'''

![Image](https://github.com/user-attachments/assets/5d5ef5a1-5e65-4185-af51-344c2710800d)

### D Flip-Flop
```
ghdl -a dff.vhdl
ghdl -a dff_tb.vhdl
ghdl -e dff_tb
ghdl -r dff_tb --vcd=dff.vcd
gtkwave dff.vcd
