# Important Verilog Practice Questions

**1. Question:** Write a one-line Verilog statement to implement a 2:1 multiplexer.
**Answer:** `assign y = sel ? in1 : in0;`

**2. Question:** Write a Verilog statement to implement a 2:1 multiplexer without using the conditional operator.
**Answer:** `assign y = (in1 & sel) | (in0 & ~sel);`

**3. Question:** Write a one-line Verilog statement to implement a 2-input XOR using only AND, OR, and NOT operators.
**Answer:** `assign y = (a & ~b) | (~a & b);`

**4. Question:** Write a Verilog statement to swap two 1-bit signals without using a temporary variable.
**Answer:** `assign {a, b} = {b, a};`

**5. Question:** Write a one-line Verilog statement to check whether an 8-bit number has even parity.
**Answer:** `assign even_parity = ^data8;`

**6. Question:** Write a one-line Verilog statement to generate the odd parity bit for an 8-bit input.
**Answer:** `assign odd_parity = ~^data8;`

**7. Question:** Write a Verilog statement to implement a 4:1 multiplexer using nested conditional operators.
**Answer:** `assign y = sel[1] ? (sel[0] ? in3 : in2) : (sel[0] ? in1 : in0);`

**8. Question:** Write a Verilog statement to implement a 4-bit 2:1 multiplexer.
**Answer:** `assign y = sel ? a4 : b4;`

**9. Question:** Write a Verilog statement to find the greater of two 8-bit unsigned numbers.
**Answer:** `assign max = (a8 > b8) ? a8 : b8;`

**10. Question:** Write a one-line Verilog statement to check whether two 8-bit numbers are equal.
**Answer:** `assign is_equal = (a8 == b8);`

**11. Question:** Write a Verilog statement to reverse the bits of an 8-bit vector.
**Answer:** `assign rev = {vec[0], vec[1], vec[2], vec[3], vec[4], vec[5], vec[6], vec[7]};`

**12. Question:** Write a one-line Verilog statement to perform a 4-bit 2's complement operation.
**Answer:** `assign twos_comp = ~val4 + 1'b1;`

**13. Question:** Write a Verilog statement to detect whether an 8-bit input is zero.
**Answer:** `assign is_zero = ~|in8;`

**14. Question:** Write a Verilog statement to implement a 1-bit full-adder sum output.
**Answer:** `assign sum = a ^ b ^ cin;`

**15. Question:** Write a Verilog statement to implement a 1-bit full-adder carry output.
**Answer:** `assign cout = (a & b) | (b & cin) | (a & cin);`

**16. Question:** Write a Verilog statement to convert a 4-bit binary number into Gray code.
**Answer:** `assign gray = bin ^ (bin >> 1);`

**17. Question:** Write a Verilog statement to extract the upper four bits of an 8-bit signal.
**Answer:** `assign upper4 = sig[7:4];`

**18. Question:** Write a Verilog statement to exchange the upper and lower four bits of an 8-bit signal.
**Answer:** `assign swapped = {sig[3:0], sig[7:4]};`