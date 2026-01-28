
This is me walking through the steps to fabricate my first transistors
#### Design (From Verilog logic -> fabrication masks):

The first step is to write a quick inverter in verilog. This comes out looking like:

`module inverter(in, out);
`input in;
`output out;
`not inv1(in, out);`
`endmodule`

That's it!

Next we use a free open source tool called yosys in orrder to synthesize this verilog into a netlist using its standard cell library.
