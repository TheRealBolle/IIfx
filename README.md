# Macintosh IIfx Logicboard recreation
  
This is a recreation of the Macintosh IIfx logicboard.  
It is not a 1:1 copy of the original logicboard but instead the original board was traced out to create schematics that were used to completely redesign and route a lookalike board.  
  
![fully populated board](/iifx.jpg)
  
The provided logicboard files are licensed under CC-BY-NC-SA - they are NOT intended for commercial use.  

  
# Reverse engineered PALs
  
The original PALs have been reverse-engineered and equations were rewritten to match the behaviour of the originals - the provided
JEDEC files are not dumps of the content of the original chips. They mostly seem to work for the test cases I was able to perform.
Most PALs handle parts of the bus arbitration between the different DMA devices on the board. Certain expansion card combinations that involve bus mastering have yet ot be tested with the rewritten equations.

The provided JEDEC files are intended to be used with a 16V8-type device (GAL16V8, PALCE16V8, ATF16V8) as a replacement
for the video, clock and RAM-signalling PALs. Certain low power ATF16V8B don't work. ATF16V8C use pinkeepers instead of internal pullups and might be problematic as well.  
  
Board locations and original part number reference:  
  
UJ7 341S0751  
UK7 341S0750 
UL6 341S0766-2  
UL8 341S0765  
UN9 341S0719  
UP16 341S0773  
  

  
# Board Files
  
The provided gerber files have been generated using the JLCPCB EAGLE cam job files.  
Other manufacturers might have different requirements to the gerbers.  
  
