# VHDL Counter Overflow Bug
This repository demonstrates a common bug in VHDL code: counter overflow. The `buggy_counter.vhdl` file contains a counter that does not handle overflow correctly.  When the counter reaches its maximum value (15), incrementing it further leads to undefined behavior. The `fixed_counter.vhdl` provides a corrected version of the code that addresses the overflow issue. 

## Bug Description
The original VHDL code lacks proper handling for the counter when it reaches the maximum value.  Simple increment may wrap around or cause unexpected simulation results. This can be especially problematic in hardware implementations, potentially leading to unpredictable behavior or even system failure. 

## Solution
The corrected code utilizes a modulo operator to reset the counter to 0 once it reaches the maximum value, preventing overflow and ensuring predictable behavior. 